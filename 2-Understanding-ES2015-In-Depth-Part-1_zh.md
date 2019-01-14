## 深入理解 ES2015，第一趴：块级作用域 `let` 和 `const`

> 原文：http://javascriptissexy.com/understanding-es2015-in-depth-part-1-block-scope-with-let-and-const/  
作者：[Dan Wellman](http://javascriptissexy.com/author/dan_wellman/)

ES2015 最大的特性之一就是有了一个全新的作用域。在这个章节里，我们将开始学习什么是作用域。我们将继续学习如何创建新的作用域类型，以及给我们代码带来的好处

### 快速了解作用域

作用域描述为一个变量，函数，标识符可以被访问的区域。JavaScript 传统上有两种作用域类型：全局作用域和函数作用域，你定义变量的位置会影响其他代码是否可以访问。让我们来看一个简单的例子来阐述作用域的概念。想象一下，你的 JavaScript 文件只包含以下代码：

```js
var globalVariable = 'This is global';

function globalFunction1() {
  var innerVariable1 = 'Non-global variable 1';
}

function globalFunction2() {
  var innerVariable2 = 'Non-global variable 2';
}
```

在上面的代码中，我们首先声明了一个变量 `globalVariable`。这个语句不在函数内部，所以会自动存到全局作用域中。浏览器用 `window` 对象创建了一个全局作用域，除了可以用 `globalVariable` 访问，我们还可以通过挂在 `window` 对象上的 `window.globalVariable` 访问。我们可以在文件的任何地方访问这个变量，这两个函数的之前或之后，甚至是在函数的内部（这就是为什么我们说全局变量是 “隐藏的”，我们可以在任何地方正确的访问他们），甚至是在附在同一页面的其他 JavaScript 文件

在全局作用域里，我们定义了两个函数，`globalFunction1` 和 `globalFunction2`，就像全局变量一样，他们是 “可见的” 并且可以在这个文件的任何地方调用，也可以被同一页面的其他 JavaScript 文件调用。然而，当 JavaScript 引擎解析这些函数时，会分别创建他们自己的作用域。因吹斯听，这两个新的函数作用域被嵌套在全局作用域下，成为子作用域。这也就意味着函数内的代码可以访问全局变量，就像是和在函数 “内部的” 定义变量一样

当我们试图访问 JavaScript 里的标识符时，浏览器会首先在当前作用域中查找。如果没有找到，浏览器会在当前作用域的父作用域中查找，并且继续向上查找，直到找到这个变量，或者到达全局作用域为止。如果这个变量在全局作用域里依旧没有找到的话，那么浏览器会抛出一个 `ReferenceError` 错误。这种嵌套的作用域被称作作用域链，而这个检查当前作用域和父作用域的过程被称作变量查找。这种查找只会向上查找作用域链，它永远不会在它的子作用域里查找 

在上面的作用域链查找方向我们得知，例子中的 `innerVariable1` 变量只能在 `globalFunction1` 函数内部被访问，`innerVariable2` 变量只能在 `globalFunction2` 函数内部被访问。`innerVariable1` 变量不能在 `globalFunction2` 函数内部或全局作用域内被访问，`innerVariable2` 变量也不能在 `globalFunction1` 函数内部或全局作用域内被访问

下面的图片是上面代码中作用域的抽象表示：

![js-scopes](http://javascriptissexy.com/wp-content/uploads/2018/01/chapter9_screenshot_1.png)

> #### 全局作用域包含了 `globalVariable` 以及两个内嵌的函数作用域。每个内嵌的函数作用域又包含自己的变量，但是这些变量不能被全局作用域访问。虚线表示的是作用域链的查找方向

让我们来看下另一个简短的代码示例，彻底的了解下到目前为止我们所介绍到的作用域概念。假设 JavaScript 文件只包含如下代码：

```js
function outer() {
  var variable1;

  function inner() {
    var variable2;
  }
}
```

在这段代码里，我们在全局作用域里声明了一个叫 `outer` 的函数。因为它是一个函数，所以它创建了一个函数作用域，嵌套在全局作用域下。在这个作用域下，我们又声明了一个叫 `variable1` 的变量和 一个叫 `inner` 的函数。因为 `inner` 也是一个函数，所以一个新的作用域又被创建了，嵌套在 `outer` 函数的作用域下

在 `inner` 函数中，我们既可以访问 `variable2` 也可以访问 `variable1`。当我们在 `inner` 函数中访问 `variable1` 时，浏览器首先会在它的作用域里查找这个变量；当这个变量没有被找到时，会继续向上在父作用域里查找（也就是 `outer` 函数的作用域）。代码里作用域如下图所示：

![js-scopes2](http://javascriptissexy.com/wp-content/uploads/2018/01/chapter9_screenshot_2.png)

> #### 函数作用域可以嵌套在其他的函数作用域里，但是作用域链查找规则是一样的，因此在 `inner` 作用域下可以访问到  `variable1` 和 `variable2`，但是在 `outer` 作用域下只能访问 `variable1`

这个示例中的作用域链比较长，从 `inner` 函数延伸到 `outer` 函数，直到全局对象 `window`

### JavaScript 的新作用域

在 JavaScript 中，一个块是由一个或多个语句用大括号包裹起来的。诸如 `if`，`for`，`while` 的条件表达式，都是用块基于特定的条件来执行块语句

其他流行的常见的编程语言都有块作用域，JavaScript 作用域中，直到如今却只有全局作用域和函数作用域，因此使我们变得很困惑。ES2015 在 JavaScript 新增了块作用域，对于我们的代码来说有很大的影响，并且对于那些熟悉其他编程语言的开发者来说变得更直观

块作用域意味着一个块可以创建它自己的作用域，而不是简单的存在于它最近到父级函数作用域或全局作用域下。让我们在认识块作用域是如何工作的之前，先来了解下传统上块里的 JavaScript 是如何工作的：

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

`var` 语句是不能够创建块作用域的，即使是在块里，因此 `console.log` 语句可以访问到 `x` 和 `y` 变量。 `fn` 函数创建了一个函数作用域而且 `x` 和 `y` 变量都是可以通过作用域内的作用域链访问到 

### 声明提升

理解提升的概念是理解 JavaScript 如何工作的基础。JavaScript 有两个阶段：解析阶段（JavaScript 引擎读取所有的代码）、执行阶段（执行已解析的代码）。大多数的事情都发生在第二阶段；例如，当你使用 `console.log` 语句时，实际的日志消息会在执行阶段打印到控制台

然而，一些重要的事情也会在解析阶段发生，包括变量的内存分配、作用域创建。提升这个术语指的是 JavaScript 引擎在遇到标识符，如变量、函数声明时所发生到事情；当发生声明提升时，它的行为就像是把它定义的字面量提升到当前作用域的顶部。鉴于此，上面到代码示例实际会变成如下情况：

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

只有变量到声明会提升到它的作用域的顶部；在这个例子的 `if` 语句中，变量赋值依然发生在我们所赋值的地方。当然，我们到变量并不会移动，而是引擎行为的确如此，因此这样可以更好的帮助我们理解代码

除了变量，函数声明也会被提升。结果就是，从 JavaScript 引擎到角度来看，代码实际上看起来是这样的：

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

`innerFn` 的声明也被提升到了它的作用域的顶部。但是，记住它仅仅是函数声明被提升了，函数调用没有被提升。上面的代码并不会报任何错，因为 `innerFn` 在 `x` 和 `y` 赋值之前并没有被调用   

### 使用 `let`

即使使用了 ES2015，`var` 语句也不会创建块作用域。为了创建块作用域，我们需要在块里使用 `let` 或 `const` 语句。我们一会再看 `const`，首先来看下 `let`

表面上，`let` 和 `var`（我们用它来声明变量）的行为很相似：

```js
function fn() {
  var variable1;
  let variable2;
}
```

在这个简单的例子中，`var` 和 `let` 语句都做了相同的事情（在 `fn` 创建的作用域下初始化了一个新的变量）。为了创建一个新的块作用域，我们需要在块里使用 `let`：

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

在这个代码示例中，抛出了一个引用错误（reference error）；让我们来探索下为什么会这样。`fn` 函数创建了一个新作用域，里面声明了变量 `variable1`。然后我们在 `if` 语句的块里，声明了变量 `variable2`。然而，因为我们在块里使用了 `let` 语句，因此一个新的块作用域在 `fn` 的作用域下被创建了

如果 `console.log` 语句也在 `if` 块中的话，那么它就和 `variable2` 在相同的作用域下了，也能够通过作用域链找到 `variable1`。但是因为 `console.log` 在外头，因此它不能访问 `variable2`，所以会抛出一个引用错误

块作用域和函数作用域的行为相同，但是他们是为块创建的，而不是函数

### 暂时性死区

当一个用 `var` 声明的常规变量被创建时，会被提升到它的作用域的顶部，然后并初始化一个 `undefined` 值，这样就允许我们能够在它赋值之前引用一个正常的变量

```js
console.log(x); // undefined
var x = 10;
```

记住，由于存在声明提升，代码实际看起来是这样的：

```js
var x = undefined;
console.log(x); // undefined
x = 10;
```

这个行为会阻止抛出引用错误 `ReferenceError`

用 `let` 声明的变量也被提升了，但重要的是，他们并不会自动初始化值 `undefined`，因此意味着下面的代码会产生一个错误：

```js
console.log(x); // Uncaught ReferenceError: x is not defined
let x = 10;
```

这个错误是由暂时性死区（TDZ）引起的。TDZ 存在于作用域初始化到变量声明期间。为了修复这个错误（`ReferenceError`），我们需要在访问它前声明它：

> 译者注：[TDZ](https://gist.github.com/rwaldron/ca35924d59ddc60a6aa165e1e4a3acda)

```js
let x;
console.log(x); // undefined
x = 10;
```

TDZ 这样设计是为了使开发更容易（试图引用一个还没声明的变量通常视为一个错误，而不是故意的决策），因此这个错误可以立即提醒我们

### 使用 `const`

The new `const` statement is used to declare a variable whose value cannot be reassigned. It behaves in a very similar way as `let` does with regard to the TDZ, but when being declared, a `const` variable must be initialised with a value:

```js
const VAR1 = 'constant';
```

From this point on, the value of `VAR1` will always be the string `constant`. If we try to change the value of the variable through reassignment, we’ll see an error:

> TypeError: Assignment to `constant` variable

If we try to create a `const` variable without initializing it with a value, we’ll also see an error; this time a SyntaxError:

> SyntaxError: Missing initializer in `const` declaration

Simirlarly, a `const` variable cannot be redeclared. If we try to declare the same `const` variable more than once, we’ll see a different type of SyntaxError:

> SyntaxError: Identifier ‘VAR1′ has already been declared

As with other programming languages, constants are useful for holding values that we do not expect to change over the life of our program.

It is important to note that `let` and `const` are both reserved words in JavaScript, and so cannot be used as identifier names in strict mode. As ES2015 becomes more and more common, a consensus is emerging that both `let` and `const` are superior to `var` because the scope of variables created with them is more aligned to other modern programming languages, and code behaves in a much more predictable way. Therefore, for most situations it is preferable to avoid the use of `var` if possible.

### 不可变性

用 `const` 声明的变量不能被再次赋值，但是 `const` 声明的变量并不是完全不可变的。如果我们用对象或数组初始化了一个 `const` 变量，我们依然可以修改对象到属性和增加删除数组到元素 

### 练习

1. 在 `for` 循环里用 `let` 来初始化计数器变量  
2. 修复下面 `const` 的错误：

```js
const VAR1 = 'constant';
const VAR1 = 'constant2';
const VAR2;
VAR2 = 'constant';
```

> #### 成功是通过不断的练习和知识的积累，而非智力

