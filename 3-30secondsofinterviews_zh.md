<h1 align="center">
  面试 30 秒
</h1>

<h4 align="center">一个面试常用的问题精选集，帮助你准备下一次面试</h4>

> 原文 https://github.com/30-seconds/30-seconds-of-interviews

## 前言

面试是令人生畏的，它甚至可以让经验丰富的专家在压力之下大脑一片空白。复习和学习那些在面试中常遇到的问题（从社区中收集了被问到的和他们是如何应对的问题）。通过把实践和现实生活结合起来，你就可以从容的准备面对下一次面试


## [在线观看](https://30secondsofinterviews.org/)


## 目录


### JavaScript

<details>
<summary>查看内容</summary>

* [创建一个 `batches` 函数，返回一个食谱中可以被作为烹饪整批食材的最大数量](#create-a-function-batches-that-returns-the-maximum-number-of-whole-batches-that-can-be-cooked-from-a-recipe)
* [什么是大 O 标记法？](#what-is-big-o-notation)
* [创建一个和 `Function.prototype.bind` 功能一样的独立函数 `bind`](#create-a-standalone-function-bind-that-is-functionally-equivalent-to-the-method-functionprototypebind)
* [你是怎么避免回调地狱的？](#how-can-you-avoid-callback-hells)
* [`setState` 将回调函数作为参数目的是什么？](#what-is-the-purpose-of-callback-function-as-an-argument-of-setstate)
* [回调引用 refs 和 findDOMNode 哪个更推荐使用？](#which-is-the-preferred-option-between-callback-refs-and-finddomnode)
* [什么是回调，你可以举个例子吗？](#what-is-a-callback-can-you-show-an-example-using-one)
* [React 组件中的属性（prop）`children` 是什么？](#what-is-children-prop)
* [在 JavaScript 中，你是如何克隆一个对象的？](#how-do-you-clone-an-object-in-javascript)
* [什么是闭包，你可以举一个有用的例子吗？](#what-is-a-closure-can-you-give-a-useful-example-of-one)
* [在 JavaScript 中，你是如何比较两个对象的？](#how-do-you-compare-two-objects-in-javascript)
* [在 React 中，什么是 `context`？](#what-is-context)
* [什么是 `CORS`？](#what-is-cors)
* [什么是 `DOM`？](#what-is-the-dom)
* [`==` 和 `===` 相等运算符有什么区别？](#what-is-the-difference-between-the-equality-operators--and-)
* [在 React 中，`Element` 和 `Component` 有什么区别？](#what-is-the-difference-between-element-and-component)
* [什么是事件委托，为什么它是有用的，你可以举个例子说明如何使用它？](#what-is-event-delegation-and-why-is-it-useful-can-you-show-an-example-of-how-to-use-it)
* [什么是事件驱动编程？](#what-is-event-driven-programming)
* [在 JavaScript 中，声明和表达式的区别？](#what-is-the-difference-between-an-expression-and-a-statement-in-javascript)
* [在 JavaScript 中，什么是真值（truthy），假值（falsy）?](#what-are-truthy-and-falsy-values-in-javascript)
* [生成一个包含的 n 项斐波那契数列元素的数组](#generate-an-array-containing-the-fibonacci-sequence-up-until-the-nth-term)
* [`0.1 + 0.2 === 0.3` 表达式的值是？](#what-does-01--02--03-evaluate-to)
* [数组 `map()` 和 `forEach()` 方法的区别？](#what-is-the-difference-between-the-array-methods-map-and-foreach)
* [在 React 中，什么是 `fragments`？](#what-are-fragments)
* [什么是函数式编程？](#what-is-functional-programming)
* [下面的例子中，`console.log` 会打印出什么？](#what-will-the-console-log-in-this-example)
* [在 JavaScript 中，声明提升是如何工作的？](#how-does-hoisting-work-in-javascript)
* [HTML 和 React 中的事件处理有什么区别？](#what-is-the-difference-between-html-and-react-event-handling)
* [为何将 JavaScript 源文件里的整个内容用匿名函数包裹起来？](#what-is-the-reason-for-wrapping-the-entire-contents-of-a-javascript-source-file-in-a-function-that-is-immediately-invoked)
* [阐释下命令式编程和声明式编程的区别？](#explain-the-differences-between-imperative-and-declarative-programming)
* [什么是内联条件表达式？](#what-is-inline-conditional-expressions)
* [什么是 key ，在 lists 中使用的好处是什么？](#what-is-a-key-what-are-the-benefits-of-using-it-in-lists)
* [词法作用域和动态作用域的区别？](#what-is-the-difference-between-lexical-scoping-and-dynamic-scoping)
* [创建一个函数，用 ‘#’ 符号遮住字符串（除最后4个字符之外）](#create-a-function-that-masks-a-string-of-characters-with--except-for-the-last-four-4-characters)
* [什么是缓存代理模式（memoization）？](#what-is-memoization)
* [在 React 类方式定义的组件中，你如何保证方法得到的 ‘this’ 是正确的？](#how-do-you-ensure-methods-have-the-correct-this-context-in-react-component-classes)
* [什么是 MIME 类型，有什么作用？](#what-is-a-mime-type-and-what-is-it-used-for)
* [对比下可变与不可变值，可变与不可变方法](#contrast-mutable-and-immutable-values-and-mutating-vs-non-mutating-methods)
* [在 JavaScript 中，哪个值不等于它自己？](#what-is-the-only-value-not-equal-to-itself-in-javascript)
* [NodeJS 错误优先回调的模式有什么优势？](#nodejs-often-uses-a-callback-pattern-where-if-an-error-is-encountered-during-execution-this-error-is-passed-as-the-first-argument-to-the-callback-what-are-the-advantages-of-this-pattern)
* [什么是 Nodejs 里的事件循环（event loop）？](#what-is-the-event-loop-in-nodejs)
* [`null`  和 `undefined` 有何不同？](#what-is-the-difference-between-null-and-undefined)
* [描述下创建对象方式的不同，哪种方式更推荐？](#describe-the-different-ways-to-create-an-object-when-should-certain-ways-be-preferred-over-others)
* [形参和实参的区别？](#what-is-the-difference-between-a-parameter-and-an-argument)
* [JavaScript 里是通过值传递还是引用传递？](#does-javascript-pass-by-value-or-by-reference)
* [你是怎么给事件处理/回调函数传参的？](#how-do-you-pass-an-argument-to-an-event-handler-or-callback)
* [创建一个管道函数，返回一个接受一个参数从左到右执行的合成函数](#create-a-function-pipe-that-performs-left-to-right-function-composition-by-returning-a-function-that-accepts-one-argument)
* [ReactJS 中，‘portals’（传送门） 是什么？](#what-are-portals-in-reactjs)
* [`i++`  和 `++i` 有什么不同？](#what-is-the-difference-between-the-postfix-i-and-prefix-i-increment-operators)
* [Promise 可以变成哪些状态？](#in-which-states-can-a-promise-be)
* [什么是 Promises？](#what-are-promises)
* [原型继承和经典继承方式有何不同？](#how-does-prototypal-inheritance-differ-from-classical-inheritance)
* [什么是纯函数？](#what-is-a-pure-function)
* [什么是递归，什么时候它是有用的？](#what-is-recursion-and-when-is-it-useful)
* [下面的代码会输出什么？](#what-is-the-output-of-the-following-code)
* [什么是 refs，什么时候用它们？](#what-are-refs-when-should-they-be-used)
* [下面的函数会返回什么？](#what-does-the-following-function-return)
* [JavaScript 里分号是必须的吗？](#are-semicolons-required-in-javascript)
* [在 JavaScript 里，什么是短路运算？](#what-is-short-circuit-evaluation-in-javascript)
* [什么是有状态组件？](#what-is-a-stateful-component)
* [什么是无状态组件？](#what-is-a-stateless-component)
* [解释下静态方法和实例方法的区别](#explain-the-difference-between-a-static-method-and-an-instance-method)
* [在 JavaScript 里，同步代码和异步代码有什么不同？](#what-is-the-difference-between-synchronous-and-asynchronous-code-in-javascript)
* [`this` 关键字是什么，它是如何工作的？](#what-is-the-this-keyword-and-how-does-it-work)
* [下面的代码执行的结果是什么？](#what-does-the-following-code-evaluate-to)
* [什么是 JavaScript 的数据类型？](#what-are-javascript-data-types)
* [诸如 React，Vue，Angular，Hyperapp 等 JavaScript UI 库/框架的目的是什么？](#what-is-the-purpose-of-javascript-ui-librariesframeworks-like-react-vue-angular-hyperapp-etc)
* [什么是‘严格模式’，它带来哪些关键性的好处？](#what-does-use-strict-do-and-what-are-some-of-the-key-benefits-to-using-it)
* [`let` `var` `const` 和无关键字声明变量有何不同？](#what-are-the-differences-between-var-let-const-and-no-keyword-statements)
* [什么是虚拟 DOM，为何库/框架都在用它？](#what-is-a-virtual-dom-and-why-is-it-used-in-librariesframeworks)
* [什么是跨站脚本攻击（XSS），你是如何阻止它的？](#what-is-a-cross-site-scripting-attack-xss-and-how-do-you-prevent-it)
</details>


### React

<details>
<summary>查看内容</summary>

* [`setState` 将回调函数作为参数目的是什么](#what-is-the-purpose-of-callback-function-as-an-argument-of-setstate)
* [回调引用 refs 和 findDOMMNode 哪个更推荐使用？](#which-is-the-preferred-option-between-callback-refs-and-finddomnode)
* [React 组件中的属性（prop）`children` 是什么？](#what-is-children-prop)
* [React 为什么用 `className` 属性代替 `class`?](#why-react-uses-classname-over-class-attribute)
* [在 React 中，什么是 `context`？](#what-is-context)
* [在 React 中，`Element` 和 `Component` 有什么区别？](#what-is-the-difference-between-element-and-component)
* [在 React 中，错误边界是什么？](#what-are-error-boundaries-in-react)
* [在 React 中，什么是 `fragments`？](#what-are-fragments)
* [什么是高阶组件？](#what-are-higher-order-components)
* [React 和 HTML 对事件处理的区别？](#what-is-the-difference-between-html-and-react-event-handling)
* [什么是内联条件表达式？](#what-is-inline-conditional-expressions)
* [什么是 key ，在 lists 中使用的好处是什么？](#what-is-a-key-what-are-the-benefits-of-using-it-in-lists)
* [React 里的生命周期有哪些？](#what-are-the-lifecycle-methods-in-react)
* [React 组件中，生命周期的各个阶段是什么？](#what-are-the-different-phases-of-the-component-lifecycle-in-react)
* [在 React 中，状态提升是什么意思？](#what-does-lifting-state-up-in-react-mean)
* [在 React class 组件中，你是如何确保 `this` 的正确指向的？](#how-do-you-ensure-methods-have-the-correct-this-context-in-react-component-classes)
* [你是怎么给事件处理或回调函数传参的？](#how-do-you-pass-an-argument-to-an-event-handler-or-callback)
* [在 React 中是 `portals` 是什么？](#what-are-portals-in-reactjs)
* [在 React 中，如何校验 `prop`？](#how-to-apply-prop-validation-in-react)
* [在 React 里，如何写注释？](#how-to-write-comments-in-react)
* [什么是 `refs`，我们如何使用它？](#what-are-refs-when-should-they-be-used)
* [什么是有状态组件？](#what-is-a-stateful-component)
* [什么是无状态组件？](#what-is-a-stateless-component)
</details>


### HTML

<details>
<summary>查看内容</summary>

* [图片里的 `alt` 属性是做什么的？](#what-is-the-purpose-of-the-alt-attribute-on-images)
* [`<script>` 标签的 `defer` 和 `async` 是什么？](#what-are-defer-and-async-attributes-on-a-script-tag)
* [不采用缓存的目的是什么，你如何实现它？](#what-is-the-purpose-of-cache-busting-and-how-can-you-achieve-it)
* [什么是 `DOM`？](#what-is-the-dom)
* [一个页面里是否可以包含多个 `<header>` 元素， `<footer>` 元素呢？](#can-a-web-page-contain-multiple-header-elements-what-about-footer-elements)
* [讨论下 HTML 规范和浏览器实现之间的区别？](#discuss-the-differences-between-an-html-specification-and-a-browsers-implementation-thereof)
* [React 和 HTML 对事件处理的区别？](#what-is-the-difference-between-html-and-react-event-handling)
* [相比 HTML，XHTML 有哪些不同？](#what-are-some-differences-that-xhtml-has-compared-to-html)
* [简明的阐述下 HTML5 语义标签 `<header>`，`<article>`，`<section>`，`<footer>` 的用法](#briefly-describe-the-correct-usage-of-the-following-html5-semantic-elements-header-articlesection-footer)
* [什么是 HTML5 Web Storage，解释下 `localStorage` 和 `sessionStorage`？](#what-is-html5-web-storage-explain-localstorage-and-sessionstorage)
* [什么时候和为什么使用 `rel="noopener"` 属性？](#where-and-why-is-the-relnoopener-attribute-used)
</details>


### CSS

<details>
<summary>查看内容</summary>

* [什么是 CSS BEM？](#what-is-css-bem)
* [简要阐述下 CSS 的盒模型，及各个组成部分？](#describe-the-layout-of-the-css-box-model-and-briefly-describe-each-component)
* [用 CSS 预处理的优势是什么？](#what-are-the-advantages-of-using-css-preprocessors)
* [CSS 里通用兄弟选择器和相邻兄弟选择器的区别？](#what-is-the-difference-between--and--sibling-selectors)
* [你能描述下 CSS 优先级是如何工作的？](#can-you-describe-how-css-specificity-works)
* [`em` 和 `rem` 单位的区别？](#what-is-the-difference-between-em-and-rem-units)
* [使用 flexbox，创建一个 3 列布局，每一列取容器的百分之 `col-{n}`/12 ](#using-flexbox-create-a-3-column-layout-where-each-column-takes-up-a-col-n--12-ratio-of-the-container)
* [什么是聚焦环，正确的解决方案是什么？](#what-is-a-focus-ring-what-is-the-correct-solution-to-handle-them)
* [你能说出 `@media` 属性的四种类型吗？](#can-you-name-the-four-types-of-media-properties)
* [CSS 雪碧图的优势在哪里，如何使用？](#what-are-the-advantages-of-using-css-sprites-and-how-are-they-utilized)
</details>


### Node

<details>
<summary>查看内容</summary>

* [你如何避免回调地狱？](#how-can-you-avoid-callback-hells)
* [Node.js 中，经常使用回调的模式，把执行过程中遇到的错误，作为回调函数的第一个参数，这么做的优势是什么？](#nodejs-often-uses-a-callback-pattern-where-if-an-error-is-encountered-during-execution-this-error-is-passed-as-the-first-argument-to-the-callback-what-are-the-advantages-of-this-pattern)
* [在 Node.js 中，事件循环是什么？](#what-is-the-event-loop-in-nodejs)
* [什么是 `REST`？](#what-is-rest)
</details>


### 安全

<details>
<summary>查看内容</summary>

* [什么是 XSS 攻击，你如何预防它？](#what-is-a-cross-site-scripting-attack-xss-and-how-do-you-prevent-it)
</details>


---

## JavaScript
### == 和 === 相等运算符有什么区别？

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

### 创建一个和 Function.prototype.bind 功能一样的独立函数 bind

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

### setState 将回调函数作为参数目的是什么？

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

### 什么是回调，你可以举个例子吗？

<details>
<summary>查看答案</summary>

Callbacks are functions passed as an argument to another function to be executed once an event has occurred or a certain task is complete, often used in asynchronous code. Callback functions are invoked later by a piece of code but can be declared on initialization without being invoked.

As an example, event listeners are asynchronous callbacks that are only executed when a specific event occurs.

```js
function onClick() {
  console.log("The user clicked on the page.")
}
document.addEventListener("click", onClick)
```

However, callbacks can also be synchronous. The following `map` function takes a callback function that is invoked synchronously for each iteration of the loop (array element).

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


* Functions are first-class objects in JavaScript
* Callbacks vs Promises


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

A value is either truthy or falsy depending on how it is evaluated in a Boolean context. Falsy means false-like and truthy means true-like. Essentially, they are values that are coerced to `true` or `false` when performing certain operations.

There are 6 falsy values in JavaScript. They are:

* `false`
* `undefined`
* `null`
* `""` (empty string)
* `NaN`
* `0` (both `+0` and `-0`)

Every other value is considered truthy.

A value's truthiness can be examined by passing it into the `Boolean` function.

```js
Boolean("") // false
Boolean([]) // true
```

There is a shortcut for this using the logical NOT `!` operator. Using `!` once will convert a value to its inverse boolean equivalent (i.e. not false is true), and `!` once more will convert back, thus effectively converting the value to a boolean.

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

Initialize an empty array of length `n`. Use `Array.prototype.reduce()` to add values into the array, using the sum of the last two values, except for the first two.

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

### 0.1 + 0.2 === 0.3 表达式的值是？

<details>
<summary>查看答案</summary>

It evaluates to `false` because JavaScript uses the IEEE 754 standard for Math and it makes use of 64-bit floating numbers. This causes precision errors when doing decimal calculations, in short, due to computers working in Base 2 while decimal is Base 10.

```js
0.1 + 0.2 // 0.30000000000000004
```

A solution to this problem would be to use a function that determines if two numbers are approximately equal by defining an error margin (epsilon) value that the difference between two values should be less than.

```js
const approxEqual = (n1, n2, epsilon = 0.0001) => Math.abs(n1 - n2) < epsilon
approxEqual(0.1 + 0.2, 0.3) // true
```


#### 小贴士


* A simple solution to this problem


##### 附加链接


* [A simple helper function to check equality](https://github.com/Chalarangelo/30-seconds-of-code#approximatelyequal)
* [Fix "0.1 + 0.2 = 0.300000004" in JavaScript](http://blog.blakesimpson.co.uk/read/61-fix-0-1-0-2-0-300000004-in-javascript)

</details>

<br>[⬆ 返回顶部](#目录)

### 数组 map() 和 forEach() 方法的区别？

<details>
<summary>查看答案</summary>

Both methods iterate through the elements of an array. `map()` maps each element to a new element by invoking the callback function on each element and returning a new array. On the other hand, `forEach()` invokes the callback function for each element but does not return a new array. `forEach()` is generally used when causing a side effect on each iteration, whereas `map()` is a common functional programming technique.


#### 小贴士


* Use `forEach()` if you need to iterate over an array and cause mutations to the elements without needing to return values to generate a new array.
* `map()` is the right choice to keep data immutable where each value of the original array is mapped to a new array.


##### 附加链接


* [MDN docs for forEach](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)
* [MDN docs for map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
* [JavaScript — Map vs. ForEach](https://codeburst.io/javascript-map-vs-foreach-f38111822c0f)

</details>

<br>[⬆ 返回顶部](#目录)

### 下面的例子中，console.log 会打印出什么？

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

Due to hoisting, the local variable `foo` is declared before the `console.log` method is called. This means the local variable `foo` is passed as an argument to `console.log()` instead of the global one declared outside of the function. However, since the value is not hoisted with the variable declaration, the output will be `undefined`, not `2`.


#### 小贴士


* Hoisting is JavaScript’s default behavior of moving declarations to the top
* Mention of `strict` mode


##### 附加链接


* [MDN docs for hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 中，声明提升是如何工作的？

<details>
<summary>查看答案</summary>

Hoisting is a JavaScript mechanism where variable and function declarations are put into memory during the compile phase. This means that no matter where functions and variables are declared, they are moved to the top of their scope regardless of whether their scope is global or local.

However, the value is not hoisted with the declaration.

The following snippet:

```js
console.log(hoist)
var hoist = "value"
```

is equivalent to:

```js
var hoist
console.log(hoist)
hoist = "value"
```

Therefore logging `hoist` outputs `undefined` to the console, not `"value"`.

Hoisting also allows you to invoke a function declaration before it appears to be declared in a program.

```js
myFunction() // No error; logs "hello"
function myFunction() {
  console.log("hello")
}
```

But be wary of function expressions that are assigned to a variable:

```js
myFunction() // Error: `myFunction` is not a function
var myFunction = function() {
  console.log("hello")
}
```


#### 小贴士


* Hoisting is JavaScript’s default behavior of moving declarations to the top
* Functions declarations are hoisted before variable declarations


##### 附加链接


* [MDN docs for hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)
* [Understanding Hoisting in JavaScript](https://scotch.io/tutorials/understanding-hoisting-in-javascript)

</details>

<br>[⬆ 返回顶部](#目录)

### HTML 和 React 中的事件处理有什么区别？

<details>
<summary>查看答案</summary>

Some of the key differences are:

* In HTML, the event name should be in lowercase, whereas in React it follows camelcase convention.

```html
<!-- HTML -->
<button onclick="handleClick()">
```

```jsx
/* React */
<button onClick="handleClick()">
```

* In HTML, `false` can be returned to prevent default behavior, whereas in React `preventDefault` has to be called explicitly.

```html
<!-- HTML -->
<a href="#" onclick="console.log('The link was clicked.'); return false"/>
```

```jsx
/* React */
function handleClick(e) {
  e.preventDefault()
  console.log("The link was clicked.")
}
```


#### 小贴士


* HTML uses lowercase event names, React uses camelcase event names.


##### 附加链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 为何将 JavaScript 源文件里的整个内容用匿名函数包裹起来？

<details>
<summary>查看答案</summary>

This technique is very common in JavaScript libraries. It creates a closure around the entire contents of the file which creates a private namespace and thereby helps avoid potential name clashes between different JavaScript modules and libraries. The function is immediately invoked so that the namespace (library name) is assigned the return value of the function.

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


* Used among many popular JavaScript libraries
* Creates a private namespace


##### 附加链接


* [MDN docs for closures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是内联条件表达式？

<details>
<summary>查看答案</summary>

You can use either `if` statements or ternary expressions to conditionally render expressions. Apart from these approaches, you can also embed any expressions in JSX by wrapping them in curly braces and then followed by the logical operator `&&`.

```jsx
;<h1>Hello!</h1>
{
  messages.length > 0 && <h2>You have {messages.length} unread messages.</h2>
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

### 词法作用域和动态作用域的区别？

<details>
<summary>查看答案</summary>

Lexical scoping refers to when the location of a function's definition determines which variables you have access to. On the other hand, dynamic scoping uses the location of the function's invocation to determine which variables are available.


#### 小贴士


* Lexical scoping is also known as static scoping.
* Lexical scoping in JavaScript allows for the concept of closures.
* Most languages use lexical scoping because it tends to promote source code that is more easily understood.


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

> There are many ways to solve this problem, this is just one one of them.

Using `String.prototype.slice()` we can grab the last 4 characters of the string by passing `-4` as an argument. Then, using `String.prototype.padStart()`, we can pad the string to the original length with the repeated mask character.

```js
const mask = (str, maskChar = "#") =>
  str.slice(-4).padStart(str.length, maskChar)
```


#### 小贴士


* Short, one-line functional solutions to problems should be preferred provided they are efficient


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 MIME 类型，有什么作用？

<details>
<summary>查看答案</summary>

`MIME` is an acronym for `Multi-purpose Internet Mail Extensions`. It is used as a standard way of classifying file types over the Internet.


#### 小贴士


* A `MIME type` actually has two parts: a type and a subtype that are separated by a slash (/). For example, the `MIME type` for Microsoft Word files is `application/msword` (i.e., type is application and the subtype is msword).


##### 附加链接


* [MIME Type MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)

</details>

<br>[⬆ 返回顶部](#目录)

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

Advantages include:

* Not needing to process data if there is no need to even reference it
* Having a consistent API leads to more adoption
* Ability to easily adapt a callback pattern that will lead to more maintainable code

As you can see from below example, the callback is called with null as its first argument if there is no error. However, if there is an error, you create an Error object, which then becomes the callback's only parameter. The callback function allows a user to easily know whether or not an error occurred.

This practice is also called the _Node.js error convention_, and this kind of callback implementations are called _error-first callbacks_.

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


* This is just a convention. However, you should stick to it.


##### 附加链接


* [The Node.js Way Understanding Error-First Callbacks](http://fredkschott.com/post/2014/03/understanding-error-first-callbacks-in-node-js/)
* [What are the error conventions?](https://docs.nodejitsu.com/articles/errors/what-are-the-error-conventions)

</details>

<br>[⬆ 返回顶部](#目录)

### `null`  和 `undefined` 有何不同？

<details>
<summary>查看答案</summary>

In JavaScript, two values discretely represent nothing - `undefined` and `null`. The concrete difference between them is that `null` is explicit, while `undefined` is implicit. When a property does not exist or a variable has not been given a value, the value is `undefined`. `null` is set as the value to explicitly indicate “no value”. In essence, `undefined` is used when the nothing is not known, and `null` is used when the nothing is known.


#### 小贴士


* `typeof undefined` evaluates to `"undefined"`.
* `typeof null` evaluates `"object"`. However, it is still a primitive value and this is considered an implementation bug in JavaScript.
* `undefined == null` evaluates to `true`.


##### 附加链接


* [MDN docs for null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)
* [MDN docs for undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)

</details>

<br>[⬆ 返回顶部](#目录)

### 描述下创建对象方式的不同，哪种方式更推荐？

<details>
<summary>查看答案</summary>

##### Object literal

Often used to store one occurrence of data.

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

##### Constructor

Often used when you need to create multiple instances of an object, each with their own data that other instances of the class cannot affect. The `new` operator must be used before invoking the constructor or the global object will be mutated.

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

##### Factory function

Creates a new object similar to a constructor, but can store private data using a closure. There is also no need to use `new` before invoking the function or the `this` keyword. Factory functions usually discard the idea of prototypes and keep all properties and methods as own properties of the object.

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

Sets the prototype of the newly created object.

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

A second argument can also be supplied to `Object.create()` which acts as a descriptor for the new properties to be defined.

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


* Prototypes are objects that other objects inherit properties and methods from.
* Factory functions offer private properties and methods through a closure but increase memory usage as a tradeoff, while classes do not have private properties or methods but reduce memory impact by reusing a single prototype object.


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 形参和实参的区别？

<details>
<summary>查看答案</summary>

Parameters are the variable names of the function definition, while arguments are the values given to a function when it is invoked.

```js
function myFunction(parameter1, parameter2) {
  console.log(arguments[0]) // "argument1"
}
myFunction("argument1", "argument2")
```


#### 小贴士


* `arguments` is an array-like object containing information about the arguments supplied to an invoked function.
* `myFunction.length` describes the arity of a function (how many parameters it has, regardless of how many arguments it is supplied).


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### JavaScript 里是通过值传递还是引用传递？

<details>
<summary>查看答案</summary>

JavaScript always passes by value. However, with objects, the value is a reference to the object.


#### 小贴士


* Difference between pass-by-value and pass-by-reference


##### 附加链接


* [JavaScript Value vs Reference](https://medium.com/dailyjs/back-to-roots-javascript-value-vs-reference-8fb69d587a18)

</details>

<br>[⬆ 返回顶部](#目录)

### 你是怎么给事件处理/回调函数传参的？

<details>
<summary>查看答案</summary>

You can use an arrow function to wrap around an event handler and pass arguments, which is equivalent to calling `bind`:

```jsx
<button onClick={() => this.handleClick(id)} />
<button onClick={this.handleClick.bind(this, id)} />
```


#### 小贴士




##### 附加链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)

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

The first `console.log` outputs `true` because JavaScript's compiler performs type conversion and therefore it compares to strings by their value. On the other hand, the second `console.log` outputs `false` because Arrays are Objects and Objects are compared by reference.


#### 小贴士


* JavaScript performs automatic type conversion
* Objects are compared by reference
* Primitives are compared by value


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

Because of JavaScript's automatic semicolon insertion (ASI), the compiler places a semicolon after `return` keyword and therefore it returns `undefined` without an error being thrown.


#### 小贴士


* Automatic semicolon placement can lead to time-consuming bugs


##### 附加链接


* [Automatic semicolon insertion in JavaScript](http://2ality.com/2011/05/semicolon-insertion.html)

</details>

<br>[⬆ 返回顶部](#目录)

### JavaScript 里分号是必须的吗？

<details>
<summary>查看答案</summary>

Sometimes. Due to JavaScript's automatic semicolon insertion, the interpreter places semicolons after most statements. This means semicolons can be omitted in most cases.

However, there are some cases where they are required. They are not required at the beginning of a block, but are if they follow a line and:

1.  The line starts with `[`

```js
const previousLine = 3
;[1, 2, previousLine].map(n => n * 2)
```

2.  The line starts with `(`

```js
const previousLine = 3
;(function() {
  // ...
})()
```

In the above cases, the interpreter does not insert a semicolon after `3`, and therefore it will see the `3` as attempting object property access or being invoked as a function, which will throw errors.


#### 小贴士


* Semicolons are usually optional in JavaScript but have edge cases where they are required.
* If you don't use semicolons, tools like Prettier will insert semicolons for you in the places where they are required on save in a text editor to prevent errors.


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

Synchronous means each operation must wait for the previous one to complete.

Asynchronous means an operation can occur while another operation is still being processed.

In JavaScript, all code is synchronous due to the single-threaded nature of it. However, asynchronous operations not part of the program (such as `XMLHttpRequest` or `setTimeout`) are processed outside of the main thread because they are controlled by native code (browser APIs), but callbacks part of the program will still be executed synchronously.


#### 小贴士


* JavaScript has a concurrency model based on an "event loop".
* Functions like `alert` block the main thread so that no user input is registered until the user closes it.


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 下面的代码执行的结果是什么？

```js
typeof typeof 0
```

<details>
<summary>查看答案</summary>

It evaluates to `"string"`.

`typeof 0` evaluates to the string `"number"` and therefore `typeof "number"` evaluates to `"string"`.


#### 小贴士




##### 附加链接


* [MDN docs for typeof](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 JavaScript 的数据类型？

<details>
<summary>查看答案</summary>

The latest ECMAScript standard defines seven data types, six of them being primitive: `Boolean`, `Null`, `Undefined`, `Number`, `String`, `Symbol` and one non-primitive data type: `Object`.


#### 小贴士


* Mention of newly added `Symbol` data type
* `Array`, `Date` and `function` are all of type `object`
* Functions in JavaScript are objects with the capability of being callable


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

### React 组件中的属性（prop）children 是什么？

<details>
<summary>查看答案</summary>

Children is a prop (`this.prop.children`) that allows components to be passed as data to other components. There are a number of methods available in the React API to work with this prop, such as `React.Children.map`, `React.Children.forEach`, `React.Children.count`, `React.Children.only` and `React.Children.toArray`. A simple usage example of the children prop is as follows:

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


* Children is a prop that allows components to be passed as data to other components.
* The React API provides methods to work with this prop.


##### 附加链接


* [React docs on Children](https://reactjs.org/docs/jsx-in-depth.html#children-in-jsx)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是闭包，你可以举一个有用的例子吗？

<details>
<summary>查看答案</summary>

A closure is a function defined inside another function and has access to its lexical scope even when it is executing outside its lexical scope. The closure has access to variables in three scopes:

* Variables declared in its own scope
* Variables declared in the scope of the parent function
* Variables declared in the global scope

In JavaScript, all functions are closures because they have access to the outer scope, but most functions don't utilise the usefulness of closures: the persistence of state. Closures are also sometimes called stateful functions because of this.

In addition, closures are the only way to store private data that can't be accessed from the outside in JavaScript. They are the key to the UMD (Universal Module Definition) pattern, which is frequently used in libraries that only expose a public API but keep the implementation details private, preventing name collisions with other libraries or the user's own code.


#### 小贴士


* Closures are useful because they let you associate data with a function that operates on that data.
* A closure can substitute an object with only a single method.
* Closures can be used to emulate private properties and methods.


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

### 在 React 中，什么是 fragments？

<details>
<summary>查看答案</summary>

Fragments allow a React component to return multiple elements without a wrapper, by groupping the children without adding extra elements to the DOM. Fragments offer better performance, lower memory usage, a cleaner DOM and can help in dealing with certain CSS mechanisms (e.g. tables, Flexbox and Grid).

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

// Short syntax (might not supported by all tools):
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


* Fragments group multiple elements returned from a component, without adding a DOM element around them.


##### 附加链接


* [React docs on Fragments](https://reactjs.org/docs/fragments.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是函数式编程？

<details>
<summary>查看答案</summary>

Functional programming is a paradigm in which programs are built in a declarative manner using pure functions that avoid shared state and mutable data. Functions that always return the same value for the same input and don't produce side effects are the pillar of functional programming. Many programmers consider this to be the best approach to software development as it reduces bugs and cognitive load.


#### 小贴士


* Cleaner, more concise development experience
* Simple function composition
* Features of JavaScript that enable functional programming (`.map`, `.reduce` etc.)
* JavaScript is multi-paradigm programming language (Object-Oriented Programming and Functional Programming live in harmony)


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

Memoization is the process of caching the output of function calls so that subsequent calls are faster. Calling the function again with the same input will return the cached output without needing to do the calculation again.

A basic implementation in JavaScript looks like this:

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


* The above technique returns a unary function even if the function can take multiple arguments.
* The first function call will be slower than usual because of the overhead created by checking if a cached result exists and setting a result before returning the value.
* Memoization increases performance on subsequent function calls but still needs to do work on the first call.


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

`NaN` (Not-a-Number) is the only value not equal to itself when comparing with any of the comparison operators. `NaN` is often the result of meaningless math computations, so two `NaN` values make no sense to be considered equal.


#### 小贴士


* The difference between `isNaN()` and `Number.isNaN()`
* `const isNaN = x => x !== x`


##### 附加链接


* [MDN docs for `NaN`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 Nodejs 里的事件循环（event loop）？

<details>
<summary>查看答案</summary>

The event loop handles all async callbacks. Callbacks are queued in a loop, while other code runs, and will run one by one when the response for each one has been received.


#### 小贴士


* The event loop allows Node.js to perform non-blocking I/O operations, despite the fact that JavaScript is single-threaded


##### 附加链接


* [Node.js docs on event loop, timers and process.nextTick()](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/)

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

Gather all supplied arguments using the rest operator `...` and return a unary function that uses `Array.prototype.reduce()` to run the value through the series of functions before returning the final value.

```js
const pipe = (...fns) => x => fns.reduce((v, fn) => fn(v), x)
```


#### 小贴士


* Function composition is the process of combining two or more functions to produce a new function.


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

A pure function is a function that satisfies these two conditions:

* Given the same input, the function returns the same output.
* The function doesn't cause side effects outside of the function's scope (i.e. mutate data outside the function or data supplied to the function).

Pure functions can mutate local data within the function as long as it satisfies the two conditions above.

##### Pure

```js
const a = (x, y) => x + y
const b = (arr, value) => arr.concat(value)
const c = arr => [...arr].sort((a, b) => a - b)
```

##### Impure

```js
const a = (x, y) => x + y + Math.random()
const b = (arr, value) => (arr.push(value), arr)
const c = arr => arr.sort((a, b) => a - b)
```


#### 小贴士


* Pure functions are easier to reason about due to their reliability.
* All functions should be pure unless explicitly causing a side effect (i.e. `setInnerHTML`).
* If a function does not return a value, it is an indication that it is causing side effects.


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

Static methods belong to a class and don't act on instances, while instance methods belong to the class prototype which is inherited by all instances of the class and acts on them.

```js
Array.isArray // static method of Array
Array.prototype.push // instance method of Array
```

In this case, the `Array.isArray` method does not make sense as an instance method of arrays because we already know the value is an array when working with it.

Instance methods could technically work as static methods, but provide terser syntax:

```js
const arr = [1, 2, 3]
arr.push(4)
Array.push(arr, 4)
```


#### 小贴士


* How to create static and instance methods with ES2015 class syntax


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

Including `'use strict'` at the beginning of your JavaScript source file enables strict mode, which enforces more strict parsing and error handling of JavaScript code. It is considered a good practice and offers a lot of benefits, such as:

* Easier debugging due to eliminating silent errors.
* Disallows variable redefinition.
* Prevents accidental global variables.
* Oftentimes provides increased performance over identical code that is not running in strict mode.
* Simplifies `eval()` and `arguments`.
* Helps make JavaScript more secure.


#### 小贴士


* Eliminates `this` coercion, throwing an error when `this` references a value of `null` or `undefined`.
* Throws an error on invalid usage of `delete`.
* Prohibits some syntax likely to be defined in future versions of ECMAScript


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

An element is a plain object describing what you want to appear on the screen in terms of the DOM nodes or other components. Elements can contain other elements in their props. Creating a React element is cheap. Once an element is created, it is never mutated.

A component, on the other hand, can be declared in several different ways. It can be a class with a `render()` method (class component) or a function (functional component). Components take props as an input and return an element tree as the output.


#### 小贴士


* Elements are immutable, plain objects that describe the DOM nodes or components you want to render.
* Components can be either classes or functions, that take props as an input and return an element tree as the output.


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


### setState 将回调函数作为参数目的是什么？

<details>
<summary>查看答案</summary>

The callback function is invoked when `setState` has finished and the component gets rendered. Since `setState` is asynchronous, the callback function is used for any post action.

```jsx
setState({ name: "sudheer" }, () =>
  console.log("The name has updated and component re-rendered")
)
```


#### 小贴士


* The callback function is invoked after `setState` finishes and is used for any post action.
* It is recommended to use lifecycle method rather this callback function.


##### 附加链接


* [React docs on `setState`](https://reactjs.org/docs/react-component.html#setstate)

</details>

<br>[⬆ 返回顶部](#目录)

### React 为什么用 className 属性代替 class?

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

### HTML 和 React 中的事件处理有什么区别？

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

There are four different phases of component’s lifecycle:

**Initialization**: In this phase react component prepares setting up the initial state and default props.

**Mounting**: The react component is ready to mount in the browser DOM. This phase covers `getDerivedStateFromProps` and `componentDidMount` lifecycle methods.

**Updating**: In this phase, the component gets updated in two ways, sending the new props and updating the state. This phase covers `getDerivedStateFromProps`, `shouldComponentUpdate`, `getSnapshotBeforeUpdate` and `componentDidUpdate` lifecycle methods.

**Unmounting**: In this last phase, the component is not needed and gets unmounted from the browser DOM. This phase includes the `componentWillUnmount` lifecycle method.

**Error Handling**: In this phase, the component is called whenever there's an error during rendering, in a lifecycle method, or in the constructor for any child component. This phase includes the `componentDidCatch` lifecycle method.

<img alt="lifecycle phases" src="https://pbs.twimg.com/media/DZ-97vzW4AAbcZj.jpg:large" style="width: 100%"/>


#### 小贴士




##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 你是怎么给事件处理/回调函数传参的？

<details>
<summary>查看答案</summary>

You can use an arrow function to wrap around an event handler and pass arguments, which is equivalent to calling `bind`:

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

### React 组件中的属性（prop）children 是什么？

<details>
<summary>查看答案</summary>

Children is a prop (`this.prop.children`) that allows components to be passed as data to other components. There are a number of methods available in the React API to work with this prop, such as `React.Children.map`, `React.Children.forEach`, `React.Children.count`, `React.Children.only` and `React.Children.toArray`. A simple usage example of the children prop is as follows:

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


* Children is a prop that allows components to be passed as data to other components.
* The React API provides methods to work with this prop.


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

Error boundaries are React components that catch JavaScript errors anywhere in their child component tree, log those errors, and display a fallback UI instead of the component tree that crashed.

A class component becomes an error boundary if it defines a new lifecycle method called `componentDidCatch`.

```jsx
class ErrorBoundary extends React.Component {
  constructor(props) {
    super(props)
    this.state = { hasError: false }
  }

  componentDidCatch(error, info) {
    // Display fallback UI
    this.setState({ hasError: true })
    // You can also log the error to an error reporting service
    logErrorToMyService(error, info)
  }

  render() {
    if (this.state.hasError) {
      // You can render any custom fallback UI
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

### 在 React 中，什么是 fragments？

<details>
<summary>查看答案</summary>

Fragments allow a React component to return multiple elements without a wrapper, by groupping the children without adding extra elements to the DOM. Fragments offer better performance, lower memory usage, a cleaner DOM and can help in dealing with certain CSS mechanisms (e.g. tables, Flexbox and Grid).

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

// Short syntax (might not supported by all tools):
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


* Fragments group multiple elements returned from a component, without adding a DOM element around them.


##### 附加链接


* [React docs on Fragments](https://reactjs.org/docs/fragments.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是高阶组件？

<details>
<summary>查看答案</summary>

A higher-order component (HOC) is a function that takes a component as an argument and returns a new component. It is a pattern that is derived from React’s compositional nature. Higher-order components are like **pure components** because they accept any dynamically provided child component, but they won’t modify or copy any behavior from their input components.

```jsx
const EnhancedComponent = higherOrderComponent(WrappedComponent)
```


#### 小贴士


* They can be used for state abstraction and manipulation, props manipulation, render high jacking, etc.


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


## HTML
###  图片里的 alt 属性是做什么的？

<details>
<summary>查看答案</summary>

如果用户看不到图像，`alt` 属性可以提供替代信息。`alt` 属性应该用于描述，而那些仅仅是装饰目的图像，可以为空

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

### 一个页面里是否可以包含多个 <header> 元素， <footer> 元素呢？

<details>
<summary>查看答案</summary>

Yes to both. The W3 documents state that the tags represent the header(`<header>`) and footer(`<footer>`) areas of their nearest ancestor "section". So not only can the page `<body>` contain a header and a footer, but so can every `<article>` and `<section>` element.


#### 小贴士


* W3 recommends having as many as you want, but only 1 of each for each "section" of your page, i.e. body, section etc.


##### 附加链接


* [StackOverflow Using header or footer tag twice](https://stackoverflow.com/questions/4837269/html5-using-header-or-footer-tag-twice?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa)

</details>

<br>[⬆ 返回顶部](#目录)

### 简明的阐述下 HTML5 语义标签 <header>，<article>，<section>，<footer> 的用法

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

### <script> 标签的 defer 和 async 是什么？

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

### HTML 和 React 中的事件处理有什么区别？

<details>
<summary>查看答案</summary>

Some of the key differences are:

* In HTML, the event name should be in lowercase, whereas in React it follows camelcase convention.

```html
<!-- HTML -->
<button onclick="handleClick()">
```

```jsx
/* React */
<button onClick="handleClick()">
```

* In HTML, `false` can be returned to prevent default behavior, whereas in React `preventDefault` has to be called explicitly.

```html
<!-- HTML -->
<a href="#" onclick="console.log('The link was clicked.'); return false"/>
```

```jsx
/* React */
function handleClick(e) {
  e.preventDefault()
  console.log("The link was clicked.")
}
```


#### 小贴士


* HTML uses lowercase event names, React uses camelcase event names.


##### 附加链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 相比 HTML，XHTML 有哪些不同？

<details>
<summary>查看答案</summary>

Some of the key differences are:

* An XHTML element must have an XHTML `<DOCTYPE>`
* Attributes values must be enclosed in quotes
* Attribute minimization is forbidden (e.g. one has to use `checked="checked"` instead of `checked`)
* Elements must always be properly nested
* Elements must always be closed
* Special characters must be escaped


#### 小贴士


* Any element can be self-closed
* Tags ands attributes are case-sensitive, usually lowercase


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

### 你能说出 @media 属性的四种类型吗？

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

Advantages include:

* Not needing to process data if there is no need to even reference it
* Having a consistent API leads to more adoption
* Ability to easily adapt a callback pattern that will lead to more maintainable code

As you can see from below example, the callback is called with null as its first argument if there is no error. However, if there is an error, you create an Error object, which then becomes the callback's only parameter. The callback function allows a user to easily know whether or not an error occurred.

This practice is also called the _Node.js error convention_, and this kind of callback implementations are called _error-first callbacks_.

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


* This is just a convention. However, you should stick to it.


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

The event loop handles all async callbacks. Callbacks are queued in a loop, while other code runs, and will run one by one when the response for each one has been received.


#### 小贴士


* The event loop allows Node.js to perform non-blocking I/O operations, despite the fact that JavaScript is single-threaded


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
