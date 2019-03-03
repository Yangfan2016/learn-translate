<h1 align="center">
  面试 30 秒
</h1>

<h4 align="center">一个面试常用的问题精选集，帮助你准备下一次面试</h4>

> 原文 https://github.com/30-seconds/30-seconds-of-interviews

## 前言

面试是令人生畏的，它甚至可以让经验丰富的专家在压力之下大脑一片空白。复习和学习哪些在面试中常遇到的问题（从社区中收集了被问到的和他们是如何应对的问题）。通过把实践和现实生活结合起来，你就可以从容的准备面对下一次面试


## [在线观看](https://30secondsofinterviews.org/)


## 目录


### JavaScript

<details>
<summary>查看内容</summary>

* [创建一个 batches 函数，返回一个食谱中可以被作为烹饪整批食材的最大数量](#创建一个-batches-函数返回一个食谱中可以被作为烹饪整批食材的最大数量)
* [什么是大 O 标记法？](#what-is-big-o-notation)
* [创建一个和 `Function.prototype.bind` 功能一样的独立函数 `bind`](#创建一个和-Functionprototypebind-功能一样的独立函数-bind)
* [你是怎么避免回调地狱的？](#how-can-you-avoid-callback-hells)
* [什么是回调，你可以举个例子吗？](#什么是回调你可以举个例子吗)
* [在 JavaScript 中，你是如何克隆一个对象的？](#how-do-you-clone-an-object-in-javascript)
* [什么是闭包，你可以举一个有用的例子吗？](#什么是闭包你可以举一个有用的例子吗)
* [在 JavaScript 中，你是如何比较两个对象的？](#how-do-you-compare-two-objects-in-javascript)
* [什么是 `CORS`？](#what-is-cors)
* [什么是 `DOM`？](#what-is-the-dom)
* [`==` 和 `===` 相等运算符有什么区别？](#-和--相等运算符有什么区别)
* [什么是事件委托，为什么它是有用的，你可以举个例子说明如何使用它？](#what-is-event-delegation-and-why-is-it-useful-can-you-show-an-example-of-how-to-use-it)
* [什么是事件驱动编程？](#what-is-event-driven-programming)
* [在 JavaScript 中，声明和表达式的区别？](#what-is-the-difference-between-an-expression-and-a-statement-in-javascript)
* [在 JavaScript 中，什么是真值（truthy），假值（falsy）?](#在-javascript-中什么是真值truthy假值falsy)
* [生成一个包含的 n 项斐波那契数列元素的数组](#生成一个包含的-n-项斐波那契数列元素的数组)
* [`0.1 + 0.2 === 0.3` 表达式的值是？](#01--02--03-表达式的值是)
* [数组 `map()` 和 `forEach()` 方法的区别？](#数组-map-和-foreach-方法的区别)
* [什么是函数式编程？](#什么是函数式编程)
* [下面的例子中，`console.log` 会打印出什么？](#下面的例子中consolelog-会打印出什么)
* [在 JavaScript 中，声明提升是如何工作的？](#在-javascript-中声明提升是如何工作的)
* [为何将 JavaScript 源文件里的整个内容用匿名函数包裹起来？](#为何将-javascript-源文件里的整个内容用匿名函数包裹起来)
* [阐释下命令式编程和声明式编程的区别？](#explain-the-differences-between-imperative-and-declarative-programming)
* [词法作用域和动态作用域的区别？](#词法作用域和动态作用域的区别)
* [创建一个函数，用 ‘#’ 符号遮住字符串（除最后4个字符之外）](#创建一个函数用--符号遮住字符串除最后4个字符之外)
* [什么是缓存代理模式（memoization）？](#什么是缓存代理模式memoization)
* [什么是 MIME 类型，有什么作用？](#什么是-mime-类型有什么作用)
* [对比下可变与不可变值，可变与不可变方法](#contrast-mutable-and-immutable-values-and-mutating-vs-non-mutating-methods)
* [在 JavaScript 中，哪个值不等于它自己？](#在-javascript-中哪个值不等于它自己)
* [`null`  和 `undefined` 有何不同？](#null--和-undefined-有何不同)
* [描述下创建对象方式的不同，哪种方式更推荐？](#描述下创建对象方式的不同哪种方式更推荐)
* [形参和实参的区别？](#what-is-the-difference-between-a-parameter-and-an-argument)
* [JavaScript 里是通过值传递还是引用传递？](#javascript-里是通过值传递还是引用传递)
* [创建一个管道函数，返回一个接受一个参数从左到右执行的合成函数](#创建一个管道函数返回一个接受一个参数从左到右执行的合成函数)
* [`i++`  和 `++i` 有什么不同？](#i--和-i-有什么不同)
* [Promise 可以变成哪些状态？](#promise-可以变成哪些状态)
* [什么是 Promises？](#what-are-promises)
* [原型继承和经典继承方式有何不同？](#how-does-prototypal-inheritance-differ-from-classical-inheritance)
* [什么是纯函数？](#什么是纯函数)
* [什么是递归，什么时候它是有用的？](#what-is-recursion-and-when-is-it-useful)
* [下面的代码会输出什么？](#下面的代码会输出什么)
* [下面的函数会返回什么？](#下面的函数会返回什么)
* [JavaScript 里分号是必须的吗？](#javascript-里分号是必须的吗)
* [在 JavaScript 里，什么是短路运算？](#what-is-short-circuit-evaluation-in-javascript)
* [解释下静态方法和实例方法的区别](#解释下静态方法和实例方法的区别)
* [在 JavaScript 里，同步代码和异步代码有什么不同？](#在-javascript-里同步代码和异步代码有什么不同)
* [`this` 关键字是什么，它是如何工作的？](#what-is-the-this-keyword-and-how-does-it-work)
* [下面的代码执行的结果是什么？](#下面的代码执行的结果是什么)
* [什么是 JavaScript 的数据类型？](#什么是-javascript-的数据类型)
* [诸如 React，Vue，Angular，Hyperapp 等 JavaScript UI 库/框架的目的是什么？](#what-is-the-purpose-of-javascript-ui-librariesframeworks-like-react-vue-angular-hyperapp-etc)
* [什么是‘严格模式’，它带来哪些关键性的好处？](#什么是严格模式它带来哪些关键性的好处)
* [`let` `var` `const` 和无关键字声明变量有何不同？](#what-are-the-differences-between-var-let-const-and-no-keyword-statements)
* [什么是虚拟 DOM，为何库/框架都在用它？](#what-is-a-virtual-dom-and-why-is-it-used-in-librariesframeworks)
* [什么是跨站脚本攻击（XSS），你是如何阻止它的？](#what-is-a-cross-site-scripting-attack-xss-and-how-do-you-prevent-it)
</details>


### React

<details>
<summary>查看内容</summary>

* [`setState` 将回调函数作为参数目的是什么？](#setstate-将回调函数作为参数目的是什么)
* [回调引用 refs 和 findDOMMNode 哪个更推荐使用？](#which-is-the-preferred-option-between-callback-refs-and-finddomnode)
* [React 组件中的属性（prop）`children` 是什么？](#react-组件中的属性propchildren-是什么)
* [React 为什么用 `className` 属性代替 `class`?](#react-为什么用-classname-属性代替-class)
* [在 React 中，什么是 `context`？](#what-is-context)
* [Element 和 Component 有什么区别？](#element-和-component-有什么区别)
* [在 React 中，错误边界是什么？](#在-react-中错误边界是什么)
* [在 React 中，什么是 `fragments`？](#在-react-中什么是-fragments)
* [什么是高阶组件？](#什么是高阶组件)
* [React 和 HTML 对事件处理的区别？](#react-和-html-对事件处理的区别)
* [什么是内联条件表达式？](#什么是内联条件表达式)
* [什么是 key ，在 lists 中使用的好处是什么？](#what-is-a-key-what-are-the-benefits-of-using-it-in-lists)
* [React 里的生命周期有哪些？](#what-are-the-lifecycle-methods-in-react)
* [React 组件中，生命周期的各个阶段是什么？](#react-组件中生命周期的各个阶段是什么)
* [在 React 中，状态提升是什么意思？](#what-does-lifting-state-up-in-react-mean)
* [在 React class 组件中，你是如何确保 `this` 的正确指向的？](#how-do-you-ensure-methods-have-the-correct-this-context-in-react-component-classes)
* [你是怎么给事件处理或回调函数传参的？](#你是怎么给事件处理回调函数传参的)
* [在 React 中，`portals` 是什么？](#what-are-portals-in-reactjs)
* [在 React 中，如何校验 `prop`？](#how-to-apply-prop-validation-in-react)
* [在 React 里，如何写注释？](#在-react-里如何写注释)
* [什么是 `refs`，我们如何使用它？](#what-are-refs-when-should-they-be-used)
* [什么是有状态组件？](#什么是有状态组件)
* [什么是无状态组件？](#什么是无状态组件)
</details>


### HTML

<details>
<summary>查看内容</summary>

* [图片里的 `alt` 属性是做什么的？](#图片里的-alt-属性是做什么的)
* [`<script>` 标签的 `defer` 和 `async` 是什么？](#what-are-defer-and-async-attributes-on-a-script-tag)
* [不采用缓存的目的是什么，你如何实现它？](#what-is-the-purpose-of-cache-busting-and-how-can-you-achieve-it)
* [什么是 `DOM`？](#what-is-the-dom)
* [一个页面里是否可以包含多个 `<header>` 元素， `<footer>` 元素呢？](#can-a-web-page-contain-multiple-header-elements-what-about-footer-elements)
* [讨论下 HTML 规范和浏览器实现之间的区别？](#discuss-the-differences-between-an-html-specification-and-a-browsers-implementation-thereof)
* [相比 HTML，XHTML 有哪些不同？](#相比-htmlxhtml-有哪些不同)
* [简明的阐述下 HTML5 语义标签 `<header>`，`<article>`，`<section>`，`<footer>` 的用法](#briefly-describe-the-correct-usage-of-the-following-html5-semantic-elements-header-articlesection-footer)
* [什么是 HTML5 Web Storage，解释下 `localStorage` 和 `sessionStorage`？](#什么是-html5-web-storage解释下-localstorage-和-sessionstorage)
* [什么时候和为什么使用 `rel="noopener"` 属性？](#where-and-why-is-the-relnoopener-attribute-used)
</details>


### CSS

<details>
<summary>查看内容</summary>

* [什么是 CSS BEM？](#what-is-css-bem)
* [简要阐述下 CSS 的盒模型，及各个组成部分？](#简要阐述下-css-的盒模型及各个组成部分)
* [用 CSS 预处理的优势是什么？](#what-are-the-advantages-of-using-css-preprocessors)
* [CSS 里通用兄弟选择器和相邻兄弟选择器的区别？](#what-is-the-difference-between--and--sibling-selectors)
* [你能描述下 CSS 优先级是如何工作的？](#can-you-describe-how-css-specificity-works)
* [`em` 和 `rem` 单位的区别？](#what-is-the-difference-between-em-and-rem-units)
* [使用 flexbox，创建一个 3 列布局，每一列取容器的百分之 `col-{n}`/12 ](#使用-flexbox创建一个-3-列布局每一列取容器的百分之-col-n12)
* [什么是聚焦环，正确的解决方案是什么？](#what-is-a-focus-ring-what-is-the-correct-solution-to-handle-them)
* [你能说出 `@media` 属性的四种类型吗？](#你能说出-media-属性的四种类型吗)
* [CSS 雪碧图的优势在哪里，如何使用？](#what-are-the-advantages-of-using-css-sprites-and-how-are-they-utilized)
</details>


### Node

<details>
<summary>查看内容</summary>

* [你如何避免回调地狱？](#how-can-you-avoid-callback-hells)
* [Node.js 中，经常使用回调的模式，把执行过程中遇到的错误，作为回调函数的第一个参数，这么做的优势是什么？](#nodejs-often-uses-a-callback-pattern-where-if-an-error-is-encountered-during-execution-this-error-is-passed-as-the-first-argument-to-the-callback-what-are-the-advantages-of-this-pattern)
* [NodeJS 错误优先回调的模式有什么优势？](#nodejs-错误优先回调的模式有什么优势)
* [什么是 Nodejs 里的事件循环（event loop）？](#什么是-nodejs-里的事件循环event-loop)
* [什么是 `REST`？](#what-is-rest)
</details>


### 安全

<details>
<summary>查看内容</summary>

* [什么是 XSS 攻击，你如何预防它？](#what-is-a-cross-site-scripting-attack-xss-and-how-do-you-prevent-it)
</details>


---

## JavaScript
### `==` 和 `===` 相等运算符有什么区别？

<details>
<summary>查看答案</summary>


三等号（`===`）检查严格相等，也就意味着类型和值必须相同。另一方面，双等号（`==`）首先类型强制转换，以致于类型相同，然后在使用严格比较

#### 小贴士


* 只要可能，就使用三等号比较相等，因为宽松的比较符双等号可能会得到不直观的结果
* 强制类型转换意味着值会被转换成同一类型
* 讨论假值及他们的比较

##### 附加链接


* [MDN docs for comparison operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators)

</details>

<br>[⬆ 返回顶部](#目录)

### `i++`  和 `++i` 有什么不同？

<details>
<summary>查看答案</summary>

两种方式都会使得变量的值增加 1。它们计算的差别：

后缀递增操作符计算的值是在它的值增加之前

```js
let i = 0
i++ // 0
// i === 1
```

前缀递增操作符计算的值是在它的值增加之后

```js
let i = 0
++i // 1
// i === 1
```


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### Promise 可以变成哪些状态？

<details>
<summary>查看答案</summary>

`Promise` 的状态只可能是下面的其中之一：

* pending: 初始状态，不是完成态（fulfilled）也不是拒绝态（rejected）
* fulfilled: 意味着操作已经完成
* rejected: 意味着操作已经失败

一个处于 `pending` 态的 `promise` 是不可能转换成完成态（fulfilled）或拒绝态（rejected）的。
当这些状态发生的时候，会调用 `promise` 的 `then` 方法处理队列里的相关处理程序


#### 小贴士




##### 附加链接


* [Official Web Docs Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

</details>

<br>[⬆ 返回顶部](#目录)

### 创建一个 batches 函数，返回一个食谱中可以被作为烹饪整批食材的最大数量

```js
/**
它接受两个对象参数：第一个是食谱，第二个是可用食材。每个食材的值是一个数字代表有多少单位
`batches(recipe, available)`
*/

// 0 批食材可用
batches(
  { milk: 100, butter: 50, flour: 5 },
  { milk: 132, butter: 48, flour: 51 }
)
batches(
  { milk: 100, flour: 4, sugar: 10, butter: 5 },
  { milk: 1288, flour: 9, sugar: 95 }
)

// 1 批食材可用
batches(
  { milk: 100, butter: 50, cheese: 10 },
  { milk: 198, butter: 52, cheese: 10 }
)

// 2 批食材可用
batches(
  { milk: 2, sugar: 40, butter: 20 },
  { milk: 5, sugar: 120, butter: 500 }
)
```

<details>
<summary>查看答案</summary>

我们必须有所有足够可用的食材，数量大于或等于所需的单位数量。如果其中一种食材数量不够，那么就构不成一批

使用 `Object.keys()` 返回一个食谱数组，然后使用 `Array.prototype.map()` 来映射每一个食材占食谱的比例。如果其中所需的食材之一数量不够，那么比例将会计算得到 `NaN`，因此在这个例子中，我们可以使用逻辑或操作符来作为后备处理（ratio || 0）

使用扩展操作符（`...`）分配食材比例数组给 `Math.min()` 函数，来决定最小比例。通过对整个结果使用 `Math.floor()` 向下取整得到整批食材的最大数

```js
const batches = (recipe, available) =>
  Math.floor(
    Math.min(...Object.keys(recipe).map(k => available[k] / recipe[k] || 0))
  )
```


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 创建一个和 `Function.prototype.bind` 功能一样的独立函数 bind

```js
function example() {
  console.log(this)
}
const boundExample = bind(example, { a: true })
boundExample.call({ b: true }) // logs { a: true }
```

<details>
<summary>查看答案</summary>

返回一个接受任意数量参数，通过 `...` rest 操作符收集参数的函数。 在这个函数中，返回一个由 `Function.prototype.apply` 调用，context 作为上下文，args 作为参数数组的函数 fn

```js
const bind = (fn, context) => (...args) => fn.apply(context, args)
```


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 什么是回调，你可以举个例子吗？

<details>
<summary>查看答案</summary>

回调函数是作为一个参数传递给另一个函数的函数，只有在事件触发或具体任务完成时调用，经常用在异步代码中。回调函数会在一段代码之后调用，但可以在初始化声明，而不需要调用

例如，事件监听是异步回调，它们只有在特定事件触发后才会执行

```js
function onClick() {
  console.log("The user clicked on the page.")
}
document.addEventListener("click", onClick)
```

然而，回调函数也可以是同步的。下面的 `map` 函数接受一个回调函数，在数组循环每次迭代（数组元素）中同步调用

```js
const map = (arr, callback) => {
  const result = []
  for (let i = 0; i < arr.length; i++) {
    result.push(callback(arr[i], i))
  }
  return result
}
map([1, 2, 3, 4, 5], n => n * 2) // [2, 4, 6, 8, 10]
```


#### 小贴士


* 在 JavaScript 中，函数是一等公民
* 回调 VS Promises


##### 附加链接


* [MDN docs for callbacks](https://developer.mozilla.org/en-US/docs/Glossary/Callback_function)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 中，你是如何克隆一个对象的？

<details>
<summary>查看答案</summary>

Using the object spread operator `...`, the object's own enumerable properties can be copied
into the new object. This creates a shallow clone of the object.

```js
const obj = { a: 1, b: 2 }
const shallowClone = { ...obj }
```

With this technique, prototypes are ignored. In addition, nested objects are not cloned, but rather their references get copied, so nested objects still refer to the same objects as the original. Deep-cloning is much more complex in order to effectively clone any type of object (Date, RegExp, Function, Set, etc) that may be nested within the object.

Other alternatives include:

* `JSON.parse(JSON.stringify(obj))` can be used to deep-clone a simple object, but it is CPU-intensive and only accepts valid JSON (therefore it strips functions and does not allow circular references).
* `Object.assign({}, obj)` is another alternative.
* `Object.keys(obj).reduce((acc, key) => (acc[key] = obj[key], acc), {})` is another more verbose alternative that shows the concept in greater depth.


#### 小贴士


* JavaScript passes objects by reference, meaning that nested objects get their references copied, instead of their values.
* The same method can be used to merge two objects.


##### 附加链接


* [MDN docs for Object.assign()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)
* [Clone an object in vanilla JS](http://voidcanvas.com/clone-an-object-in-vanilla-js-in-depth/)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 中，你是如何比较两个对象的？

<details>
<summary>查看答案</summary>

Even though two different objects can have the same properties with equal values, they are not considered equal when compared using `==` or `===`. This is because they are being compared by their reference (location in memory), unlike primitive values which are compared by value.

In order to test if two objects are equal in structure, a helper function is required. It will
iterate through the own properties of each object to test if they have the same values, including nested objects.
Optionally, the prototypes of the objects may also be tested for equivalence by passing `true` as the 3rd argument.

Note: this technique does not attempt to test equivalence of data structures other than
plain objects, arrays, functions, dates and primitive values.

```js
function isDeepEqual(obj1, obj2, testPrototypes = false) {
  if (obj1 === obj2) {
    return true
  }

  if (typeof obj1 === "function" && typeof obj2 === "function") {
    return obj1.toString() === obj2.toString()
  }

  if (obj1 instanceof Date && obj2 instanceof Date) {
    return obj1.getTime() === obj2.getTime()
  }

  if (
    Object.prototype.toString.call(obj1) !==
      Object.prototype.toString.call(obj2) ||
    typeof obj1 !== "object"
  ) {
    return false
  }

  const prototypesAreEqual = testPrototypes
    ? isDeepEqual(
        Object.getPrototypeOf(obj1),
        Object.getPrototypeOf(obj2),
        true
      )
    : true

  const obj1Props = Object.getOwnPropertyNames(obj1)
  const obj2Props = Object.getOwnPropertyNames(obj2)

  return (
    obj1Props.length === obj2Props.length &&
    prototypesAreEqual &&
    obj1Props.every(prop => isDeepEqual(obj1[prop], obj2[prop]))
  )
}
```


#### 小贴士


* Primitives like strings and numbers are compared by their value
* Objects on the other hand are compared by their reference (location in memory)


##### 附加链接


* [Object Equality in JavaScript](http://adripofjavascript.com/blog/drips/object-equality-in-javascript.html)
* [Deep comparison between two values](https://30secondsofcode.org/object#equals)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 CORS？

<details>
<summary>查看答案</summary>

Cross-Origin Resource Sharing or CORS is a mechanism that uses additional HTTP headers to grant a browser permission to access resources from a server at an origin different from the website origin.

An example of a cross-origin request is a web application served from `http://mydomain.com` that uses AJAX to make a request for `http://yourdomain.com`.

For security reasons, browsers restrict cross-origin HTTP requests initiated by JavaScript. `XMLHttpRequest` and `fetch` follow the same-origin policy, meaning a web application using those APIs can only request HTTP resources from the same origin the application was accessed, unless the response from the other origin includes the correct CORS headers.


#### 小贴士


* CORS behavior is not an error,  it’s a security mechanism to protect users.
* CORS is designed to prevent a malicious website that a user may unintentionally visit from making a request to a legitimate website to read their personal data or perform actions against their will.


##### 附加链接


* [MDN docs for CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 DOM？

<details>
<summary>查看答案</summary>

The DOM (Document Object Model) is a cross-platform API that treats HTML and XML documents as a tree structure consisting of nodes. These nodes (such as elements and text nodes) are objects that can be programmatically manipulated and any visible changes made to them are reflected live in the document. In a browser, this API is available to JavaScript where DOM nodes can be manipulated to change their styles, contents, placement in the document, or interacted with through event listeners.


#### 小贴士


* The DOM was designed to be independent of any particular programming language, making the structural representation of the document available from a single, consistent API.
* The DOM is constructed progressively in the browser as a page loads, which is why scripts are often placed at the bottom of a page, in the `<head>` with a `defer` attribute, or inside a `DOMContentLoaded` event listener. Scripts that manipulate DOM nodes should be run after the DOM has been constructed to avoid errors.
* `document.getElementById()` and `document.querySelector()` are common functions for selecting DOM nodes.
* Setting the `innerHTML` property to a new value runs the string through the HTML parser, offering an easy way to append dynamic HTML content to a node.


##### 附加链接


* [MDN docs for DOM](https://developer.mozilla.org/en-US/docs/DOM)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是事件委托，为什么它是有用的，你可以举个例子说明如何使用它？

<details>
<summary>查看答案</summary>

Event delegation is a technique of delegating events to a single common ancestor. Due to event bubbling, events "bubble" up the DOM tree by executing any handlers progressively on each ancestor element up to the root that may be listening to it.

DOM events provide useful information about the element that initiated the event via `Event.target`. This allows the parent element to handle behavior as though the target element was listening to the event, rather than all children of the parent or the parent itself.

This provides two main benefits:

* It increases performance and reduces memory consumption by only needing to register a single event listener to handle potentially thousands of elements.
* If elements are dynamically added to the parent, there is no need to register new event listeners for them.

Instead of:

```js
document.querySelectorAll("button").forEach(button => {
  button.addEventListener("click", handleButtonClick)
})
```

Event delegation involves using a condition to ensure the child target matches our desired element:

```js
document.addEventListener("click", e => {
  if (e.target.closest("button")) {
    handleButtonClick()
  }
})
```


#### 小贴士


* The difference between event bubbling and capturing


##### 附加链接


* [Event Delegation](https://davidwalsh.name/event-delegate)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 中，声明和表达式的区别？

<details>
<summary>查看答案</summary>

There are two main syntactic categories in JavaScript: expressions and statements. A third one is both together, referred to as an expression statement. They are roughly summarized as:

* **Expression**: produces a value
* **Statement**: performs an action
* **Expression statement**: produces a value and performs an action

A general rule of thumb:

> If you can print it or assign it to a variable, it’s an expression. If you can’t, it’s a statement.

##### Statements

```js
let x = 0

function declaration() {}

if (true) {
}
```

Statements appear as instructions that do something but don't produce values.

```js
// Assign `x` to the absolute value of `y`.
var x
if (y >= 0) {
  x = y
} else {
  x = -y
}
```

The only expression in the above code is `y >= 0` which produces a value, either `true` or `false`. A value is not produced by other parts of the code.

##### Expressions

Expressions produce a value. They can be passed around to functions because the interpreter replaces them with the value they resolve to.

```js
5 + 5 // => 10

lastCharacter("input") // => "t"

true === true // => true
```

##### Expression statements

There is an equivalent version of the set of statements used before as an expression using the conditional operator:

```js
// Assign `x` as the absolute value of `y`.
var x = y >= 0 ? y : -y
```

This is both an expression and a statement, because we are declaring a variable `x` (statement) as an evaluation (expression).


#### 小贴士


* Function declarations vs function expressions


##### 附加链接


* [What is the difference between a statement and an expression?](https://stackoverflow.com/questions/12703214/javascript-difference-between-a-statement-and-an-expression)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 中，什么是真值（truthy），假值（falsy）?

<details>
<summary>查看答案</summary>

一个值是真值（truthy）还是假值（falsy），取决于它在布尔上下文中是如何计算的。假值意味着和 `false` 相似，真值意味着和 `true` 相似。本质上，它们在执行某些操作时会被强制转换成 `true` 或 `false` 

JavaScript 里有 6 个假值：

* `false`
* `undefined`
* `null`
* `""` (空字符串)
* `NaN`
* `0` (包括正负 0 (`+0`，`-0`))

其余值看作真值

可以通过  `Boolean` 函数检查一个值是真值还是假值

```js
Boolean("") // false
Boolean([]) // true
```

这里有一个快捷方法，使用逻辑非操作符（`!`）。使用 `!` 会将值转换为一个等价的布尔值（即是，非假即真），再次使用 `!` 会转换回去，因此这是一个非常高效的布尔转换方法

```js
!!"" // false
!![] // true
```


#### 小贴士




##### 附加链接


* [Truthy on MDN](https://developer.mozilla.org/en/docs/Glossary/Truthy)
* [Falsy on MDN](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)

</details>

<br>[⬆ 返回顶部](#目录)

### 生成一个包含的 n 项斐波那契数列元素的数组

<details>
<summary>查看答案</summary>

初始化一个长度为 n 的空数组。使用 `Array.prototype.reduce()` 函数向这个数组累加值（使用最后两个数相加，除了第一个、第二个数）

```js
const fibonacci = n =>
  [...Array(n)].reduce(
    (acc, val, i) => acc.concat(i > 1 ? acc[i - 1] + acc[i - 2] : i),
    []
  )
```


#### 小贴士




##### 附加链接


* [Similar problem](https://github.com/Chalarangelo/30-seconds-of-code/blob/master/snippets_archive/fibonacciUntilNum.md)

</details>

<br>[⬆ 返回顶部](#目录)

### `0.1 + 0.2 === 0.3` 表达式的值是？

<details>
<summary>查看答案</summary>

这个表达式的计算结果为 `false` ，这是因为 JavaScript 遵循 IEEE 754 数学标准，使用 64 位浮点数进行运算。在进行十进制运算时会导致精度丢失，简言之，计算机是以 2 为基础进行运算的，而十进制是以 10 为基础进行运算的

```js
0.1 + 0.2 // 0.30000000000000004
```

一个解决方案是，定义一个误差值（epsilon），使得两数之差小于这个值，然后通过函数判断它们是否近似相等

```js
const approxEqual = (n1, n2, epsilon = 0.0001) => Math.abs(n1 - n2) < epsilon
approxEqual(0.1 + 0.2, 0.3) // true
```


#### 小贴士


* 这个问题的一个简单解决方案


##### 附加链接


* [A simple helper function to check equality](https://github.com/Chalarangelo/30-seconds-of-code#approximatelyequal)
* [Fix "0.1 + 0.2 = 0.300000004" in JavaScript](http://blog.blakesimpson.co.uk/read/61-fix-0-1-0-2-0-300000004-in-javascript)

</details>

<br>[⬆ 返回顶部](#目录)

### 数组 `map()` 和 `forEach()` 方法的区别？

<details>
<summary>查看答案</summary>

这两个方法都是进行遍历数组的方法。`map()` 方法通过调回回调函数映射每一个元素到新元素上，并且返回的是一个新数组。另一方面，`forEach()` 为每个元素调用回调函数，但是它不返回新数组。`forEach()` 函数通常用于在迭代中产生副作用，而 `map()` 函数是一种常见的函数式编程技术


#### 小贴士


* 如果你需要遍历数组，会造成元素变化，而且不需要返回值来生成一个新数组，你可以使用 `forEach()` 
* 对于保持数据的不变，`map()` 是正确的选择，原始数组的每一个值都会映射到一个新数组中


##### 附加链接


* [MDN docs for forEach](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)
* [MDN docs for map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
* [JavaScript — Map vs. ForEach](https://codeburst.io/javascript-map-vs-foreach-f38111822c0f)

</details>

<br>[⬆ 返回顶部](#目录)

### 下面的例子中，`console.log` 会打印出什么？

```js
var foo = 1
var foobar = function() {
  console.log(foo)
  var foo = 2
}
foobar()
```

<details>
<summary>查看答案</summary>

由于存在声明提升，局部变量 `foo` 会在 `console.log` 方法调用前声明。这就意味着 `console.log` 方法接受到的参数是局部变量 `foo`，而不是全局变量 `foo`。然而，变量提升并不会赋值，因此结果会输出 `undefined` 而不是 `2`


#### 小贴士


* 声明提升是 JavaScript 把声明移动到顶部的一种默认行为
* 注意严格模式


##### 附加链接


* [MDN docs for hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 中，声明提升是如何工作的？

<details>
<summary>查看答案</summary>

提升是 JavaScript 的一种机制，在编译阶段会把变量和函数的声明放入内存中。这就意味着无论函数和或变量在什么位置声明，它们都会移动到它们所在作用域的顶部，不管是全局作用域还是局部作用域

然而，它的值并不会被随着声明提升

下面这个代码片段：

```js
console.log(hoist)
var hoist = "value"
```

等价于：

```js
var hoist
console.log(hoist)
hoist = "value"
```

因此控制台打印 `hoist` 会输出 `undefined` 而不是 `"value"`.
提升也允许你在声明在程序出现之前调用它

```js
myFunction() // No error; logs "hello"
function myFunction() {
  console.log("hello")
}
```

但是要注意函数表达式赋值给变量的情况：

```js
myFunction() // Error: `myFunction` is not a function
var myFunction = function() {
  console.log("hello")
}
```


#### 小贴士


* 提升是将声明移动到顶部的 JavaScript 默认行为
* 函数声明在变量声明之前被提升


##### 附加链接


* [MDN docs for hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)
* [Understanding Hoisting in JavaScript](https://scotch.io/tutorials/understanding-hoisting-in-javascript)

</details>

<br>[⬆ 返回顶部](#目录)

### 为何将 JavaScript 源文件里的整个内容用匿名函数包裹起来？

<details>
<summary>查看答案</summary>

这个技术在 JavaScript 库广为流传。它在文件中包围整个内容创建一个闭包（创建里一个私有命名空间），因此它可以避免不同 JavaScript 模块和库的潜在命名冲突。这个函数会被立即调用，以便于把函数的返回值赋值给命名空间（库名）

```js
const myLibrary = (function() {
  var privateVariable = 2
  return {
    publicMethod: () => privateVariable
  }
})()
privateVariable // ReferenceError
myLibrary.publicMethod() // 2
```


#### 小贴士


* 许多流行的 JavaScript 库中使用它
* 创建一个私有命名空间


##### 附加链接


* [MDN docs for closures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

</details>

<br>[⬆ 返回顶部](#目录)

### 词法作用域和动态作用域的区别？

<details>
<summary>查看答案</summary>

词法作用域指的是一个函数定义的位置决定哪些变量你可以访问。另一方面，动态作用域使用函数调用的位置决定哪些变量你可以使用


#### 小贴士


* 词法作用域也叫做静态作用域
* 词法作用域允许闭包概念
* 大多数语言使用词法作用域，因为它倾向于源代码更易理解


##### 附加链接


* [Mozilla Docs Closures & Lexical Scoping](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

</details>

<br>[⬆ 返回顶部](#目录)

### 创建一个函数，用 ‘#’ 符号遮住字符串（除最后4个字符之外）

```js
mask("123456789") // "#####6789"
```

<details>
<summary>查看答案</summary>

> 这里有许多种解决方案，这个只是其中之一

使用 `String.prototype.slice()` 方法，参数传 `-4`，我们取到字符串的后 4 个字符。然后，使用 `String.prototype.padStart()` 方法指定字符指定长度填充原始字符串

```js
const mask = (str, maskChar = "#") =>
  str.slice(-4).padStart(str.length, maskChar)
```


#### 小贴士


* 如果高效的解决问题，那么首选简短的单行函数解决方案


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 MIME 类型，有什么作用？

<details>
<summary>查看答案</summary>

`MIME` 是 `多用途互联网邮件扩展` 的首字母缩写。它用来作为互联网上文件分类的标准

#### 小贴士


* 一个 `MIME 类型` 通常分为两部分：一个类型和一个子类型（用斜线 “/” 分割）。例如，微软 Word 文档的类型是 `application/msword`（即是，应用类型并且是子类型是 msword）


##### 附加链接


* [MIME Type MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)

</details>

<br>[⬆ 返回顶部](#目录)

### `null`  和 `undefined` 有何不同？

<details>
<summary>查看答案</summary>

在 JavaScript 中，两个值有区别的代表 “nothing” - `undefined` 和 `null`。它们具体的区别是，`null` 是显性的，`undefined` 是隐性的。一个属性不存在或没有赋值时，它的值时 `undefined`。设置值为 `null` 是隐性代表 “没有值”。本质上，当 “nothing” 不知道时，用 `undefined`，当 “nothing” 知道时，用 `null`


#### 小贴士


* `typeof undefined` 计算得到 `"undefined"`.
* `typeof null` 计算得到 `"object"`. 然而, 它依旧是一个原始类型值，它被认为是在 JavaScript 实现中的一个 bug
* `undefined == null` 计算得到 `true`.


##### 附加链接


* [MDN docs for null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)
* [MDN docs for undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)

</details>

<br>[⬆ 返回顶部](#目录)

### 描述下创建对象方式的不同，哪种方式更推荐？

<details>
<summary>查看答案</summary>

##### 对象字面量

常常用来存储出现一次的数据

```js
const person = {
  name: "John",
  age: 50,
  birthday() {
    this.age++
  }
}
person.birthday() // person.age === 51
```

##### 构造函数

经常用于创建一个对象的多个实例，而且每个实例彼此互不影响，必须使用 `new` 操作符调用构造器，否则全局对象会被污染/改变

```js
function Person(name, age) {
  this.name = name
  this.age = age
}
Person.prototype.birthday = function() {
  this.age++
}
const person1 = new Person("John", 50)
const person2 = new Person("Sally", 20)
person1.birthday() // person1.age === 51
person2.birthday() // person2.age === 21
```

##### 工厂函数

创建一个和构造函数相似的对象，但是可以通过闭包存储私有数据。在调用函数或使用 `this` 关键字之前不需要使用 `new` 操作符。工厂函数通常放弃了原型概念，并且将所有属性和方法保持在对象上

```js
const createPerson = (name, age) => {
  const birthday = () => person.age++
  const person = { name, age, birthday }
  return person
}
const person = createPerson("John", 50)
person.birthday() // person.age === 51
```

##### `Object.create()`

设置新创建对象的原型对象

```js
const personProto = {
  birthday() {
    this.age++
  }
}
const person = Object.create(personProto)
person.age = 50
person.birthday() // person.age === 51
```

`Object.create()` 也支持第二个参数，它的担当定义新属性的描述符

```js
Object.create(personProto, {
  age: {
    value: 50,
    writable: true,
    enumerable: true
  }
})
```


#### 小贴士


* 原型是其他对象继承属性和方法的对象
* 工厂函数通过闭包提供私有属性和方法，但是会增加内存消耗作为交换，然而 `class` 没有私有属性和方法，但可以通过使用单原型对象减少内存影响


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 形参和实参的区别？

<details>
<summary>查看答案</summary>

形参是函数吧定义的变量名，而实参是在函数调用时所给的值

```js
function myFunction(parameter1, parameter2) {
  console.log(arguments[0]) // "argument1"
}
myFunction("argument1", "argument2")
```


#### 小贴士


* `arguments` 是一个类数组对象，包括函数调用提供的参数信息
* `myFunction.length` 描述一个函数的形参数量（无论形参有多少，无视它提供的实参）


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### JavaScript 里是通过值传递还是引用传递？

<details>
<summary>查看答案</summary>

JavaScript 总是通过值传递的。然而，对于对象来说，它的值是一个指向对象的引用


#### 小贴士


* 值传递和引用传递的区别


##### 附加链接


* [JavaScript Value vs Reference](https://medium.com/dailyjs/back-to-roots-javascript-value-vs-reference-8fb69d587a18)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 Promises？

<details>
<summary>查看答案</summary>

The `Promise` object represents the eventual completion (or failure) of an asynchronous operation, and its resulting value.
An example can be the following snippet, which after 100ms prints out the result string to the standard output. Also, note the catch, which can be used for error handling. `Promise`s are chainable.

```js
new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve("result")
  }, 100)
})
  .then(console.log)
  .catch(console.error)
```


#### 小贴士


* Take a look into the other questions regarding `Promise`s!


##### 附加链接


* [Master the JavaScript Interview: What is a Promise?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e772618)

</details>

<br>[⬆ 返回顶部](#目录)

### 原型继承和经典继承方式有何不同？

<details>
<summary>查看答案</summary>

In the classical inheritance paradigm, object instances inherit their properties and functions from a class, which acts as a blueprint for the object. Object instances are typically created using a constructor and the `new` keyword.

In the prototypal inheritance paradigm, object instances inherit directly from other objects and are typically created using factory functions or `Object.create()`.


#### 小贴士




##### 附加链接


* [MDN docs for inheritance and the prototype chain](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)

</details>

<br>[⬆ 返回顶部](#目录)

### 下面的代码会输出什么？

```js
const a = [1, 2, 3]
const b = [1, 2, 3]
const c = "1,2,3"

console.log(a == c)
console.log(a == b)
```

<details>
<summary>查看答案</summary>

第一个 `console.log` 输出 `true` ，因为 JavaScript 的编译器执行了类型转换，因此它们通过 `string` 来比较值。另一方面，第二个 `console.log` 输出 `false`，因为数组是对象，而对象是通过引用比较的


#### 小贴士


* JavaScript 执行自动类型转换
* Objects 通过引用比较
* 原始值通过值比较


##### 附加链接


* [JavaScript Value vs Reference](https://medium.com/dailyjs/back-to-roots-javascript-value-vs-reference-8fb69d587a18)

</details>

<br>[⬆ 返回顶部](#目录)

### 下面的函数会返回什么？

```js
function greet() {
  return
  {
    message: "hello"
  }
}
```

<details>
<summary>查看答案</summary>

因为 JavaScript 自动插入分号（ASI）机制，编译器在 `return` 之后会插入一个分号，因此这个函数会返回 `undefined` 并且不会抛出报错


#### 小贴士


* 自动添加分号导致耗时的 bug


##### 附加链接


* [Automatic semicolon insertion in JavaScript](http://2ality.com/2011/05/semicolon-insertion.html)

</details>

<br>[⬆ 返回顶部](#目录)

### JavaScript 里分号是必须的吗？

<details>
<summary>查看答案</summary>

有时由于 JavaScript 的分号自动插入机制，解释器会在多数语句后放置分号。这就意味着在大多数情况下分号可以被忽略

然而，有些情况分号是必须的。在块的开始不需要加分号，但是如果它们遵循在一行并且：

1. 行的开始是 `[`

```js
const previousLine = 3
;[1, 2, previousLine].map(n => n * 2)
```

2.  行的开始是 `(`

```js
const previousLine = 3
;(function() {
  // ...
})()
```

在上面的例子，解释器并不会在 `3` 后面加入分号，并且因此它会把 `3` 当作是尝试对象访问属性或调用函数，这样会抛出错误


#### 小贴士


* 在 JavaScript 中，分号通常是可选的，但是在一些边缘情况它们是必须的
* 如果你不用分号，像 Prettier 之类的工具会在文本编辑器保存时插入分号，以防出错


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 里，什么是短路运算？

<details>
<summary>查看答案</summary>

Short-circuit evaluation involves logical operations evaluating from left-to-right and stopping early.

```js
true || false
```

In the above sample using logical OR, JavaScript won't look at the second operand `false`, because the expression evaluates to `true` regardless. This is known as short-circuit evaluation.

This also works for logical AND.

```js
false && true
```

This means you can have an expression that throws an error if evaluated, and it won't cause issues.

```js
true || nonexistentFunction()
false && nonexistentFunction()
```

This remains true for multiple operations because of left-to-right evaluation.

```js
true || nonexistentFunction() || window.nothing.wouldThrowError
true || window.nothing.wouldThrowError
true
```

A common use case for this behavior is setting default values. If the first operand is falsy the second operand will be evaluated.

```js
const options = {}
const setting = options.setting || "default"
setting // "default"
```

Another common use case is only evaluating an expression if the first operand is truthy.

```js
// Instead of:
addEventListener("click", e => {
  if (e.target.closest("button")) {
    handleButtonClick(e)
  }
})

// You can take advantage of short-circuit evaluation:
addEventListener(
  "click",
  e => e.target.closest("button") && handleButtonClick(e)
)
```

In the above case, if `e.target` is not or does not contain an element matching the `"button"` selector, the function will not be called. This is because the first operand will be falsy, causing the second operand to not be evaluated.


#### 小贴士


* Logical operations do not produce a boolean unless the operand(s) evaluate to a boolean.


##### 附加链接


* [JavaScript: What is short-circuit evaluation?](https://codeburst.io/javascript-what-is-short-circuit-evaluation-ff22b2f5608c)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 里，同步代码和异步代码有什么不同？

<details>
<summary>查看答案</summary>

同步意味着每一个操作必须等前一个完成后才能执行

异步意味着一个操作可以在其他操作仍然在执行过程中发生

在 JavaScript, 由于单线程特性所有的代码都是同步的。然而，异步操作（例如 `XMLHttpRequest` 或 `setTimeout`）并不是程序的一部分，它是脱离主线程的，因为它们是被内置代码控制的（浏览器的 API），但是程序的回调部分仍然是同步执行的


#### 小贴士


* JavaScript 有一个基于 “事件循环” 的并发模型JavaScript has a concurrency model based on an "event loop".
* 像 `alert` 这样的函数会阻塞主线程，因此在用户关闭它之前是不会有用户输入被注册的


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 下面的代码执行的结果是什么？

```js
typeof typeof 0
```

<details>
<summary>查看答案</summary>

计算得到 `"string"`.

`typeof 0` 计算得到字符串 `"number"`，因此 `typeof "number"` 计算得到 `"string"`.


#### 小贴士




##### 附加链接


* [MDN docs for typeof](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 JavaScript 的数据类型？

<details>
<summary>查看答案</summary>

最新的 ECMAScript 标准定义了 7 种数据类型，其中 6 种是原始类型：`Boolean`，`Null`，`Undefined`，`Number`，`String`，`Symbol`，和一种非原始数据类型：`Object`

#### 小贴士


* 提及新添加的数据类型 `Symbol`
* `Array`，`Date` 和 `function` 都是 `object` 类型
* 函数在 JavaScript 是具有可调用能力的对象


##### 附加链接


* [MDN docs for data types and data structures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
* [Understanding Data Types in JavaScript](https://www.digitalocean.com/community/tutorials/understanding-data-types-in-javascript)

</details>

<br>[⬆ 返回顶部](#目录)

### `let` `var` `const` 和无关键字声明变量有何不同？

<details>
<summary>查看答案</summary>

##### No keyword

When no keyword exists before a variable assignment, it is either assigning a global variable if one does not exist, or reassigns an already declared variable. In non-strict mode, if the variable has not yet been declared, it will assign the variable as a property of the global object (`window` in browsers). In strict mode, it will throw an error to prevent unwanted global variables from being created.

##### var

`var` was the default statement to declare a variable until ES2015. It creates a function-scoped variable that can be reassigned and redeclared. However, due to its lack of block scoping, it can cause issues if the variable is being reused in a loop that contains an asynchronous callback because the variable will continue to exist outside of the block scope.

Below, by the time the the `setTimeout` callback executes, the loop has already finished and the `i` variable is `10`, so all ten callbacks reference the same variable available in the function scope.

```js
for (var i = 0; i < 10; i++) {
  setTimeout(() => {
    // logs `10` ten times
    console.log(i)
  })
}

/* Solutions with `var` */
for (var i = 0; i < 10; i++) {
  // Passed as an argument will use the value as-is in
  // that point in time
  setTimeout(console.log, 0, i)
}

for (var i = 0; i < 10; i++) {
  // Create a new function scope that will use the value
  // as-is in that point in time
  ;(i => {
    setTimeout(() => {
      console.log(i)
    })
  })(i)
}
```

##### let

`let` was introduced in ES2015 and is the new preferred way to declare variables that will be reassigned later. Trying to redeclare a variable again will throw an error. It is block-scoped so that using it in a loop will keep it scoped to the iteration.

```js
for (let i = 0; i < 10; i++) {
  setTimeout(() => {
    // logs 0, 1, 2, 3, ...
    console.log(i)
  })
}
```

##### const

`const` was introduced in ES2015 and is the new preferred default way to declare all variables if they won't be reassigned later, even for objects that will be mutated (as long as the reference to the object does not change). It is block-scoped and cannot be reassigned.

```js
const myObject = {}
myObject.prop = "hello!" // No error
myObject = "hello" // Error
```


#### 小贴士


* All declarations are hoisted to the top of their scope.
* However, with `let` and `const` there is a concept called the temporal dead zone (TDZ). While the declarations are still hoisted, there is a period between entering scope and being declared where they cannot be accessed.
* Show a common issue with using `var` and how `let` can solve it, as well as a solution that keeps `var`.
* `var` should be avoided whenever possible and prefer `const` as the default declaration statement for all variables unless they will be reassigned later, then use `let` if so.


##### 附加链接


* [`let` vs `const`](https://wesbos.com/let-vs-const/)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是跨站脚本攻击（XSS），你是如何阻止它的？

<details>
<summary>查看答案</summary>

XSS refers to client-side code injection where the attacker injects malicious scripts into a legitimate website or web application. This is often achieved when the application does not validate user input and freely injects dynamic HTML content.

For example, a comment system will be at risk if it does not validate or escape user input. If the comment contains unescaped HTML, the comment can inject a `<script>` tag into the website that other users will execute against their knowledge.

* The malicious script has access to cookies which are often used to store session tokens. If an attacker can obtain a user’s session cookie, they can impersonate the user.
* The script can arbitrarily manipulate the DOM of the page the script is executing in, allowing the attacker to insert pieces of content that appear to be a real part of the website.
* The script can use AJAX to send HTTP requests with arbitrary content to arbitrary destinations.


#### 小贴士


* On the client, using `textContent` instead of `innerHTML` prevents the browser from running the string through the HTML parser which would execute scripts in it.
* On the server, escaping HTML tags will prevent the browser from parsing the user input as actual HTML and therefore won't execute the script.


##### 附加链接


* [Cross-Site Scripting Attack (XSS)](https://www.acunetix.com/websitesecurity/cross-site-scripting/)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是大 O 标记法？

<details>
<summary>查看答案</summary>

Big O notation is used in Computer Science to describe the time complexity of an algorithm. The best algorithms will execute the fastest and have the simplest complexity.

Algorithms don't always perform the same and may vary based on the data they are supplied. While in some cases they will execute quickly, in other cases they will execute slowly, even with the same number of elements to deal with.

In these examples, the base time is 1 element = `1ms`.

##### O(1)

```js
arr[arr.length - 1]
```

* 1000 elements = `1ms`

Constant time complexity. No matter how many elements the array has, it will theoretically take (excluding real-world variation) the same amount of time to execute.

##### O(N)

```js
arr.filter(fn)
```

* 1000 elements = `1000ms`

Linear time complexity. The execution time will increase linearly with the number of elements the array has. If the array has 1000 elements and the function takes 1ms to execute, 7000 elements will take 7ms to execute. This is because the function must iterate through all elements of the array before returning a result.

##### O([1, N])

```js
arr.some(fn)
```

* 1000 elements = `1ms <= x <= 1000ms`

The execution time varies depending on the data supplied to the function, it may return very early or very late. The best case here is O(1) and the worst case is O(N).

##### O(NlogN)

```js
arr.sort(fn)
```

* 1000 elements ~= `10000ms`

Browsers usually implement the quicksort algorithm for the `sort()` method and the average time complexity of quicksort is O(NlgN). This is very efficient for large collections.

##### O(N^2)

```js
for (let i = 0; i < arr.length; i++) {
  for (let j = 0; j < arr.length; j++) {
    // ...
  }
}
```

* 1000 elements = `1000000ms`

The execution time rises quadratically with the number of elements. Usually the result of nesting loops.

##### O(N!)

```js
const permutations = arr => {
  if (arr.length <= 2) return arr.length === 2 ? [arr, [arr[1], arr[0]]] : arr
  return arr.reduce(
    (acc, item, i) =>
      acc.concat(
        permutations([...arr.slice(0, i), ...arr.slice(i + 1)]).map(val => [
          item,
          ...val
        ])
      ),
    []
  )
}
```

* 1000 elements = `Infinity` (practically) ms

The execution time rises extremely fast with even just 1 addition to the array.


#### 小贴士


* Be wary of nesting loops as execution time increases exponentially.


##### 附加链接


* [Big O Notation in JavaScript](https://medium.com/cesars-tech-insights/big-o-notation-javascript-25c79f50b19b)

</details>

<br>[⬆ 返回顶部](#目录)

### 你是怎么避免回调地狱的？

```js
getData(function(a) {
  getMoreData(a, function(b) {
    getMoreData(b, function(c) {
      getMoreData(c, function(d) {
        getMoreData(d, function(e) {
          // ...
        })
      })
    })
  })
})
```

<details>
<summary>查看答案</summary>

Refactoring the functions to return promises and using `async/await` is usually the best option. Instead of supplying the functions with callbacks that cause deep nesting, they return a promise that can be `await`ed and will be resolved once the data has arrived, allowing the next line of code to be evaluated in a sync-like fashion.

The above code can be restructured like so:

```js
async function asyncAwaitVersion() {
  const a = await getData()
  const b = await getMoreData(a)
  const c = await getMoreData(b)
  const d = await getMoreData(c)
  const e = await getMoreData(d)
  // ...
}
```

There are lots of ways to solve the issue of callback hells:

* Modularization: break callbacks into independent functions
* Use a control flow library, like async
* Use generators with Promises
* Use async/await (from v7 on)


#### 小贴士


* As an efficient JavaScript developer, you have to avoid the constantly growing indentation level, produce clean and readable code and be able to handle complex flows.


##### 附加链接


* [Avoiding Callback Hell in Node.js](http://stackabuse.com/avoiding-callback-hell-in-node-js/)
* [Asynchronous JavaScript: From Callback Hell to Async and Await](https://blog.hellojs.org/asynchronous-javascript-from-callback-hell-to-async-and-await-9b9ceb63c8e8)

</details>

<br>[⬆ 返回顶部](#目录)

### 回调引用 refs 和 findDOMNode 哪个更推荐使用？

<details>
<summary>查看答案</summary>

Callback refs are preferred over the `findDOMNode()` API, due to the fact that `findDOMNode()` prevents certain improvements in React in the future.

```jsx
/* Legacy approach using findDOMNode() */
class MyComponent extends Component {
  componentDidMount() {
    findDOMNode(this).scrollIntoView()
  }

  render() {
    return <div />
  }
}

/* Recommended approach using callback refs */
class MyComponent extends Component {
  componentDidMount() {
    this.node.scrollIntoView()
  }

  render() {
    return <div ref={node => (this.node = node)} />
  }
}
```


#### 小贴士


* Callback refs are preferred over `findDOMNode()`.


##### 附加链接


* [React docs on Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html#exposing-dom-refs-to-parent-components)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是闭包，你可以举一个有用的例子吗？

<details>
<summary>查看答案</summary>

一个闭包是一个定义另一个函数内部可以访问它的词法作用域，甚至是它在词法作用域外执行。闭包可以在三种作用域中访问变量：

* 定义在自己作用域下的变量
* 定义在父函数作用域下的变量
* 定义在全局作用域的变量

在 JavaScript 中，所有的函数都是闭包，因为它们可以访问外部作用域，但是大多数函数并没有利用好闭包的有效性：状态的持久性。因此闭包有时也叫有状态函数

此外，闭包是唯一一种存储私有数据不能被外部访问的方式。它们是 UMD（Universal Module Definition，通用模块定义）模式的关键，它已经在许多库中熟练地被使用，只暴露一个公共的 API，隐藏私有的实现细节，阻止了在用户代码中和其他库的命名冲突


#### 小贴士


* 闭包是有用的，因为它们可以使你的数据和操作它的函数关联起来
* 一个闭包可以用一个单方法替代
* 闭包可以被用来模仿私有属性和方法


##### 附加链接


* [MDN docs for closures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)
* [What is a closure](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36)
* [I never understood JavaScript closures](https://medium.com/dailyjs/i-never-understood-javascript-closures-9663703368e8)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 中，什么是 context？

<details>
<summary>查看答案</summary>

Context provides a way to pass data through the component tree without having to pass props down manually at every level. For example, authenticated user, locale preference, UI theme need to be accessed in the application by many components.

```jsx
const { Provider, Consumer } = React.createContext(defaultValue)
```


#### 小贴士


* Context provides a way to pass data through a tree of React components, without having to manually pass props.
* Context is designed to share data that is considered _global_ for a tree of React components.


##### 附加链接


* [React docs on Context](https://reactjs.org/docs/context.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是事件驱动编程？

<details>
<summary>查看答案</summary>

Event-driven programming is a paradigm that involves building applications that send and receive events. When the program emits events, the program responds by running any callback functions that are registered to that event and context, passing in associated data to the function. With this pattern, events can be emitted into the wild without throwing errors even if no functions are subscribed to it.

A common example of this is the pattern of elements listening to DOM events such as `click` and `mouseenter`, where a callback function is run when the event occurs.

```js
document.addEventListener("click", function(event) {
  // This callback function is run when the user
  // clicks on the document.
})
```

Without the context of the DOM, the pattern may look like this:

```js
const hub = createEventHub()
hub.on("message", function(data) {
  console.log(`${data.username} said ${data.text}`)
})
hub.emit("message", {
  username: "John",
  text: "Hello?"
})
```

With this implementation, `on` is the way to _subscribe_ to an event, while `emit` is the way to _publish_ the event.


#### 小贴士


* Follows a publish-subscribe pattern.
* Responds to events that occur by running any callback functions subscribed to the event.
* Show how to create a simple pub-sub implementation with JavaScript.


##### 附加链接


* [MDN docs on Events and Handlers](https://developer.mozilla.org/en-US/docs/Web/Guide/Events/Overview_of_Events_and_Handlers)
* [Understanding Node.js event-driven architecture](https://medium.freecodecamp.org/understanding-node-js-event-driven-architecture-223292fcbc2d)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是函数式编程？

<details>
<summary>查看答案</summary>

函数式编程是一个声明式方式构建的范式，使用纯函数避免数据共享和数据突变。函数总是以相同的输入返回相同输出值，而不会产生副作用，是函数式编程的支柱。许多程序员认为它更接近软件开发，因为它可以减少错误和认知负担


#### 小贴士


* 更清晰，更简洁的开发体验
* 简单的函数复合
* 使函数式编程可能的 JavaScript 的特征（`.map`, `.reduce` 等等）
* JavaScript 是一个多范式编程语言（面向对象编程和函数式编程和谐共处）


##### 附加链接


* [Javascript and Functional Programming: An Introduction](https://hackernoon.com/javascript-and-functional-programming-an-introduction-286aa625e26d)
* [Master the JavaScript Interview:  什么是函数式编程？](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)

</details>

<br>[⬆ 返回顶部](#目录)

### 阐释下命令式编程和声明式编程的区别？

<details>
<summary>查看答案</summary>

These two types of programming can roughly be summarized as:

* Imperative: **how** to achieve something
* Declarative: **what** should be achieved

A common example of declarative programming is CSS. The developer specifies CSS properties that describe what something should look like rather than how to achieve it. The "how" is abstracted away by the browser.

On the other hand, imperative programming involves the steps required to achieve something. In JavaScript, the differences can be contrasted like so:

##### Imperative

```js
const numbers = [1, 2, 3, 4, 5]
const numbersDoubled = []
for (let i = 0; i < numbers.length; i++) {
  numbersDoubled[i] = numbers[i] * 2
}
```

We manually loop over the numbers of the array and assign the new index as the number doubled.

##### Declarative

```js
const numbers = [1, 2, 3, 4, 5]
const numbersDoubled = numbers.map(n => n * 2)
```

We declare that the new array is mapped to a new one where each value is doubled.


#### 小贴士


* Declarative programming often works with functions and expressions. Imperative programming frequently uses statements and relies on low-level features that cause mutations, while declarative programming has a strong focus on abstraction and purity.
* Declarative programming is more terse and easier to process at a glance.


##### 附加链接


* [Declarative vs Imperative Programming](https://codeburst.io/declarative-vs-imperative-programming-a8a7c93d9ad2)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是缓存代理模式（memoization）？

<details>
<summary>查看答案</summary>

缓存代理是缓存函数调用输出的过程，以致于下一次调用更快。再次调用相同输入的函数时，返回已缓存的输出，而无需再次计算

在 JavaScript，一个基本的实现看起来像这样：

```js
const memoize = fn => {
  const cache = new Map()
  return value => {
    const cachedResult = cache.get(value)
    if (cachedResult !== undefined) return cachedResult
    const result = fn(value)
    cache.set(value, result)
    return result
  }
}
```


#### 小贴士


* 上述技术会返回一个一元函数，即使函数接受多个参数
* 第一次调用函数可能会比通常慢，因为在返回值之前它会检查结果是否存在和设置缓存，增加开销
* 缓存代理在后续的函数调用中提高了性能，但是仍需要在第一次调用时作用


##### 附加链接


* [Implementing memoization in JavaScript](https://www.sitepoint.com/implementing-memoization-in-javascript/)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 类方式定义的组件中，你如何保证方法得到的 ‘this’ 是正确的？

<details>
<summary>查看答案</summary>

* In JavaScript classes, the methods are not bound by default. This means that their `this` context can be changed (in the case of an event handler, to the element that is listening to the event) and will not refer to the component instance. To solve this, `Function.prototype.bind()` can be used to enforce the `this` context as the component instance.

```jsx
constructor(props) {
  super(props);
  this.handleClick = this.handleClick.bind(this);
}

handleClick() {
  // Perform some logic
}
```

* The `bind` approach can be verbose and requires defining a `constructor`, so the new public class fields syntax is generally preferred:

```jsx
handleClick = () => {
  console.log('this is:', this);
}

render() {
  return (
    <button onClick={this.handleClick}>
      Click me
    </button>
  );
}
```

* You can also use an inline arrow function, because lexical `this` (referring to the component instance) is preserved:

```jsx
<button onClick={e => this.handleClick(e)}>Click me</button>
```

Note that extra re-rendering can occur using this technique because a new function reference is created on render, which gets passed down to child components and breaks `shouldComponentUpdate` / `PureComponent` shallow equality checks to prevent unnecessary re-renders. In cases where performance is important, it is preferred to go with `bind` in the constructor, or the public class fields syntax approach, because the function reference remains constant.


#### 小贴士


* You can either bind methods to the component instance context in the constructor, use public class fields syntax, or use inline arrow functions.


##### 附加链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)
* [React docs on Passing Functions to Components](https://reactjs.org/docs/faq-functions.html#how-do-i-bind-a-function-to-a-component-instance)

</details>

<br>[⬆ 返回顶部](#目录)

### 对比下可变与不可变值，可变与不可变方法

<details>
<summary>查看答案</summary>

The two terms can be contrasted as:

* Mutable: subject to change
* Immutable: cannot change

In JavaScript, objects are mutable while primitive values are immutable. This means operations performed on objects can change the original reference in some way, while operations performed on a primitive value cannot change the original value.

All `String.prototype` methods do not have an effect on the original string and return a new string. On the other hand, while some methods of `Array.prototype` do not mutate the original array reference and produce a fresh array, some cause mutations.

```js
const myString = "hello!"
myString.replace("!", "") // returns a new string, cannot mutate the original value

const originalArray = [1, 2, 3]
originalArray.push(4) // mutates originalArray, now [1, 2, 3, 4]
originalArray.concat(4) // returns a new array, does not mutate the original
```


#### 小贴士


* List of mutating and non-mutating array methods


##### 附加链接


* [Mutating vs non-mutating array methods](https://lorenstewart.me/2017/01/22/javascript-array-methods-mutating-vs-non-mutating/)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 中，哪个值不等于它自己？

<details>
<summary>查看答案</summary>

`NaN`（Not-a-Number）是唯一一个在用任何比较操作符比较时不等于自己本身的值。`NaN` 经常表示数学计算无意义的结果，因此两个 `NaN` 值的相等比较毫无意义

#### 小贴士


* `isNaN()` 和 `Number.isNaN()` 的区别
* `const isNaN = x => x !== x`


##### 附加链接


* [MDN docs for `NaN`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN)

</details>

<br>[⬆ 返回顶部](#目录)

### 创建一个管道函数，返回一个接受一个参数从左到右执行的合成函数

```js
const square = v => v * v
const double = v => v * 2
const addOne = v => v + 1
const res = pipe(square, double, addOne)
res(3) // 19; addOne(double(square(3)))
```

<details>
<summary>查看答案</summary>

通过剩余参数操作符 `...` 收集所有接受到的实参，并且返回一个用 `Array.prototype.reduce()` 处理（在返回最终值之前执行一系列操作）的一元函数

```js
const pipe = (...fns) => x => fns.reduce((v, fn) => fn(v), x)
```


#### 小贴士


* 函数合成是一个两个或更多函数组合生产一个函数的过程


##### 附加链接


* [What is function composition?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-function-composition-20dfb109a1a0)

</details>

<br>[⬆ 返回顶部](#目录)

### ReactJS 中，‘portals’（传送门） 是什么？

<details>
<summary>查看答案</summary>

Portal are the recommended way to render children into a DOM node that exists outside the DOM hierarchy of the parent component.

```jsx
ReactDOM.createPortal(child, container)
```

The first argument (`child`) is any renderable React child, such as an element, string, or fragment. The second argument (`container`) is a DOM element.


#### 小贴士




##### 附加链接


* [React docs on Portals](https://reactjs.org/docs/portals.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是纯函数？

<details>
<summary>查看答案</summary>

一个纯函数满足两个条件：

* 给定相同的输入，返回相同的输出
* 函数不会在函数作用域外造成副作用（即，改变函数外的数据或函数接受到的数据）

只要满足以上两个条件，纯函数就可以改变内部数据

##### 纯函数

```js
const a = (x, y) => x + y
const b = (arr, value) => arr.concat(value)
const c = arr => [...arr].sort((a, b) => a - b)
```

##### 非纯函数

```js
const a = (x, y) => x + y + Math.random()
const b = (arr, value) => (arr.push(value), arr)
const c = arr => arr.sort((a, b) => a - b)
```


#### 小贴士


* 纯函数更易推导由于它们的可靠性
* 所有的函数都应该时纯函数，除非显示地造成副作用（即，`setInnerHTML`）
* 如果一个函数没有返回一个值，那么表明它正在造成副作用


##### 附加链接


* [Pure functions in JavaScript](http://www.nicoespeon.com/en/2015/01/pure-functions-javascript/)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是递归，什么时候它是有用的？

<details>
<summary>查看答案</summary>

Recursion is the repeated application of a process. In JavaScript, recursion involves functions that call themselves repeatedly until they reach a base condition. The base condition breaks out of the recursion loop because otherwise the function would call itself indefinitely. Recursion is very useful when working with data structures that contain nesting where the number of levels deep is unknown.

For example, you may have a thread of comments returned from a database that exist in a flat array but need to be nested for display in the UI. Each comment is either a top-level comment (no parent) or is a reply to a parent comment. Comments can be a reply of a reply of a reply... we have no knowledge beforehand the number of levels deep a comment may be. This is where recursion can help.

```js
const nest = (items, id = null, link = "parent_id") =>
  items
    .filter(item => item[link] === id)
    .map(item => ({ ...item, children: nest(items, item.id) }))

const comments = [
  { id: 1, parent_id: null, text: "First reply to post." },
  { id: 2, parent_id: 1, text: "First reply to comment #1." },
  { id: 3, parent_id: 1, text: "Second reply to comment #1." },
  { id: 4, parent_id: 3, text: "First reply to comment #3." },
  { id: 5, parent_id: 4, text: "First reply to comment #4." },
  { id: 6, parent_id: null, text: "Second reply to post." }
]

nest(comments)
/*
[
  { id: 1, parent_id: null, text: "First reply to post.", children: [...] },
  { id: 6, parent_id: null, text: "Second reply to post.", children: [] }
]
*/
```

In the above example, the base condition is met if `filter()` returns an empty array. The chained `map()` won't invoke the callback function which contains the recursive call, thereby breaking the loop.


#### 小贴士


* Recursion is useful when working with data structures containing an unknown number of nested structures.
* Recursion must have a base condition to be met that breaks out of the loop or it will call itself indefinitely.


##### 附加链接


* [In plain English, what is recursion?](https://softwareengineering.stackexchange.com/questions/25052/in-plain-english-what-is-recursion)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 refs，什么时候用它们？

<details>
<summary>查看答案</summary>

Refs provide a way to access DOM nodes or React elements created in the render method. Refs should be used sparringly, but there are some good use cases for refs, such as:

* Managing focus, text selection, or media playback.
* Triggering imperative animations.
* Integrating with third-party DOM libraries.

Refs are created using `React.createRef()` method and attached to React elements via the `ref` attribute. In order to use refs throughout the component, just assign the `ref` to the instance property within the constructor:

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props)
    this.myRef = React.createRef()
  }
  render() {
    return <div ref={this.myRef} />
  }
}
```

Refs can also be used in functional components with the help of closures.


#### 小贴士


* Refs are used to return a reference to an element.
* Refs shouldn't be overused.
* You can create a ref using `React.createRef()` and attach to Reactelements via the `ref` attribute.


##### 附加链接


* [React docs on Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 解释下静态方法和实例方法的区别

<details>
<summary>查看答案</summary>

静态方法属于类（class），不会作用于实例上，而实例方法属于类原型，会被所有实例继承并且作用于它们

```js
Array.isArray // 数据的静态方法static method of Array
Array.prototype.push // 数组的实例方法instance method of Array
```

在这个例子中，`Array.isArray` 作为实例方法并没有意义，因为我们在使用时已经知道它是一个数组

实例方法可以在技术上和静态方法一样作用，但提供简洁的语法：

```js
const arr = [1, 2, 3]
arr.push(4)
Array.push(arr, 4)
```


#### 小贴士


* 如何用 ES2015 class 语法创建静态和实例方法


##### 附加链接


* [Classes on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

</details>

<br>[⬆ 返回顶部](#目录)

### `this` 关键字是什么，它是如何工作的？

<details>
<summary>查看答案</summary>

The `this` keyword is an object that represents the context of an executing function. Regular functions can have their `this` value changed with the methods `call()`, `apply()` and `bind()`. Arrow functions implicitly bind `this` so that it refers to the context of its lexical environment, regardless of whether or not its context is set explicitly with `call()`.

Here are some common examples of how `this` works:

##### Object literals

`this` refers to the object itself inside regular functions if the object precedes the invocation of the function.

Properties set as `this` do not refer to the object.

```js
var myObject = {
  property: this,
  regularFunction: function() {
    return this
  },
  arrowFunction: () => {
    return this
  },
  iife: (function() {
    return this
  })()
}
myObject.regularFunction() // myObject
myObject["regularFunction"]() // my Object

myObject.property // NOT myObject; lexical `this`
myObject.arrowFunction() // NOT myObject; lexical `this`
myObject.iife // NOT myObject; lexical `this`
const regularFunction = myObject.regularFunction
regularFunction() // NOT myObject; lexical `this`
```

##### Event listeners

`this` refers to the element listening to the event.

```js
document.body.addEventListener("click", function() {
  console.log(this) // document.body
})
```

##### Constructors

`this` refers to the newly created object.

```js
class Example {
  constructor() {
    console.log(this) // myExample
  }
}
const myExample = new Example()
```

##### Manual

With `call()` and `apply()`, `this` refers to the object passed as the first argument.

```js
var myFunction = function() {
  return this
}
myFunction.call({ customThis: true }) // { customThis: true }
```

##### Unwanted `this`

Because `this` can change depending on the scope, it can have unexpected values when using regular functions.

```js
var obj = {
  arr: [1, 2, 3],
  doubleArr() {
    return this.arr.map(function(value) {
      // this is now this.arr
      return this.double(value)
    })
  },
  double() {
    return value * 2
  }
}
obj.doubleArr() // Uncaught TypeError: this.double is not a function
```


#### 小贴士


* In non-strict mode, global `this` is the global object (`window` in browsers), while in strict mode global `this` is `undefined`.
* `Function.prototype.call` and `Function.prototype.apply` set the `this` context of an executing function as the first argument, with `call` accepting a variadic number of arguments thereafter, and `apply` accepting an array as the second argument which are fed to the function in a variadic manner.
* `Function.prototype.bind` returns a new function that enforces the `this` context as the first argument which cannot be changed by other functions.
* If a function requires its `this` context to be changed based on how it is called, you must use the `function` keyword. Use arrow functions when you want `this` to be the surrounding (lexical) context.


##### 附加链接


* [`this` on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)

</details>

<br>[⬆ 返回顶部](#目录)

### 诸如 React，Vue，Angular，Hyperapp 等 JavaScript UI 库/框架的目的是什么？

<details>
<summary>查看答案</summary>

The main purpose is to avoid manipulating the DOM directly and keep the state of an application
in sync with the UI easily. Additionally, they provide the ability to create components that can be reused when they have similar functionality with minor differences, avoiding duplication which would require multiple changes whenever the structure of a component which is reused in multiple places needs to be updated.

When working with DOM manipulation libraries like jQuery, the data of an application is generally kept in the DOM itself, often as class names or `data` attributes. Manipulating the DOM to update the UI involves many extra steps and can introduce subtle bugs over time. Keeping the state separate and letting a framework handle the UI updates when the state changes reduces cognitive load. Saying you want the UI to look a certain way when the state is a certain value is the declarative way of creating an application, instead of the imperative way of manually updating the UI to reflect the new state.


#### 小贴士


* The virtual DOM is a representation of the real DOM tree in the form of plain objects, which allows a library to write code as if the entire document is thrown away and rebuilt on each change, while the real DOM only updates what needs to be changed. Comparing the new virtual DOM against the previous one leads to high efficiency as changing real DOM nodes is costly compared to recalculating the virtual DOM.
* JSX is an extension to JavaScript that provides XML-like syntax to create virtual DOM objects which is transformed to function calls by a transpiler. It simplifies control flow (if statements/ternary expressions) compared to tagged template literals.


##### 附加链接


* [Virtual DOM in Hyperapp](https://github.com/hyperapp/hyperapp#view)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是‘严格模式’，它带来哪些关键性的好处？

<details>
<summary>查看答案</summary>

在 JavaScript 源文件开头包含 `'use strict'` 会开启严格模式，它会强制解析和错误处理更严格。它被认为是一个好的体验和提供很多好处，例如：

* 由于排除了无声的错误，所以更容易调试
* 不允许变量重新定义
* 防止意外的全局变量
* 相比非严格模式下的同一代码，提高了执行性能
* 简化了 `eval()` 和 `arguments`
* 帮助 JavaScript 更安全


#### 小贴士


* 排除 `this` ，当 `this` 引用 `null` 或 `undefined` 会抛出错误
* 无效使用 `delete` 会抛出一个错误
* 禁止在 ECMAScript 未来版本定义一些语法


##### 附加链接


* [MDN docs for strict mode](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是虚拟 DOM，为何库/框架都在用它？

<details>
<summary>查看答案</summary>

The virtual DOM (VDOM) is a representation of the real DOM in the form of plain JavaScript objects. These objects have properties to describe the real DOM nodes they represent: the node name, its attributes, and child nodes.

```html
<div class="counter">
  <h1>0</h1>
  <button>-</button>
  <button>+</button>
</div>
```

The above markup's virtual DOM representation might look like this:

```js
{
  nodeName: "div",
  attributes: { class: "counter" },
  children: [
    {
      nodeName: "h1",
      attributes: {},
      children: [0]
    },
    {
      nodeName: "button",
      attributes: {},
      children: ["-"]
    },
    {
      nodeName: "button",
      attributes: {},
      children: ["+"]
    }
  ]
}
```

The library/framework uses the virtual DOM as a means to improve performance. When the state of an application changes, the real DOM needs to be updated to reflect it. However, changing real DOM nodes is costly compared to recalculating the virtual DOM. The previous virtual DOM can be compared to the new virtual DOM very quickly in comparison.

Once the changes between the old VDOM and new VDOM have been calculated by the diffing engine of the framework, the real DOM can be patched efficiently in the least time possible to match the new state of the application.


#### 小贴士


* Why accessing the DOM can be so costly.


##### 附加链接


* [The difference between Virtual DOM and DOM](http://reactkungfu.com/2015/10/the-difference-between-virtual-dom-and-dom/)

</details>

<br>[⬆ 返回顶部](#目录)


## React
### Element 和 Component 有什么区别？

<details>
<summary>查看答案</summary>

一个元素是一个纯对象，用来描述你想在屏幕上显示的 DOM 节点或其他组件。元素在它们的属性上可以包含其他元素。创建一个 React 元素很简单。一旦元素被创建，它就永远不会突变了

另一方面，一个组件有很多中不同的声明方式。它可以通过一个含有 `render()` 方法的类定义（类组件），也可以通过一个函数定义（函数式组件）。组件接受 `props` 作为输入，并且返回一个元素树作为输出


#### 小贴士


* 元素（Element）是一个不可变，描述你想渲染的 DOM 节点或其他组件的纯对象
* 组件（Component） 可以是类形式的，也可以是函数形式的，接受 `props` 作为输入，并且返回一个元素树作为输出


##### 附加链接


* [React docs on Rendering Elements](https://reactjs.org/docs/rendering-elements.html)
* [React docs on Components and Props](https://reactjs.org/docs/components-and-props.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 中，状态提升是什么意思？

<details>
<summary>查看答案</summary>

When several components need to share the same data, then it is recommended to lift the shared state up to their closest common ancestor. For example, if two child components share the same data, it is recommended to move the shared state to parent instead of maintaining the local state in both child components.


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 里，如何写注释？

<details>
<summary>查看答案</summary>

React 的注释和 Javascript 的多行注释很相似，它是用大括号包裹起来的。在 JSX 中这么使用：

```jsx
render() => (<div>
  {/* 单行注释 */}
  Hey {user}, write cool comments
  {/* 多行注释 */}
</div>)
```

<!-- tags: (react) -->

<!-- expertise: (0) -->


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)


### `setState` 将回调函数作为参数目的是什么？

<details>
<summary>查看答案</summary>

在 `setState` 设置完成和组件渲染完时，会调用这个回调函数。因为 `setState` 是一步操作，所以这个回调函数可以用来做任何 post 操作

```jsx
setState({ name: "sudheer" }, () =>
  console.log("The name has updated and component re-rendered")
)
```


#### 小贴士


* 这个回调函数在 `setState` 完成后被调用，而且可以用于任何 post 操作
* 更推荐使用生命周期的方法，而不是这个回调函数


##### 附加链接


* [React docs on `setState`](https://reactjs.org/docs/react-component.html#setstate)

</details>

<br>[⬆ 返回顶部](#目录)

### React 为什么用 `className` 属性代替 `class`?

<details>
<summary>查看答案</summary>

`class` 是 JavaScript 的保留关键字，而 JSX 是 JavaScript 的扩展，这就是为何使用 `className` 代替 `class` 的主要原因 

```jsx
render() {
  return <span className="tooltip">tooltip</span>
}
```


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### React 和 HTML 对事件处理的区别？

<details>
<summary>查看答案</summary>

一些关键的区别：

* 在 HTML 中，事件名应该是小写，然而在 React 中，遵循驼峰写法约定

```html
<!-- HTML -->
<button onclick="handleClick()">Click me</button>
```

```jsx
/* React */
<button onClick="handleClick()">Click me</button>
```

* 在 HTML 中，返回 `false` 可以阻止默认行为发生，然而在 React 中，必须显示调用 `preventDefault`才能阻止默认行为

```html
<!-- HTML -->
<a href="#" onclick="console.log('The link was clicked.'); return false">Click me</a>
```

```jsx
/* React */
function handleClick(e) {
  e.preventDefault()
  console.log("The link was clicked.")
}
```


#### 小贴士


* HTML 事件名通常小写，而 React 事件名使用驼峰写法


##### 附加链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是内联条件表达式？

<details>
<summary>查看答案</summary>

你可以使用 `if` 语句或三元表达式有条件的渲染表达式。除了这些方法之外，你也可以在 JSX 中使用大括号内嵌任何表达式，然后后面跟上逻辑与运算符 `&&`

```jsx
;<h1>你好！</h1>
{
  messages.length > 0 && <h2>你有 {messages.length} 条未读消息</h2>
}
```


#### 小贴士




##### 附加链接


* [React docs on Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 key ，在 lists 中使用的好处是什么？

<details>
<summary>查看答案</summary>

Keys are a special string attribute that helps React identify which items have been changed, added or removed. They are used when rendering array elements to give them a stable indentity. Each element's key must be unique (e.g. IDs from the data or indexes as a last resort).

```jsx
const todoItems = todos.map(todo => <li key={todo.id}>{todo.text}</li>)
```

* Using indexes as keys is not recommended if the order of items may change, as it might negatively impact performance and may cause issues with component state.
* If you extract list items as a separate component then apply keys on the list component instead of the `<li>` tag.


#### 小贴士


* Keys give elements in a collection a stable identity and help React identify changes.
* You should avoid using indexes as keys if the order of items may change.
* You should lift the key up to the component, instead of the `<li>` element, if you extract list items as components.


##### 附加链接


* [React docs on Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)

</details>

<br>[⬆ 返回顶部](#目录)

### React 里的生命周期有哪些？

<details>
<summary>查看答案</summary>

`getDerivedStateFromProps`: Executed before rendering on the initial mount and all component updates. Used to update the state based on changes in props over time. Has rare use cases, like tracking component animations during the lifecycle. There are only few cases where this makes sense to use over other lifecycle methods. It expects to return an object that will be the the new state, or null to update nothing. This method does not have access to the component instance either.

`componentDidMount`: Executed after first rendering and here all AJAX requests, DOM or state updates, and set up eventListeners should occur.

`shouldComponentUpdate`: Determines if the component will be updated or not. By default, it returns true. If you are sure that the component doesn't need to render after state or props are updated, you can return a false value. It is a great place to improve performance as it allows you to prevent a rerender if component receives new prop.

`getSnapshotBeforeUpdate`: Invoked right after a component render happens because of an update, before `componentDidUpdate`. Any value returned from this method will be passed to `componentDidUpdate`.

`componentDidUpdate`: Mostly it is used to update the DOM in response to prop or state changes.

`componentWillUnmount`: It will be used to cancel any outgoing network requests, or remove all event listeners associated with the component.

`componentDidCatch`: Used in error boundaries, which are components that implement this method. It allows the component to catch JavaScript errors anywhere in the _child_ component tree (below this component), log errors, and display a UI with error information.


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### React 组件中，生命周期的各个阶段是什么？

<details>
<summary>查看答案</summary>

组件的生命周期有 4 个不同的阶段：

**初始化阶段**：在这个阶段，react 组件准备初始化 state 和设置默认 props

**挂载阶段**：react 组件准备挂载到浏览器的 DOM 上。这个阶段包含 `getDerivedStateFromProps` 和 `componentDidMount` 生命周期方法

**更新阶段**：在这个阶段，组件以两种方式进行更新（设置新的 props 和更新 state）。这个阶段包含 `getDerivedStateFromProps`、`shouldComponentUpdate`、`getSnapshotBeforeUpdate` 和 `componentDidUpdate` 生命周期方法

**卸载阶段**：在最后一个阶段，组件已经不再需要，并且从浏览器 DOM 上卸载掉。这个阶段包括 `componentWillUnmount` 生命周期方法

**错误处理阶段**：在这个阶段，当渲染过程发生错误时，或任何一个子组件的构造函数发生错误，组件会调用这个生命周期方法。这个阶段包括 `componentDidCatch` 生命周期方法

<img alt="lifecycle phases" src="https://pbs.twimg.com/media/DZ-97vzW4AAbcZj.jpg:large" style="width: 100%"/>


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 你是怎么给事件处理或回调函数传参的？

<details>
<summary>查看答案</summary>

你可以通过箭头函数包裹一个事件处理句柄然后传参，等价于调用 `bind` 函数：

```jsx
<button onClick={() => this.handleClick(id)} />
<button onClick={this.handleClick.bind(this, id)} />
```


#### 小贴士




##### 附加链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 回调引用 refs 和 findDOMNode 哪个更推荐使用？

<details>
<summary>查看答案</summary>

Callback refs are preferred over the `findDOMNode()` API, due to the fact that `findDOMNode()` prevents certain improvements in React in the future.

```jsx
/* Legacy approach using findDOMNode() */
class MyComponent extends Component {
  componentDidMount() {
    findDOMNode(this).scrollIntoView()
  }

  render() {
    return <div />
  }
}

/* Recommended approach using callback refs */
class MyComponent extends Component {
  componentDidMount() {
    this.node.scrollIntoView()
  }

  render() {
    return <div ref={node => (this.node = node)} />
  }
}
```


#### 小贴士


* Callback refs are preferred over `findDOMNode()`.


##### 附加链接


* [React docs on Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html#exposing-dom-refs-to-parent-components)

</details>

<br>[⬆ 返回顶部](#目录)

### React 组件中的属性（prop）`children` 是什么？

<details>
<summary>查看答案</summary>

`Children` 是一个属性（`this.prop.children`），允许组件作为数据传给其他组件。React API 提供了许多处理这个属性的方法，例如：`React.Children.map`、`React.Children.forEach`、`React.Children.count`、`React.Children.only` 和 `React.Children.toArray`。下面是一个简单的使用 `children` 属性例子：

```jsx
var MyDiv = React.createClass({
  render: function() {
    return <div>{this.props.children}</div>
  }
})

ReactDOM.render(
  <MyDiv>
    <span>Hello</span>
    <span>World</span>
  </MyDiv>,
  node
)
```


#### 小贴士


* `Children` 是一个属性，允许组件作为数据传给其他组件
* React API 提供了方法处理这个属性


##### 附加链接


* [React docs on Children](https://reactjs.org/docs/jsx-in-depth.html#children-in-jsx)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 中，什么是 context？

<details>
<summary>查看答案</summary>

Context provides a way to pass data through the component tree without having to pass props down manually at every level. For example, authenticated user, locale preference, UI theme need to be accessed in the application by many components.

```jsx
const { Provider, Consumer } = React.createContext(defaultValue)
```


#### 小贴士


* Context provides a way to pass data through a tree of React components, without having to manually pass props.
* Context is designed to share data that is considered _global_ for a tree of React components.


##### 附加链接


* [React docs on Context](https://reactjs.org/docs/context.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 中，错误边界是什么？

<details>
<summary>查看答案</summary>

错误边界是 React 组件捕获子组件树抛出的任何错误，记录这些错误，并且用一个回退的 UI 展示，而不是这个组件树崩溃

一个类形式的组件如果定义了一个新的生命周期方法 `componentDidCatch`，那么它就成为了一个错误边界

```jsx
class ErrorBoundary extends React.Component {
  constructor(props) {
    super(props)
    this.state = { hasError: false }
  }

  componentDidCatch(error, info) {
    // 展示回退 UI 
    this.setState({ hasError: true })
    // 你也可以把错误日志报告给服务器 
    logErrorToMyService(error, info)
  }

  render() {
    if (this.state.hasError) {
      // 你可以渲染任何自定义的回退 UI 
      return <h1>Something went wrong.</h1>
    }
    return this.props.children
  }
}
```


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 中，什么是 `fragments`？

<details>
<summary>查看答案</summary>

Fragments 允许 React 组件返回没有包裹层多个元素，按组把子元素加入 DOM（不增加额外元素）。Fragments 提供更好的表现，更低内存使用，一个更加干净的 DOM 可以帮助处理特定的 CSS 机制（例如，tables，Flexbox 和 Grid）

```jsx
render() {
  return (
    <React.Fragment>
      <ChildA />
      <ChildB />
      <ChildC />
    </React.Fragment>
  );
}

// 缩写语法（新版本支持 React v16.2.0+）：
render() {
  return (
    <>
      <ChildA />
      <ChildB />
      <ChildC />
    </>
  );
}
```


#### 小贴士


* Fragments 组件让你在一个 render() 方法中返回多个元素，而不用创造一个额外的 DOM 元素

##### 附加链接


* [React docs on Fragments](https://reactjs.org/docs/fragments.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是高阶组件？

<details>
<summary>查看答案</summary>

高阶组件（HOC）是指接受一个组件作为参数，然后返回一个新组件的函数。它是一种 React 合成性质衍生来的模式。高阶组件像 **纯组件** ，因为它接受任何动态提供的子组件，但是它不会修改或拷贝输入组件的任何行为

```jsx
const EnhancedComponent = higherOrderComponent(WrappedComponent)
```


#### 小贴士


* 它可用于 state 抽象和操控，props 的操控，提高渲染，等等


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 类方式定义的组件中，你如何保证方法得到的 ‘this’ 是正确的？

<details>
<summary>查看答案</summary>

* In JavaScript classes, the methods are not bound by default. This means that their `this` context can be changed (in the case of an event handler, to the element that is listening to the event) and will not refer to the component instance. To solve this, `Function.prototype.bind()` can be used to enforce the `this` context as the component instance.

```jsx
constructor(props) {
  super(props);
  this.handleClick = this.handleClick.bind(this);
}

handleClick() {
  // Perform some logic
}
```

* The `bind` approach can be verbose and requires defining a `constructor`, so the new public class fields syntax is generally preferred:

```jsx
handleClick = () => {
  console.log('this is:', this);
}

render() {
  return (
    <button onClick={this.handleClick}>
      Click me
    </button>
  );
}
```

* You can also use an inline arrow function, because lexical `this` (referring to the component instance) is preserved:

```jsx
<button onClick={e => this.handleClick(e)}>Click me</button>
```

Note that extra re-rendering can occur using this technique because a new function reference is created on render, which gets passed down to child components and breaks `shouldComponentUpdate` / `PureComponent` shallow equality checks to prevent unnecessary re-renders. In cases where performance is important, it is preferred to go with `bind` in the constructor, or the public class fields syntax approach, because the function reference remains constant.


#### 小贴士


* You can either bind methods to the component instance context in the constructor, use public class fields syntax, or use inline arrow functions.


##### 附加链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)
* [React docs on Passing Functions to Components](https://reactjs.org/docs/faq-functions.html#how-do-i-bind-a-function-to-a-component-instance)

</details>

<br>[⬆ 返回顶部](#目录)

### ReactJS 中，‘portals’（传送门） 是什么？

<details>
<summary>查看答案</summary>

Portal are the recommended way to render children into a DOM node that exists outside the DOM hierarchy of the parent component.

```jsx
ReactDOM.createPortal(child, container)
```

The first argument (`child`) is any renderable React child, such as an element, string, or fragment. The second argument (`container`) is a DOM element.


#### 小贴士




##### 附加链接


* [React docs on Portals](https://reactjs.org/docs/portals.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 中，如何校验 prop？

<details>
<summary>查看答案</summary>

When the application is running in development mode, React will automatically check for all props that we set on components to make sure they are the correct data type. For incorrect data type, it will generate warning messages in the console for development mode whereas it is disabled in production mode due to performance impact. The required prop is defined with `isRequired`.

The set of predefined prop types are the following:

-`PropTypes.string` -`PropTypes.number` -`PropTypes.func` -`PropTypes.node` -`PropTypes.bool`

For example, we define propTypes for component as below:

```jsx
import PropTypes from 'prop-types';

class User extends React.Component {
  render() {
    return (
      <h1>Welcome, {this.props.name}</h1>
      <h2>Age, {this.props.age}
    );
  }
}

User.propTypes = {
  name: PropTypes.string.isRequired,
  age: PropTypes.number.isRequired
};
```


#### 小贴士


* We can define custom `PropTypes`
* Using `PropTypes` is not mandatory. However, it is a good practice


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 refs，什么时候用它们？

<details>
<summary>查看答案</summary>

Refs provide a way to access DOM nodes or React elements created in the render method. Refs should be used sparringly, but there are some good use cases for refs, such as:

* Managing focus, text selection, or media playback.
* Triggering imperative animations.
* Integrating with third-party DOM libraries.

Refs are created using `React.createRef()` method and attached to React elements via the `ref` attribute. In order to use refs throughout the component, just assign the `ref` to the instance property within the constructor:

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props)
    this.myRef = React.createRef()
  }
  render() {
    return <div ref={this.myRef} />
  }
}
```

Refs can also be used in functional components with the help of closures.


#### 小贴士


* Refs are used to return a reference to an element.
* Refs shouldn't be overused.
* You can create a ref using `React.createRef()` and attach to Reactelements via the `ref` attribute.


##### 附加链接


* [React docs on Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是有状态组件？

<details>
<summary>查看答案</summary>

一个有状态组件是一个行为依赖它状态（state）的组件。有状态组件总是类组件，并且在构造函数中初始化它的状态（state）

```jsx
class App extends Component {
  constructor(props) {
    super(props)
    this.state = { count: 0 }
  }
  render() {
    // ...
  }
}
```


#### 小贴士


* 有状态组件拥有他们所依赖的内部状态（state）
* 有状态组件总是类组件
* 有状态组件拥有他们在构造函数初始化的状态（state）


##### 附加链接


* [React docs on State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是无状态组件？

<details>
<summary>查看答案</summary>

一个无状态组件是一个行为不依赖它状态（state）的组件。无状态组件可以是类组件，也可以是函数式组件。无状态的函数式组件更易维护和测试，而且完全不用考虑 `this` 的问题。当不需要生命周期钩子时，更推荐函数式组件


#### 小贴士


* 无状态组件不依赖他们的状态
* 无状态组件可以是类组件也可以是函数式组件
* 无状态组件可以完全避免 `this` 关键字


##### 附加链接


* [React docs on State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

</details>

<br>[⬆ 返回顶部](#目录)


## HTML
###  图片里的 `alt` 属性是做什么的？

<details>
<summary>查看答案</summary>

如果用户看不到图像，`alt` 属性可以提供替代信息。`alt` 属性应该用于描述，而哪些仅仅是装饰目的图像，可以为空

#### 小贴士


* 装饰性的图像应该有一个空的 `alt` 属性
* web 爬虫可以通过 `alt` 属性理解图像的信息，因此认为它对于搜索引擎优化（SEO）非常重要
* 在 `alt` 末尾加 `.` 可以提高访问性


##### 附加链接


* [A good basis for accessibility](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML)

</details>

<br>[⬆ 返回顶部](#目录)

### 不采用缓存的目的是什么，你如何实现它？

<details>
<summary>查看答案</summary>

Browsers have a cache to temporarily store files on websites so they don't need to be re-downloaded again when switching between pages or reloading the same page. The server is set up to send headers that tell the browser to store the file for a given amount of time. This greatly increases website speed and preserves bandwidth.

However, it can cause problems when the website has been changed by developers because the user's cache still references old files. This can either leave them with old functionality or break a website if the cached CSS and JavaScript files are referencing elements that no longer exist, have moved or have been renamed.

Cache busting is the process of forcing the browser to download the new files. This is done by naming the file something different to the old file.

A common technique to force the browser to re-download the file is to append a query string to the end of the file.

* `src="js/script.js"` => `src="js/script.js?v=2"`

The browser considers it a different file but prevents the need to change the file name.


#### 小贴士




##### 附加链接


* [Strategies for cache-busting CSS](https://css-tricks.com/strategies-for-cache-busting-css/)

</details>

<br>[⬆ 返回顶部](#目录)

### 一个页面里是否可以包含多个 `<header>` 元素， `<footer>` 元素呢？

<details>
<summary>查看答案</summary>

Yes to both. The W3 documents state that the tags represent the header(`<header>`) and footer(`<footer>`) areas of their nearest ancestor "section". So not only can the page `<body>` contain a header and a footer, but so can every `<article>` and `<section>` element.


#### 小贴士


* W3 recommends having as many as you want, but only 1 of each for each "section" of your page, i.e. body, section etc.


##### 附加链接


* [StackOverflow Using header or footer tag twice](https://stackoverflow.com/questions/4837269/html5-using-header-or-footer-tag-twice?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa)

</details>

<br>[⬆ 返回顶部](#目录)

### 简明的阐述下 HTML5 语义标签 `<header>`，`<article>`，`<section>`，`<footer>` 的用法

<details>
<summary>查看答案</summary>

* `<header>` is used to contain introductory and navigational information about a section of the page. This can include the section heading, the author’s name, time and date of publication, table of contents, or other navigational information.

* `<article>` is meant to house a self-contained composition that can logically be independently recreated outside of the page without losing its meaning. Individual blog posts or news stories are good examples.

* `<section>` is a flexible container for holding content that shares a common informational theme or purpose.

* `<footer>` is used to hold information that should appear at the end of a section of content and contain additional information about the section. Author’s name, copyright information, and related links are typical examples of such content.


#### 小贴士


* Other semantic elements are `<form>` and `<table>`


##### 附加链接


* [HTML 5 Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)

</details>

<br>[⬆ 返回顶部](#目录)

### `<script>` 标签的 `defer` 和 `async` 是什么？

<details>
<summary>查看答案</summary>

If neither attribute is present, the script is downloaded and executed synchronously, and will halt parsing of the document until it has finished executing (default behavior). Scripts are downloaded and executed in the order
they are encountered.

The `defer` attribute downloads the script while the document is still parsing but waits until the document has finished parsing before executing it, equivalent to executing inside a `DOMContentLoaded` event listener. `defer` scripts will execute in order.

The `async` attribute downloads the script during parsing the document but will pause the parser to execute the script before it has fully finished parsing. `async` scripts will not necessarily execute in order.

Note: both attributes must only be used if the script has a `src` attribute (i.e. not an inline script).

```html
<script src="myscript.js"></script>
<script src="myscript.js" defer></script>
<script src="myscript.js" async></script>
```


#### 小贴士


* Placing a `defer` script in the `<head>` allows the browser to download the script while the page is still parsing, and is therefore a better option than placing the script before the end of the body.
* If the scripts rely on each other, use `defer`.
* If the script is independent, use `async`.
* Use `defer` if the DOM must be ready and the contents are not placed within a `DOMContentLoaded` listener.


##### 附加链接


* [async vs defer attributes](http://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 DOM？

<details>
<summary>查看答案</summary>

The DOM (Document Object Model) is a cross-platform API that treats HTML and XML documents as a tree structure consisting of nodes. These nodes (such as elements and text nodes) are objects that can be programmatically manipulated and any visible changes made to them are reflected live in the document. In a browser, this API is available to JavaScript where DOM nodes can be manipulated to change their styles, contents, placement in the document, or interacted with through event listeners.


#### 小贴士


* The DOM was designed to be independent of any particular programming language, making the structural representation of the document available from a single, consistent API.
* The DOM is constructed progressively in the browser as a page loads, which is why scripts are often placed at the bottom of a page, in the `<head>` with a `defer` attribute, or inside a `DOMContentLoaded` event listener. Scripts that manipulate DOM nodes should be run after the DOM has been constructed to avoid errors.
* `document.getElementById()` and `document.querySelector()` are common functions for selecting DOM nodes.
* Setting the `innerHTML` property to a new value runs the string through the HTML parser, offering an easy way to append dynamic HTML content to a node.


##### 附加链接


* [MDN docs for DOM](https://developer.mozilla.org/en-US/docs/DOM)

</details>

<br>[⬆ 返回顶部](#目录)

### 讨论下 HTML 规范和浏览器实现之间的区别？

<details>
<summary>查看答案</summary>

HTML specifications such as `HTML5` define a set of rules that a document must adhere to in order to be “valid” according to that specification. In addition, a specification provides instructions on how a browser must interpret and render such a document.

A browser is said to “support” a specification if it handles valid documents according to the rules of the specification. As of yet, no browser supports all aspects of the `HTML5` specification (although all of the major browser support most of it), and as a result, it is necessary for the developer to confirm whether the aspect they are making use of will be supported by all of the browsers on which they hope to display their content. This is why cross-browser support continues to be a headache for developers, despite the improved specificiations.


#### 小贴士


* `HTML5` defines some rules to follow for an invalid `HTML5` document (i.e., one that contains syntactical errors)
* However, invalid documents may contain anything, so it's impossible for the specification to handle all possibilities comprehensively.
* Thus, many decisions about how to handle malformed documents are left up to the browser.


##### 附加链接


* [HTML 5.2 WWW Specifications](https://www.w3.org/TR/html52/)

</details>

<br>[⬆ 返回顶部](#目录)

### 相比 HTML，XHTML 有哪些不同？

<details>
<summary>查看答案</summary>

有一些关键区别：

* 一个 XHTML 元素必须要有一个 XHTML `<DOCTYPE>`
* 属性值必须用引号包裹
* 禁止属性简写（例如，`checked="checked"` 不能简写为 `checked`）
* 元素必须正确的被嵌套
* 元素必须闭合
* 特殊字符必须被转义


#### 小贴士


* 任何被标签都是自闭合
* 标签和属性区分大小写，通常小写


##### 附加链接


* [W3Schools docs for HTML and XHTML](https://www.w3schools.com/html/html_xhtml.asp)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么时候和为什么使用 rel="noopener" 属性？

<details>
<summary>查看答案</summary>

The `rel="noopener"` is an attribute used in `<a>` elements (hyperlinks). It prevents pages from having a `window.opener` property, which would otherwise point to the page from where the link was opened and would allow the page opened from the hyperlink to manipulate the page where the hyperlink is.


#### 小贴士


* `rel="noopener"` is applied to hyperlinks.
* `rel="noopener"` prevents opened links from manipulating the source page.


##### 附加链接


* [Open external anchors using rel="noopener"](https://developers.google.com/web/tools/lighthouse/audits/noopener)
* [About rel="noopener"](https://mathiasbynens.github.io/rel-noopener/)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 HTML5 Web Storage，解释下 localStorage 和 sessionStorage？

<details>
<summary>查看答案</summary>

随着 HTML5 的发展，web 页面拥有了在用户浏览器存储本地数据的能力
数据是以键值对的形式存储的，而且 web 页面只能访问它自己存储的数据

**从生命周期角度看，`localStorage` 和 `sessionStorage` 的区别：**

* 通过 `localStorage` 存储的数据是永久的：它永远不会过期，而且会一直保留在用户电脑中，直到 web app 删除或用户通过浏览器删除
* `sessionStorage` 存储的数据与顶级 window 或浏览器 tab 拥有一样的生命周期。当 tab 被永久关闭后，通过 `sessionStorage` 存储的任何数据就会被删除

**从存储范围角度看，`localStorage` 和 `sessionStorage` 的区别：**
这两种存储方式均遵循浏览器同源策略，因此不同的域的数据永远不可共享

* `sessionStorage` 也作为每个 window 为基础。两个同域的浏览器 tab 具有独立的 `sessionStorage`  数据
* 和 `localStorage` 不同，在打开的不同的 tab 中，即使是同域相同的脚本也不能访问彼此的 `sessionStorage` 


#### 小贴士


* 较早时候，存储是用 cookie 做的
* 这个存储限制（至少 5MB）远比 cookie 大而且更快
* 数据永远不会传输到服务器，只能在客户端的特别要求下使用


##### 附加链接


* [W3Schools HTML5 Webstorage](https://www.w3schools.com/html/html5_webstorage.asp)

</details>

<br>[⬆ 返回顶部](#目录)


## CSS
### 什么是 CSS BEM？

<details>
<summary>查看答案</summary>

The BEM methodology is a naming convention for CSS classes in order to keep CSS more maintainable by defining namespaces to solve scoping issues. BEM stands for Block Element Modifier which is an explanation for its structure. A Block is a standalone component that is reusable across projects and acts as a "namespace" for sub components (Elements). Modifiers are used as flags when a Block or Element is in a certain state or is different in structure or style.

```css
/* block component */
.block {
}

/* element */
.block__element {
}

/* modifier */
.block__element--modifier {
}
```

Here is an example with the class names on markup:

```html
<nav class="navbar">
  <a href="/" class="navbar__link navbar__link--active"></a>
  <a href="/" class="navbar__link"></a>
  <a href="/" class="navbar__link"></a>
</nav>
```

In this case, `navbar` is the Block, `navbar__link` is an Element that makes no sense outside of the `navbar` component, and `navbar__link--active` is a Modifier that indicates a different state for the `navbar__link` Element.

Since Modifiers are verbose, many opt to use `is-*` flags instead as modifiers.

```html
<a href="/" class="navbar__link is-active"></a>
```

These must be chained to the Element and never alone however, or there will be scope issues.

```css
.navbar__link.is-active {
}
```


#### 小贴士


* Alternative solutions to scope issues like CSS-in-JS


##### 附加链接


* [Writing clean and maintainable CSS](https://hackernoon.com/writing-clean-and-maintainable-css-using-bem-methodology-1dcbf810a664)

</details>

<br>[⬆ 返回顶部](#目录)

### 用 CSS 预处理的优势是什么？

<details>
<summary>查看答案</summary>

CSS preprocessors add useful functionality that native CSS does not have, and generally make CSS neater and more maintainable by enabling DRY (Don't Repeat Yourself) principles. Their terse syntax for nested selectors cuts down on repeated code. They provide variables for consistent theming (however, CSS variables have largely replaced this functionality) and additional tools like color functions (`lighten`, `darken`, `transparentize`, etc), mixins, and loops that make CSS more like a real programming language and gives the developer more power to generate complex CSS.


#### 小贴士


* They allow us to write more maintainable and scalable CSS
* Some disadvantages of using CSS preprocessors (setup, re-compilation time can be slow etc.)


##### 附加链接


* [CSS Preprocessors](https://medium.com/@garyfagan/css-preprocessors-6f226fa16f27)

</details>

<br>[⬆ 返回顶部](#目录)

### 使用 flexbox，创建一个 3 列布局，每一列取容器的百分之 col-{n}/12

```html
<div class="row">
  <div class="col-2"></div>
  <div class="col-7"></div>
  <div class="col-3"></div>
</div>
```

<details>
<summary>查看答案</summary>

给类名为 `.row` 的父元素设置 `display:flex;`，并且使用 `flex-grow` 属性的缩写 `flex` 设置与列所给类名一致的比例值

```css
.row {
  display: flex;
}

.col-2 {
  flex: 2;
}

.col-7 {
  flex: 7;
}

.col-3 {
  flex: 3;
}
```


#### 小贴士




##### 附加链接


* [MDN docs for basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
* [A complete guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

</details>

<br>[⬆ 返回顶部](#目录)

### 你能说出 `@media` 属性的四种类型吗？

<details>
<summary>查看答案</summary>

* `all`，适用于所有媒体设备
* `print`，仅适用于打印机
* `screen`，仅适用于屏幕设备（台式电脑、平板电脑、移动设备等）
* `speech`，仅适用于屏幕阅读器


#### 小贴士




##### 附加链接


* [MDN docs for `@media` rule](https://developer.mozilla.org/en-US/docs/Web/CSS/@media)
* [MDN docs for using media queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)

</details>

<br>[⬆ 返回顶部](#目录)

### 简要阐述下 CSS 的盒模型，及各个组成部分？

<details>
<summary>查看答案</summary>

<!-- Your answer goes here. -->

`Content`: 盒子的最里面的部分，被内容填充（如：文本、图像、视频播放器）。它有 `content-box width` 和 `content-box height` 两个维度

`Padding`: 围绕内容的透明区域。它有 `padding-box width` 和 `padding-box height` 两个维度

`Border`: 围绕内边距（如果有的话）和内容的透明区域。它有 `border-box width` 和 `border-box height`  两个维度

_Margin_: 围绕着边框的盒子最外层区域。它将 DOM 元素之间分割开来。它有 `margin-box width` 和 `margin-box height` 两个维度

![alt text](https://www.washington.edu/accesscomputing/webd2/student/unit3/images/boxmodel.gif)


#### 小贴士


* 这个在前端面试是个很常见的问题，虽然看起来很容易，但关键是你对它很熟悉。
* 展示了一个对 DOM 更深刻的了解


##### 附加链接


* [W3School's CSS Box Model Page](https://www.w3schools.com/Css/css_boxmodel.asp)
* [Mozilla's Intro to the CSS Box Model](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model)

</details>

<br>[⬆ 返回顶部](#目录)

### em 和 rem 单位的区别？

<details>
<summary>查看答案</summary>

Both `em` and `rem` units are based on the `font-size` CSS property. The only difference is where they inherit their values from.

* `em` units inherit their value from the `font-size` of the parent element
* `rem` units inherit their value from the `font-size` of the root element (`html`)

In most browsers, the `font-size` of the root element is set to `16px` by default.


#### 小贴士


* Benefits of using `em` and `rem` units


##### 附加链接


* [CSS units for font-size: px | em | rem](https://medium.com/code-better/css-units-for-font-size-px-em-rem-79f7e592bb97)

</details>

<br>[⬆ 返回顶部](#目录)

### CSS 雪碧图的优势在哪里，如何使用？

<details>
<summary>查看答案</summary>

CSS sprites combine multiple images into one image, limiting the number of HTTP requests a browser has to make, thus improving load times. Even under the new HTTP/2 protocol, this remains true.

Under HTTP/1.1, at most one request is allowed per TCP connection. With HTTP/1.1, modern browsers open multiple parallel connections (between 2 to 8) but it is limited. With HTTP/2, all requests between the browser and the server are multiplexed on a single TCP connection. This means the cost of opening and closing multiple connections is mitigated, resulting in a better usage of the TCP connection and limits the impact of latency between the client and server. It could then become possible to load tens of images in parallel on the same TCP connection.

However, according to [benchmark results](https://blog.octo.com/en/http2-arrives-but-sprite-sets-aint-no-dead/), although HTTP/2 offers 50% improvement over HTTP/1.1, in most cases the sprite set is still faster to load than individual images.

To utilize a spritesheet in CSS, one would use certain properties, such as `background-image`, `background-position` and `background-size` to ultimately alter the `background` of an element.


#### 小贴士


* `background-image`, `background-position` and `background-size` can be used to utilize a spritesheet.


##### 附加链接


* [CSS Sprites explained by CSS Tricks](https://css-tricks.com/css-sprites/)

</details>

<br>[⬆ 返回顶部](#目录)

###  CSS 里通用兄弟选择器和相邻兄弟选择器的区别？

<details>
<summary>查看答案</summary>

The General Sibling Selector `~` selects all elements that are siblings of a specified element.

The following example selects all `<p>` elements that are siblings of `<div>` elements:

```css
div ~ p {
  background-color: blue;
}
```

The Adjacent Sibling Selector `+` selects all elements that are the adjacent siblings of a specified element.

The following example will select all `<p>` elements that are placed immediately after `<div>` elements:

```css
div + p {
  background-color: red;
}
```

##### 附加链接

* [W3School's CSS Combinators Page](https://www.w3schools.com/css/css_combinators.asp)
* [Mozilla's Combinators and groups of selectors page](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors)

<!-- tags: (css) -->

<!-- expertise: (2) -->


#### 小贴士




##### 附加链接


* [W3School's CSS Combinators Page](https://www.w3schools.com/css/css_combinators.asp)
* [Mozilla's Combinators and groups of selectors page](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors)

</details>

<br>[⬆ 返回顶部](#目录)

### 你能描述下 CSS 优先级是如何工作的？

<details>
<summary>查看答案</summary>

Assuming the browser has already determined the set of rules for an element, each rule is assigned a matrix of values, which correspond to the following from highest to lowest specificity:

* Inline rules (binary - 1 or 0)
* Number of id selectors
* Number of class, pseudo-class and attribute selectors
* Number of tags and pseudo-element selectors

When two selectors are compared, the comparison is made on a per-column basis (e.g. an id selector will always be higher than any amount of class selectors, as ids have higher specificity than classes). In cases of equal specificity between multiple rules, the rules that comes last in the page's style sheet is deemed more specific and therefore applied to the element.


#### 小贴士


* Specificity matrix: [inline, id, class/pseudo-class/attribute, tag/pseudo-element]
* In cases of equal specificity, last rule is applied


##### 附加链接


* [CSS Specificity](https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是聚焦环，正确的解决方案是什么？

<details>
<summary>查看答案</summary>

A focus ring is a visible outline given to focusable elements such as buttons and anchor tags. It varies depending on the vendor, but generally it appears as a blue outline around the element to indicate it is currently focused.

In the past, many people specified `outline: 0;` on the element to remove the focus ring. However, this causes accessibility issues for keyboard users because the focus state may not be clear. When not specified though, it causes an unappealing blue ring to appear around an element.

In recent times, frameworks like Bootstrap have opted to use a more appealing `box-shadow` outline to replace the default focus ring. However, this is still not ideal for mouse users.

The best solution is an upcoming pseudo-selector `:focus-visible` which can be polyfilled today with JavaScript. It will only show a focus ring if the user is using a keyboard and leave it hidden for mouse users. This keeps both aesthetics for mouse use and accessibility for keyboard use.


#### 小贴士




##### 附加链接


* [:focus-visible](https://css-tricks.com/focus-visible-and-backwards-compatibility/)

</details>

<br>[⬆ 返回顶部](#目录)


## Node
### NodeJS 错误优先回调的模式有什么优势？

```js
fs.readFile(filePath, function(err, data) {
  if (err) {
    // handle the error, the return is important here
    // so execution stops here
    return console.log(err)
  }
  // use the data object
  console.log(data)
})
```

<details>
<summary>查看答案</summary>

优势包括：

* 如果不需要引用它，就不用处理数据
* 拥有一致性的 API 适配更多情况
* 能够更容易使用回调模式，将使得代码维护变得更容易

正如你所见到的下面这个例子，如果没有发生错误回调将接收到的第一个参数是 `null`。然而，如果发生了错误，你可以创建一个 `Error` 对象，这将成为回调的唯一参数。这种回调函数使得用户更容易知道是否遇到了错误

这个惯例也叫做 _Node.js 错误约定_，并且这种回调实现成为 _错误优先回调_

```js
var isTrue = function(value, callback) {
  if (value === true) {
    callback(null, "Value was true.")
  } else {
    callback(new Error("Value is not true!"))
  }
}

var callback = function(error, retval) {
  if (error) {
    console.log(error)
    return
  }
  console.log(retval)
}

isTrue(false, callback)
isTrue(true, callback)

/*
  { stack: [Getter/Setter],
    arguments: undefined,
    type: undefined,
    message: 'Value is not true!' }
  Value was true.
*/
```


#### 小贴士


* 这只是一个约定。然而，你应该坚持使用这种写法


##### 附加链接


* [The Node.js Way Understanding Error-First Callbacks](http://fredkschott.com/post/2014/03/understanding-error-first-callbacks-in-node-js/)
* [What are the error conventions?](https://docs.nodejitsu.com/articles/errors/what-are-the-error-conventions)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 REST？

<details>
<summary>查看答案</summary>

REST (REpresentational State Transfer) is a software design pattern for network architecture. A RESTful web application exposes data in the form of information about its resources.

Generally, this concept is used in web applications to manage state. With most applications, there is a common theme of reading, creating, updating, and destroying data. Data is modularized into separate tables like `posts`, `users`, `comments`, and a RESTful API exposes access to this data with:

* An identifier for the resource. This is known as the endpoint or URL for the resource.
* The operation the server should perform on that resource in the form of an HTTP method or verb. The common HTTP methods are GET, POST, PUT, and DELETE.

Here is an example of the URL and HTTP method with a `posts` resource:

* Reading: `/posts/` => GET
* Creating: `/posts/new` => POST
* Updating: `/posts/:id` => PUT
* Destroying: `/posts/:id` => DELETE


#### 小贴士


* Alternatives to this pattern like GraphQL


##### 附加链接


*   ](https://medium.com/extend/what-is-rest-a-simple-explanation-for-beginners-part-1-introduction-b4a072f8740f)

</details>

<br>[⬆ 返回顶部](#目录)

### 你是怎么避免回调地狱的？

```js
getData(function(a) {
  getMoreData(a, function(b) {
    getMoreData(b, function(c) {
      getMoreData(c, function(d) {
        getMoreData(d, function(e) {
          // ...
        })
      })
    })
  })
})
```

<details>
<summary>查看答案</summary>

Refactoring the functions to return promises and using `async/await` is usually the best option. Instead of supplying the functions with callbacks that cause deep nesting, they return a promise that can be `await`ed and will be resolved once the data has arrived, allowing the next line of code to be evaluated in a sync-like fashion.

The above code can be restructured like so:

```js
async function asyncAwaitVersion() {
  const a = await getData()
  const b = await getMoreData(a)
  const c = await getMoreData(b)
  const d = await getMoreData(c)
  const e = await getMoreData(d)
  // ...
}
```

There are lots of ways to solve the issue of callback hells:

* Modularization: break callbacks into independent functions
* Use a control flow library, like async
* Use generators with Promises
* Use async/await (from v7 on)


#### 小贴士


* As an efficient JavaScript developer, you have to avoid the constantly growing indentation level, produce clean and readable code and be able to handle complex flows.


##### 附加链接


* [Avoiding Callback Hell in Node.js](http://stackabuse.com/avoiding-callback-hell-in-node-js/)
* [Asynchronous JavaScript: From Callback Hell to Async and Await](https://blog.hellojs.org/asynchronous-javascript-from-callback-hell-to-async-and-await-9b9ceb63c8e8)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 Nodejs 里的事件循环（event loop）？

<details>
<summary>查看答案</summary>

事件循环处理所有的异步回调。回调在一个循环按里队列排列，当其他代码执行时，并且收到响应时它们会一个接一个执行


#### 小贴士


* 事件循环允许 Node.js 执行非阻塞 I/O 操作，尽管 JavaScript 是单线程


##### 附加链接


* [Node.js docs on event loop, timers and process.nextTick()](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/)

</details>

<br>[⬆ 返回顶部](#目录)


## Security
### 什么是跨站脚本攻击（XSS），你是如何阻止它的？

<details>
<summary>查看答案</summary>

XSS refers to client-side code injection where the attacker injects malicious scripts into a legitimate website or web application. This is often achieved when the application does not validate user input and freely injects dynamic HTML content.

For example, a comment system will be at risk if it does not validate or escape user input. If the comment contains unescaped HTML, the comment can inject a `<script>` tag into the website that other users will execute against their knowledge.

* The malicious script has access to cookies which are often used to store session tokens. If an attacker can obtain a user’s session cookie, they can impersonate the user.
* The script can arbitrarily manipulate the DOM of the page the script is executing in, allowing the attacker to insert pieces of content that appear to be a real part of the website.
* The script can use AJAX to send HTTP requests with arbitrary content to arbitrary destinations.


#### 小贴士


* On the client, using `textContent` instead of `innerHTML` prevents the browser from running the string through the HTML parser which would execute scripts in it.
* On the server, escaping HTML tags will prevent the browser from parsing the user input as actual HTML and therefore won't execute the script.


##### 附加链接


* [Cross-Site Scripting Attack (XSS)](https://www.acunetix.com/websitesecurity/cross-site-scripting/)

</details>

<br>[⬆ 返回顶部](#目录)


## 协议

[MIT](LICENSE). Copyright (c) [Stefan Feješ](https://stefanfejes.com/).
