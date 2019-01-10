## Promises/A+ 规范
> 原文： https://promisesaplus.com/  

**An open standard for sound, interoperable JavaScript promises—by implementers, for implementers.**

**一个开放标准，对于开发人员可互操作的 Javascript 承诺**

A promise represents the eventual result of an asynchronous operation. The primary way of interacting with a promise is through its then method, which registers callbacks to receive either a promise’s eventual value or the reason why the promise cannot be fulfilled.

一个 promise 代表一个异步操作的最终结果。主要的操作方式是通过调用 promise 的 then 方法，它接受的回调函数接受 promise 成功的结果或失败的原因

This specification details the behavior of the then method, providing an interoperable base which all Promises/A+ conformant promise implementations can be depended on to provide. As such, the specification should be considered very stable. Although the Promises/A+ organization may occasionally revise this specification with minor backward-compatible changes to address newly-discovered corner cases, we will integrate large or backward-incompatible changes only after careful consideration, discussion, and testing.

这个规范详细的描述了 then 方法的行为，提供一个互操作基础，所有符合 Promises/A+ 的都可以依赖这个标准实现。因此，该规范已经十分稳定。尽管 Promises/A+ 组织可能会偶尔修改以实现向后兼容，我们也会整合这些大的或不能向后兼容的改变，一起研究，讨论，测试。


Historically, Promises/A+ clarifies the behavioral clauses of the earlier Promises/A proposal, extending it to cover de facto behaviors and omitting parts that are underspecified or problematic.

曾经， Promises/A+ 解释了早期 PromisesA 提议的条款，扩展了事实上的行为和忽略了不标准和有问题的部分。

Finally, the core Promises/A+ specification does not deal with how to create, fulfill, or reject promises, choosing instead to focus on providing an interoperable then method. Future work in companion specifications may touch on these subjects.

最终，Promises/A+ 规范并没处理如何创建 fulfill，或 reject promise，而选择了可互操作的 then 方法替代。在今后的工作中可能会考虑。


### 1. Terminology

### 1. 术语

1.1 “promise” is an object or function with a then method whose behavior conforms to this specification.

1.1 ‘promoise’ 是一个有符合此标准的 then 方法的 object 或 function 

1.2 “thenable” is an object or function that defines a then method. 

1.2 ‘thenable’ 是 then 方法定义的 object 或 function

1.3 “value” is any legal JavaScript value (including undefined, a thenable, or a promise).

1.3 ‘value’ 是一个 Javascript 合法值（包括 undefined，thenable，promise）

1.4 “exception” is a value that is thrown using the throw statement.

1.4 ‘exception’ 是一个 throw 语句抛出错误的值

1.5 “reason” is a value that indicates why a promise was rejected.

1.5 ‘reason’ 是一个表明 promise 失败的原因的值

### 2. Requirements

### 2. 要求

#### 2.1 Promise States

#### 2.1 Promise 状态

A promise must be in one of three states: pending, fulfilled, or rejected.

一个 promise 有且只有一个状态（pending，fulfilled，rejected 其中之一）

2.1.1 When pending, a promise:   

2.1.1 pending 状态时：

- 2.1.1.1 may transition to either the fulfilled or rejected state.

- 2.1.1.1 可能会转变为 fulfilled 或 rejected 状态

2.1.2 When fulfilled, a promise:

2.1.2 fulfilled 状态时：

- 2.1.2.1 must not transition to any other state.

- 2.1.2.1 不能再状态为任何其他状态

- 2.1.2.2 must have a value, which must not change.

- 2.1.2.2 必须有一个 value，且不可改变

2.1.3 When rejected, a promise:  

2.1.3 rejected 状态时：

- 2.1.3.1 must not transition to any other state.

- 2.1.3.1 不能再状态为任何其他状态

- 2.1.3.2 must have a reason, which must not change.

- 2.1.3.2 必须有一个 reason，且不可改变


Here, “must not change” means immutable identity (i.e. ===), but does not imply deep immutability.

注：这里 ‘不可改变’ 意思是不可变恒等（同理 === ），但不意味永远不可变

#### 2.2 The then Method

#### 2.2 then 方法

A promise must provide a then method to access its current or eventual value or reason.

一个 promise 必须提供一个 then 方法，用来获取当前或最终的 value 或 reason

A promise’s then method accepts two arguments:

一个 promise 的 then 方法接受两个参数：

`promise.then(onFulfilled, onRejected)`  

2.2.1 Both onFulfilled and onRejected are optional arguments:

2.2.1 onFulfilled 和 onRejected 都是可选参数：

- 2.2.1.1 If onFulfilled is not a function, it must be ignored.  

- 2.2.1.1 如果 onFulfilled 不是函数，它会被忽略

- 2.2.1.2 If onRejected is not a function, it must be ignored. 

- 2.2.1.2 如果 onRejected 不是函数，它会被忽略


2.2.2 If onFulfilled is a function:

2.2.2 如果 onFulfilled 是一个函数：

- 2.2.2.1 it must be called after promise is fulfilled, with promise’s value as its first argument.

- 2.2.2.1 它一定是在 promise 是 fulfilled 状态后调用，并且接受一个参数 value

- 2.2.2.2 it must not be called before promise is fulfilled.

- 2.2.2.2 它一定是在 promise 是 fulfilled 状态后调用

- 2.2.2.3 it must not be called more than once.

- 2.2.2.3 它最多被调用一次

2.2.3 If onRejected is a function:

2.2.3 如果 onRejected 是一个函数：

- 2.2.3.1 it must be called after promise is rejected, with promise’s reason as its first argument.

- 2.2.3.1 它一定在 promise 是 rejected 状态后调用，并且接受一个参数 reason

- 2.2.3.2 it must not be called before promise is rejected.

- 2.2.3.2 它一定在 promise 是 rejected 状态后调用

- 2.2.3.3 it must not be called more than once.

- 2.2.3.3 它最多被调用一次

2.2.4 onFulfilled or onRejected must not be called until the execution context stack contains only platform code. [3.1]. 

2.2.4 onFulfilled 或 onRejected 只在执行环境堆栈只包含平台代码之后调用 [3.1]

2.2.5 onFulfilled and onRejected must be called as functions (i.e. with no this value). [3.2]

2.2.5 onFulfilled 和 onRejected 会作为函数形式调用 (也就是说，默认 this 指向 global，严格模式 undefined) [3.2]

2.2.6 then may be called multiple times on the same promise.

2.2.6 在同一个 promise 实例中，then 可以链式调用多次

- 2.2.6.1 If/when promise is fulfilled, all respective onFulfilled callbacks must execute in the order of their originating calls to then.

- 2.2.6.1 如果或当 promise 转态是 fulfilled 时，所有的 onFulfilled 回调回以他们注册时的顺序依次执行

- 2.2.6.2 If/when promise is rejected, all respective onRejected callbacks must execute in the order of their originating calls to then.

- 2.2.6.2 如果或当 promise 转态是 rejected 时，所有的 onRejected 回调回以他们注册时的顺序依次执行

2.2.7 then must return a promise [3.3].

2.2.7 then 方法一定返回一个 promise

 `promise2 = promise1.then(onFulfilled, onRejected);`

- 2.2.7.1 If either onFulfilled or onRejected returns a value x, run the Promise Resolution Procedure [[Resolve]](promise2, x).

- 2.2.7.1 如果 onFulfilled 或 onRejected 返回的是一个 x，那么它会以 [[Resolve]](promise2, x) 处理解析

- 2.2.7.2 If either onFulfilled or onRejected throws an exception e, promise2 must be rejected with e as the reason.

- 2.2.7.2 如果 onFulfilled 或 onRejected 里抛出了一个异常，那么 promise2 必须捕获这个错误（接受一个 reason 参数）

- 2.2.7.3 If onFulfilled is not a function and promise1 is fulfilled, promise2 must be fulfilled with the same value as promise1.

- 2.2.7.3 如果 onFulfilled 不是一个函数，并且 promise1 状态是 fulfilled，那么 promise2 一定会接受到与 promse1 一样的值 value

- 2.2.7.4 If onRejected is not a function and promise1 is rejected, promise2 must be rejected with the same reason as promise1.

- 2.2.7.4 如果 onRejected 不是一个函数，并且 promise1 状态是 rejected，promise2 一定会接受到与 promse1 一样的值 reason

#### 2.3 The Promise Resolution Procedure

#### 2.3 Promise 处理程序

The promise resolution procedure is an abstract operation taking as input a promise and a value, which we denote as [[Resolve]](promise, x). If x is a thenable, it attempts to make promise adopt the state of x, under the assumption that x behaves at least somewhat like a promise. Otherwise, it fulfills promise with the value x.

promise 处理程序是一个表现形式为 [[Resolve]](promise, x) 的抽象处理操作。如果 x 是 thenable 类型，它会尝试生成一个 promise 处理 x，否则它将直接 resolve x

This treatment of thenables allows promise implementations to interoperate, as long as they expose a Promises/A+-compliant then method. It also allows Promises/A+ implementations to “assimilate” nonconformant implementations with reasonable then methods.

只要 then 方法符合 Promises/A+ 规则，那么对 thenables 处理就允许实现可互操作（链式调用，层层传递下去）。它也允许对那些不符合 Promises/A+ 的 then 方法进行 “吸收”

To run [[Resolve]](promise, x), perform the following steps:

[[Resolve]](promise, x) 的执行表现形式如下步骤：

2.3.1 If promise and x refer to the same object, reject promise with a TypeError as the reason.

2.3.1 如果返回的 promise1 和 x 是指向同一个引用（循环引用），则抛出错误

2.3.2 If x is a promise, adopt its state [3.4]:

2.3.2 如果 x 是一个 promise 实例，则采用它的状态：

- 2.3.2.1 If x is pending, promise must remain pending until x is fulfilled or rejected.

- 2.3.2.1 如果 x 是 pending 状态，那么保留它（递归执行这个 promise 处理程序），直到 pending 状态转为 fulfilled 或 rejected 状态

- 2.3.2.2 If/when x is fulfilled, fulfill promise with the same value.

- 2.3.2.2 如果或当 x 状态是 fulfilled，resolve 它，并且传入和 promise1 一样的值 value

- 2.3.2.3 If/when x is rejected, reject promise with the same reason.

- 2.3.2.3 如果或当 x 状态是 rejected，reject 它，并且传入和 promise1 一样的值 reason

2.3.3 Otherwise, if x is an object or function,

2.3.3 此外，如果 x 是个对象或函数类型

- 2.3.3.1 Let then be x.then. [3.5]

- 2.3.3.1 把 x.then 赋值给 then 变量

- 2.3.3.2 If retrieving the property x.then results in a thrown exception e, reject promise with e as the reason.

- 2.3.3.2 如果捕获（try，catch）到 x.then 抛出的错误的话，需要 reject 这个promise

- 2.3.3.3 If then is a function, call it with x as this, first argument resolvePromise, and second argument rejectPromise, where:

- 2.3.3.3 如果 then 是函数类型，那个用 x 调用它（将 then 的 this 指向 x）,第一个参数传 resolvePromise ，第二个参数传 rejectPromise：

    - 2.3.3.3.1 If/when resolvePromise is called with a value y, run [[Resolve]](promise, y).

    - 2.3.3.3.1 如果或当 resolvePromise 被调用并接受一个参数 y 时，执行 [[Resolve]](promise, y)

    - 2.3.3.3.2 If/when rejectPromise is called with a reason r, reject promise with r.

    - 2.3.3.3.2 如果或当 rejectPromise 被调用并接受一个参数 r 时，执行 reject(r)    

    - 2.3.3.3.3 If both resolvePromise and rejectPromise are called, or multiple calls to the same argument are made, the first call takes precedence, and any further calls are ignored.

    - 2.3.3.3.3 如果 resolvePromise 和 rejectPromise 已经被调用或以相同的参数多次调用的话吗，优先第一次的调用，并且之后的调用全部被忽略（避免多次调用）

    - 2.3.3.3.4 If calling then throws an exception e,
        
    - 2.3.3.4 如果 then 执行过程中抛出了异常，

        - 2.3.3.3.4.1 If resolvePromise or rejectPromise have been called, ignore it.

        - 2.3.3.3.4.1 如果 resolvePromise 或 rejectPromise 已经被调用，那么忽略异常

        - 2.3.3.3.4.2 Otherwise, reject promise with e as the reason.

        - 2.3.3.3.4.2 否则，则 reject 这个异常

- 2.3.3.4 If then is not a function, fulfill promise with x.

- 2.3.3.4 如果 then 不是函数类型，直接 resolve x（resolve(x)）

2.3.4 If x is not an object or function, fulfill promise with x.

2.3.4 如果 x 即不是函数类型也不是对象类型，直接 resolve x（resolve(x)）

If a promise is resolved with a thenable that participates in a circular thenable chain, such that the recursive nature of [[Resolve]](promise, thenable) eventually causes [[Resolve]](promise, thenable) to be called again, following the above algorithm will lead to infinite recursion. Implementations are encouraged, but not required, to detect such recursion and reject promise with an informative TypeError as the reason. [3.6]

/// TODO

### 3.Notes
3.1 Here “platform code” means engine, environment, and promise implementation code. In practice, this requirement ensures that onFulfilled and onRejected execute asynchronously, after the event loop turn in which then is called, and with a fresh stack. This can be implemented with either a “macro-task” mechanism such as setTimeout or setImmediate, or with a “micro-task” mechanism such as MutationObserver or process.nextTick. Since the promise implementation is considered platform code, it may itself contain a task-scheduling queue or “trampoline” in which the handlers are called.

3.2 That is, in strict mode this will be undefined inside of them; in sloppy mode, it will be the global object.


3.2 这个 this 在严格模式下是 undefined，在宽松模式，指向 global 对象

3.3 Implementations may allow promise2 === promise1, provided the implementation meets all requirements. Each implementation should document whether it can produce promise2 === promise1 and under what conditions.

3.4 Generally, it will only be known that x is a true promise if it comes from the current implementation. This clause allows the use of implementation-specific means to adopt the state of known-conformant promises.

3.5 This procedure of first storing a reference to x.then, then testing that reference, and then calling that reference, avoids multiple accesses to the x.then property. Such precautions are important for ensuring consistency in the face of an accessor property, whose value could change between retrievals.

3.6 Implementations should not set arbitrary limits on the depth of thenable chains, and assume that beyond that arbitrary limit the recursion will be infinite. Only true cycles should lead to a TypeError; if an infinite chain of distinct thenables is encountered, recursing forever is the correct behavior.