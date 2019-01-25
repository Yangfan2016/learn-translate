## Understanding ES2015 In Depth, Part 1: Block Scope with `let` and `const`

> - 原文地址：http://javascriptissexy.com/understanding-es2015-in-depth-part-1-block-scope-with-let-and-const/
> - 原文作者：[Dan Wellman](http://javascriptissexy.com/author/dan_wellman/)
> - Markdown 地址：https://github.com/Yangfan2016/learn-translate/blob/master/2-Understanding-ES2015-In-Depth-Part-1.md
> - 译者：[Yangfan2016](https://github.com/Yangfan2016)

One of the major features introduced by ES2015 is a whole new scope. In this section, we’re going to start by learning what a scope is. We’ll then move on to look at how we can create the new type of scope, and the benefits it can bring to our code.

### A Quick Introduction to Scope

The term scope describes an area in which variables and functions, or identifiers, can be accessed. JavaScript has traditionally had two types of scope: global scope and function scope, and the place in your code in which a variable is declared affects whether it can be accessed by other parts of your code. Let’s look at an example with some code to illustrate the concept of scope. Imagine that you have a JavaScript file containing only the following code:


```js
var globalVariable = 'This is global';

function globalFunction1() {
  var innerVariable1 = 'Non-global variable 1';
}

function globalFunction2() {
  var innerVariable2 = 'Non-global variable 2';
}
```

In the above code we first declare `globalVariable`. This statement is not inside a function so this variable will automatically be stored in the global scope. The browser creates the global scope, using the `window` object, so as well as accessing the variable using the identifier `globalVariable`, we could also access it through the `window` object using `window.globalVariable`. We can access this variable anywhere in the file, before or after the two functions, and even inside them, which is why we say that global variables are “visible” to all of our code we can literally access them from anywhere, even in other JavaScript files attached to the same page.

Following the global variable we declare two functions, `globalFunction1` and `globalFunction2`, like the global variable, these function can be “seen” and invoked by code anywhere else in this file, or in other files loaded by the same page. However, when the JavaScript engine parses these functions, it will create two new function scopes, one for each of the functions. This is where things get interesting; scopes in JavaScript are nested so the two new function scopes become child scopes of the global scope. This means that the code inside each function can access the global globalVariable variable, as if it had been declared inside the function alongside the `inner` variables.

When trying to access an identifier in JavaScript, the browser will first look for the variable inside the current scope. If it is not found, the browser will then look in the parent scope of the current scope, and will keep moving up through the parent scopes until it either finds the variable, or reaches the global scope. If the variable still isn’t found in the global scope, the browser will generate a `ReferenceError`. The nested scopes are known as a scope chain, and this process of checking the current scope and then the parent scopes is known as a variable look-up. This look-up is only able to go up the scope chain, it will never look inside child scopes of the current scope.

What the direction of the look-up through the scope chain means for the above example is that `innerVariable1` can only be accessed inside the `globalFunction1` function, and `innerVariable2` can only be accessed inside the `globalFunction2` function. `innerVariable1` cannot be accessed within the `globalFunction2` function, or by the global scope, and `innerVariable2` cannot be accessed by `globalFunction1` or the global scope.

The following image shows an abstract representation of the scopes in the above code:

![js-scopes](http://javascriptissexy.com/wp-content/uploads/2018/01/chapter9_screenshot_1.png)

> #### The global scope contains the `globalVariable` as well as the two nested function scopes. Each nested function scope contains its own variable, but these variables are not accessible to the global scope. The dotted lines represent the direction of the look-up through the scope chain.

Let’s look at another brief code example to hammer home the scope concepts that we’ve covered so far. Consider a JavaScript file which contains only the following code:

```js
function outer() {
  var variable1;

  function inner() {
    var variable2;
  }
}
```

In this code, we have an `outer` function named `outer`, which is defined in the global scope. As it’s a function, it creates a function scope which is nested within the global scope. Inside this scope we declare the variable `variable1` and a new function called `inner`. As `inner` is also a function, a new scope is created, and nested within the `outer` function’s scope.

Inside the `inner` function, we can access both variable2 which is in the `inner` function’s scope and `variable1`. When we access `variable1` from inside the `inner` function, the browser will first look for the variable in its current scope; when the variable is not found, the look-up will navigate up to the parent scope, which is the `outer` function’s scope. The scopes in this code could be represented like this:

![js-scopes2](http://javascriptissexy.com/wp-content/uploads/2018/01/chapter9_screenshot_2.png)

> #### Function scopes may be nested within other function scopes, but the same rules around the scope-chain look-up apply, so the `inner` scope can access both `variable1` and `variable2`, but the `outer` scope can only access `variable1`.

The scope chain is longer in this example, stretching from the `inner` function, through the `outer` function, and up to the global window object.

### JavaScript’s New Scope

In JavaScript, a block is one or more statements within curly brackets. Conditional expressions, such as `if`, `for`, and `while` statements, all use blocks to execute statements based on certain conditions.

Other popular and common programming languages have block scope, so scope in JavaScript, which until now has only had global and function scope, has always been considered confusing. The ES2015 addition of block scope to JavaScript has important implications for our code and can also make the language more intuitive to developers familiar with other programming languages.

Block scope means that a block is able to create its own scope, rather than simply existing within the scope created by its nearest parent function, or the global scope. Let’s take a quick look at how scope has traditionally worked with blocks in JavaScript before we move on to look at how block scope now works:

```js
function fn() {
  var x = 'function scope';

  if (true) {
    var y = 'not block scope';
  }

  function innerFn() {
    console.log(x, y); // function scope not block scope
  }
  innerFn();
}
```

The `var` statement is not able to create a block scope, even when used within a block, so the `console.log` statement is able to access both the `x` and `y` variables. The `fn` function creates a function scope and both the `x` and `y` variables are accessible via the scope chain within that scope.

### Hoisting

Understanding the concept of hoisting is fundamental to understanding how JavaScript works. JavaScript has two phases: a parsing phase—where all of the code is read by the JavaScript engine—followed by an execution phase in which the code that has been parsed is executed. It is during this second phase that most things happen; for example, when you use a `console.log` statement, the actual log message is printed to the console during the execution phase.

However, some important things happen during the parsing phase as well, including memory allocation for variables and scope creation. The term hoisting describes what happens when the JavaScript engine encounters an identifier, such as a variable or function declaration; when it does this, it acts as if it literally lifts (hoists) that declaration up to the top of the current scope. In light of this, in the above code example, what really happens is this:

```js
function fn() {
  var x;
  var y;

  x = 'function scope';

  if (true) {
    y = 'not block scope';
  }

  function innerFn() {
    console.log(x, y); // function scope not block scope
  }
  innerFn();
}
```

Only the variable declaration is hoisted to the top of its scope; the variable assignment still occurs at the place where we assigned the value, inside the `if` statement in this example. Of course, our variables aren’t literally moved around in our code, but the engine behaves as if this is what happens, so this is a useful device for understanding our code better.

In addition to variables, function declarations are also hoisted. Consequently, from the JavaScript engine’s perspective, the code actually looks like this:

```js
function fn() {
  var x;
  var y;
  function innerFn() {
    console.log(x, y); // function scope not block scope
  }

  x = 'function scope';

  if (true) {
    y = 'not block scope';
  }
  innerFn();
}
```

The declaration of `innerFn` is also moved to the top of its scope. But remember, it is just the declaration of the function that is hoisted, not the invocation of the function. The above code won’t throw any errors because `innerFn` isn’t invoked until after the `x` and `y` variables have had values assigned to them.

### Using `let`

Even when using ES2015, the `var` statement does not create block scope. In order to create block scope, we need to use either the `let` or `const` statements inside a block. We’ll come back to `const` shortly. For now, let’s focus on `let`.

Superficially, `let` is very similar to `var`—we use it to declare variables:

```js
function fn() {
  var variable1;
  let variable2;
}
```

In this simple example, the `var` and `let` statements both do the same thing—they initialise a new variable in the current scope, which is the scope created by the `fn` function. In order to create a new block scope, we need to use `let` inside a block:

```js
function fn() {
  var variable1 = 'function scope';

  if (true) {
    let variable2 = 'block scope';
  }

  console.log(variable1, variable2); // Uncaught ReferenceError: variable2 is not defined
}
fn();
```

In this case the code throws a reference error; let’s explore why. The `fn` function creates a new scope within which `variable1` is declared. We then have an `if` statement, which uses a block to declare `variable2`. However, because we used the `let` statement within that block, a new block scope is created within the `fn` scope.

If the `console.log` statement had been inside the `if` block as well, it would be in the same scope as `variable2` and would be able to use the scope chain to find `variable1`. But because `console.log` is in the `outer` `fn` scope, it can’t access `variable2`, so it throws a reference error.

Block scopes work the same as function scopes work, but they are created for blocks, rather than functions.

### The Temporal Dead Zone

When a regular variable created using `var` is hoisted to the top of its scope, it’s initialized with the value `undefined`, which is what allows us to be able to reference a normal variable before it has a value declared through assignment:

```js
console.log(x); // undefined
var x = 10;
```

Remember, because of hoisting, the code is actually understood as this:

```js
var x = undefined;
console.log(x); // undefined
x = 10;
```

This behavior prevents a `ReferenceError` from being thrown.

Variables declared with `let` are hoisted, but crucially, they are not automatically initialised with the value `undefined`, which means that the following code produces an error:

```js
console.log(x); // Uncaught ReferenceError: x is not defined
let x = 10;
```

This error is caused by the temporal dead zone (TDZ). The TDZ exists from the moment the scope is initialized to the moment the variable is declared. To fix the `ReferenceError`, we need to declare the variable before trying to access it:

```js
let x;
console.log(x); // undefined
x = 10;
```

The TDZ was designed like this in order to make development easier—trying to reference a variable that has not been declared yet is more commonly an error than an intentional decision, so the error highlights this to us immediately.

### Using `const`

The new `const` statement is used to declare a variable whose value cannot be reassigned. It behaves in a very similar way as `let` does with regard to the TDZ, but when being declared, a `const` variable must be initialised with a value:

```js
const VAR1 = 'constant';
```

From this point on, the value of `VAR1` will always be the string `constant`. If we try to change the value of the variable through reassignment, we’ll see an error:

> TypeError: Assignment to `constant` variable

If we try to create a `const` variable without initializing it with a value, we’ll also see an error; this time a SyntaxError:

> SyntaxError: Missing initializer in `const` declaration

Similarly, a `const` variable cannot be redeclared. If we try to declare the same `const` variable more than once, we’ll see a different type of SyntaxError:

> SyntaxError: Identifier ‘VAR1′ has already been declared

As with other programming languages, constants are useful for holding values that we do not expect to change over the life of our program.

It is important to note that `let` and `const` are both reserved words in JavaScript, and so cannot be used as identifier names in strict mode. As ES2015 becomes more and more common, a consensus is emerging that both `let` and `const` are superior to `var` because the scope of variables created with them is more aligned to other modern programming languages, and code behaves in a much more predictable way. Therefore, for most situations it is preferable to avoid the use of `var` if possible.

### Immutability

While the value of a `const` variable cannot be changed with reassignment, `const` variables are not completely immutable. If we initialize a `const` variable with an object or an array, we will still be able to set the properties of the object and add and remove items to the array.

### Exercises

1. Use `let` to initialize the counter variable for a for loop.  
2. Fix the following `const` errors:

```js
const VAR1 = 'constant';
const VAR1 = 'constant2';
const VAR2;
VAR2 = 'constant';
```

> #### success emerges through knowledge and dedicated practices,not by intelligence

