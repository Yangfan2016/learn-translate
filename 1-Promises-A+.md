## Promises/A+ 规范
> 原文： https://promisesaplus.com/  

**An open standard for sound, interoperable JavaScript promises—by implementers, for implementers.**

A promise represents the eventual result of an asynchronous operation. The primary way of interacting with a promise is through its then method, which registers callbacks to receive either a promise’s eventual value or the reason why the promise cannot be fulfilled.

This specification details the behavior of the then method, providing an interoperable base which all Promises/A+ conformant promise implementations can be depended on to provide. As such, the specification should be considered very stable. Although the Promises/A+ organization may occasionally revise this specification with minor backward-compatible changes to address newly-discovered corner cases, we will integrate large or backward-incompatible changes only after careful consideration, discussion, and testing.

Historically, Promises/A+ clarifies the behavioral clauses of the earlier Promises/A proposal, extending it to cover de facto behaviors and omitting parts that are underspecified or problematic.

Finally, the core Promises/A+ specification does not deal with how to create, fulfill, or reject promises, choosing instead to focus on providing an interoperable then method. Future work in companion specifications may touch on these subjects.

### 1. Terminology

1.1 “promise” is an object or function with a then method whose behavior conforms to this specification.

1.2 “thenable” is an object or function that defines a then method. 

1.3 “value” is any legal JavaScript value (including undefined, a thenable, or a promise).

1.4 “exception” is a value that is thrown using the throw statement.

1.5 “reason” is a value that indicates why a promise was rejected.

### 2. Requirements

#### 2.1 Promise States

A promise must be in one of three states: pending, fulfilled, or rejected.

2.1.1 When pending, a promise:   

- 2.1.1.1 may transition to either the fulfilled or rejected state.

2.1.2 When fulfilled, a promise:

- 2.1.2.1 must not transition to any other state.

- 2.1.2.2 must have a value, which must not change.

2.1.3 When rejected, a promise:  

- 2.1.3.1 must not transition to any other state.

- 2.1.3.2 must have a reason, which must not change.

Here, “must not change” means immutable identity (i.e. ===), but does not imply deep immutability.

#### 2.2 The then Method

A promise must provide a then method to access its current or eventual value or reason.

A promise’s then method accepts two arguments:

`promise.then(onFulfilled, onRejected)`  

2.2.1 Both onFulfilled and onRejected are optional arguments:

- 2.2.1.1 If onFulfilled is not a function, it must be ignored.  

- 2.2.1.2 If onRejected is not a function, it must be ignored. 

2.2.2 If onFulfilled is a function:

- 2.2.2.1 it must be called after promise is fulfilled, with promise’s value as its first argument.

- 2.2.2.2 it must not be called before promise is fulfilled.

- 2.2.2.3 it must not be called more than once.

2.2.3 If onRejected is a function:

- 2.2.3.1 it must be called after promise is rejected, with promise’s reason as its first argument.

- 2.2.3.2 it must not be called before promise is rejected.

- 2.2.3.3 it must not be called more than once.

2.2.4 onFulfilled or onRejected must not be called until the execution context stack contains only platform code. [3.1]. 

2.2.5 onFulfilled and onRejected must be called as functions (i.e. with no this value). [3.2]

2.2.6 then may be called multiple times on the same promise.

- 2.2.6.1 If/when promise is fulfilled, all respective onFulfilled callbacks must execute in the order of their originating calls to then.

- 2.2.6.2 If/when promise is rejected, all respective onRejected callbacks must execute in the order of their originating calls to then.

2.2.7 then must return a promise [3.3].

 `promise2 = promise1.then(onFulfilled, onRejected);`

- 2.2.7.1 If either onFulfilled or onRejected returns a value x, run the Promise Resolution Procedure [[Resolve]](promise2, x).

- 2.2.7.2 If either onFulfilled or onRejected throws an exception e, promise2 must be rejected with e as the reason.

- 2.2.7.3 If onFulfilled is not a function and promise1 is fulfilled, promise2 must be fulfilled with the same value as promise1.

- 2.2.7.4 If onRejected is not a function and promise1 is rejected, promise2 must be rejected with the same reason as promise1.

#### 2.3 The Promise Resolution Procedure

The promise resolution procedure is an abstract operation taking as input a promise and a value, which we denote as [[Resolve]](promise, x). If x is a thenable, it attempts to make promise adopt the state of x, under the assumption that x behaves at least somewhat like a promise. Otherwise, it fulfills promise with the value x.

This treatment of thenables allows promise implementations to interoperate, as long as they expose a Promises/A+-compliant then method. It also allows Promises/A+ implementations to “assimilate” nonconformant implementations with reasonable then methods.

To run [[Resolve]](promise, x), perform the following steps:

2.3.1 If promise and x refer to the same object, reject promise with a TypeError as the reason.

2.3.2 If x is a promise, adopt its state [3.4]:

- 2.3.2.1 If x is pending, promise must remain pending until x is fulfilled or rejected.

- 2.3.2.2 If/when x is fulfilled, fulfill promise with the same value.

- 2.3.2.3 If/when x is rejected, reject promise with the same reason.

2.3.3 Otherwise, if x is an object or function,

- 2.3.3.1 Let then be x.then. [3.5]

- 2.3.3.2 If retrieving the property x.then results in a thrown exception e, reject promise with e as the reason.

- 2.3.3.3 If then is a function, call it with x as this, first argument resolvePromise, and second argument rejectPromise, where:

    - 2.3.3.3.1 If/when resolvePromise is called with a value y, run [[Resolve]](promise, y).

    - 2.3.3.3.2 If/when rejectPromise is called with a reason r, reject promise with r.  

    - 2.3.3.3.3 If both resolvePromise and rejectPromise are called, or multiple calls to the same argument are made, the first call takes precedence, and any further calls are ignored.

    - 2.3.3.3.4 If calling then throws an exception e,

        - 2.3.3.3.4.1 If resolvePromise or rejectPromise have been called, ignore it.

        - 2.3.3.3.4.2 Otherwise, reject promise with e as the reason.

- 2.3.3.4 If then is not a function, fulfill promise with x.

2.3.4 If x is not an object or function, fulfill promise with x.

If a promise is resolved with a thenable that participates in a circular thenable chain, such that the recursive nature of [[Resolve]](promise, thenable) eventually causes [[Resolve]](promise, thenable) to be called again, following the above algorithm will lead to infinite recursion. Implementations are encouraged, but not required, to detect such recursion and reject promise with an informative TypeError as the reason. [3.6]

### 3.Notes

3.1 Here “platform code” means engine, environment, and promise implementation code. In practice, this requirement ensures that onFulfilled and onRejected execute asynchronously, after the event loop turn in which then is called, and with a fresh stack. This can be implemented with either a “macro-task” mechanism such as setTimeout or setImmediate, or with a “micro-task” mechanism such as MutationObserver or process.nextTick. Since the promise implementation is considered platform code, it may itself contain a task-scheduling queue or “trampoline” in which the handlers are called.

3.2 That is, in strict mode this will be undefined inside of them; in sloppy mode, it will be the global object.

3.3 Implementations may allow promise2 === promise1, provided the implementation meets all requirements. Each implementation should document whether it can produce promise2 === promise1 and under what conditions.

3.4 Generally, it will only be known that x is a true promise if it comes from the current implementation. This clause allows the use of implementation-specific means to adopt the state of known-conformant promises.

3.5 This procedure of first storing a reference to x.then, then testing that reference, and then calling that reference, avoids multiple accesses to the x.then property. Such precautions are important for ensuring consistency in the face of an accessor property, whose value could change between retrievals.

3.6 Implementations should not set arbitrary limits on the depth of thenable chains, and assume that beyond that arbitrary limit the recursion will be infinite. Only true cycles should lead to a TypeError; if an infinite chain of distinct thenables is encountered, recursing forever is the correct behavior.