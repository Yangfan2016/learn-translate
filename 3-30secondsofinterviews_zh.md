<a href="https://30secondsofinterviews.org"><img src="https://github.com/30-seconds/30-seconds-of-interviews/raw/master/logo.jpg" alt="30 Seconds of Interviews logo"></a>

<h1 align="center">
  面试 30 秒
</h1>

<h4 align="center">一个面试常用的问题精选集，帮助你准备下一次面试</h4>


> - 原文地址：https://github.com/30-seconds/30-seconds-of-interviews/blob/master/README.md
> - 原文作者：[Stefan Feješ](https://github.com/fejes713)  
> - 译者：[Yangfan2016](https://github.com/Yangfan2016)
> - 备注：删除了重复部分，整理和精简了原文档的索引部分
> - 英文版权所有：[MIT. Copyright (c) Stefan Feješ](https://github.com/30-seconds/30-seconds-of-interviews/blob/master/LICENSE)

## 前言

面试是令人生畏的，它甚至可以让经验丰富的专家在压力之下大脑一片空白。复习和学习哪些在面试中常遇到的问题（从社区中收集了被问到的和他们是如何应对的问题）。通过把实践和现实生活结合起来，你就可以从容的准备面对下一次面试


## [在线观看](https://30secondsofinterviews.org/)


## 目录


### JavaScript

<details>
<summary>查看内容</summary>

* [创建一个 batches 函数，返回一个食谱中可以被作为烹饪整批食材的最大数量](#创建一个-batches-函数返回一个食谱中可以被作为烹饪整批食材的最大数量)
* [什么是大 O 标记法？](#什么是大-o-标记法)
* [创建一个和 `Function.prototype.bind` 功能一样的独立函数 `bind`](#创建一个和-Functionprototypebind-功能一样的独立函数-bind)
* [你是怎么避免回调地狱的？](#你是怎么避免回调地狱的)
* [什么是回调，你可以举个例子吗？](#什么是回调你可以举个例子吗)
* [在 JavaScript 中，你是如何克隆一个对象的？](#在-javascript-中你是如何克隆一个对象的)
* [什么是闭包，你可以举一个有用的例子吗？](#什么是闭包你可以举一个有用的例子吗)
* [在 JavaScript 中，你是如何比较两个对象的？](#在-javascript-中你是如何比较两个对象的)
* [什么是 `CORS`？](#什么是-cors)
* [`==` 和 `===` 相等运算符有什么区别？](#-和--相等运算符有什么区别)
* [什么是事件代理，为什么它是有用的，你可以举个例子说明如何使用它？](#什么是事件代理为什么它是有用的你可以举个例子说明如何使用它)
* [什么是事件驱动编程？](#什么是事件驱动编程)
* [在 JavaScript 中，表达式和语句的区别？](#在-javascript-中表达式和语句的区别)
* [在 JavaScript 中，什么是真值（truthy），假值（falsy）?](#在-javascript-中什么是真值truthy假值falsy)
* [生成一个包含的 n 项斐波那契数列元素的数组](#生成一个包含的-n-项斐波那契数列元素的数组)
* [`0.1 + 0.2 === 0.3` 表达式的值是？](#01--02--03-表达式的值是)
* [数组 `map()` 和 `forEach()` 方法的区别？](#数组-map-和-foreach-方法的区别)
* [什么是函数式编程？](#什么是函数式编程)
* [下面的例子中，`console.log` 会打印出什么？](#下面的例子中consolelog-会打印出什么)
* [在 JavaScript 中，声明提升是如何工作的？](#在-javascript-中声明提升是如何工作的)
* [为何将 JavaScript 源文件里的整个内容用匿名函数包裹起来？](#为何将-javascript-源文件里的整个内容用匿名函数包裹起来)
* [阐释下命令式编程和声明式编程的区别？](#阐释下命令式编程和声明式编程的区别)
* [词法作用域和动态作用域的区别？](#词法作用域和动态作用域的区别)
* [创建一个函数，用 ‘#’ 符号遮住字符串（除最后4个字符之外）](#创建一个函数用--符号遮住字符串除最后4个字符之外)
* [什么是缓存代理模式（memoization）？](#什么是缓存代理模式memoization)
* [什么是 MIME 类型，有什么作用？](#什么是-mime-类型有什么作用)
* [对比下可变与不可变值，可变与不可变方法](#对比下可变与不可变值可变与不可变方法)
* [在 JavaScript 中，哪个值不等于它自己？](#在-javascript-中哪个值不等于它自己)
* [`null`  和 `undefined` 有何不同？](#null--和-undefined-有何不同)
* [描述下创建对象方式的不同，哪种方式更推荐？](#描述下创建对象方式的不同哪种方式更推荐)
* [形参和实参的区别？](#形参和实参的区别)
* [JavaScript 里是通过值传递还是引用传递？](#javascript-里是通过值传递还是引用传递)
* [创建一个管道函数，返回一个接受一个参数从左到右执行的合成函数](#创建一个管道函数返回一个接受一个参数从左到右执行的合成函数)
* [`i++`  和 `++i` 有什么不同？](#i--和-i-有什么不同)
* [Promise 可以变成哪些状态？](#promise-可以变成哪些状态)
* [什么是 Promises？](#什么是-promises)
* [原型继承和经典继承方式有何不同？](#原型继承和经典继承方式有何不同)
* [什么是纯函数？](#什么是纯函数)
* [什么是递归，什么时候它是有用的？](#什么是递归什么时候它是有用的)
* [下面的代码会输出什么？](#下面的代码会输出什么)
* [下面的函数会返回什么？](#下面的函数会返回什么)
* [JavaScript 里分号是必须的吗？](#javascript-里分号是必须的吗)
* [在 JavaScript 里，什么是短路运算？](#在-javascript-里什么是短路运算)
* [解释下静态方法和实例方法的区别](#解释下静态方法和实例方法的区别)
* [在 JavaScript 里，同步代码和异步代码有什么不同？](#在-javascript-里同步代码和异步代码有什么不同)
* [`this` 关键字是什么，它是如何工作的？](#this-关键字是什么它是如何工作的)
* [下面的代码执行的结果是什么？](#下面的代码执行的结果是什么)
* [什么是 JavaScript 的数据类型？](#什么是-javascript-的数据类型)
* [诸如 React，Vue，Angular，Hyperapp 等 JavaScript UI 库/框架的目的是什么？](#诸如-reactvueangularhyperapp-等-javascript-ui-库框架的目的是什么)
* [什么是 “严格模式”，它带来哪些关键性的好处？](#什么是严格模式它带来哪些关键性的好处)
* [`let` `var` `const` 和无关键字声明变量有何不同？](#let-var-const-和无关键字声明变量有何不同)
* [什么是虚拟 DOM，为何库/框架都在用它？](#什么是虚拟-dom为何库框架都在用它)
</details>


### React

<details>
<summary>查看内容</summary>

* [`setState` 将回调函数作为参数目的是什么？](#setstate-将回调函数作为参数目的是什么)
* [回调引用 refs 和 findDOMNode 哪个更推荐使用？](#回调引用-refs-和-finddomnode-哪个更推荐使用)
* [React 组件中的属性（prop）`children` 是什么？](#react-组件中的属性propchildren-是什么)
* [React 为什么用 `className` 属性代替 `class`?](#react-为什么用-classname-属性代替-class)
* [在 React 中，什么是 `context`？](#在-react-中什么是-context)
* [Element 和 Component 有什么区别？](#element-和-component-有什么区别)
* [在 React 中，错误边界是什么？](#在-react-中错误边界是什么)
* [在 React 中，什么是 `fragments`？](#在-react-中什么是-fragments)
* [什么是高阶组件？](#什么是高阶组件)
* [React 和 HTML 对事件处理的区别？](#react-和-html-对事件处理的区别)
* [什么是内联条件表达式？](#什么是内联条件表达式)
* [什么是 key ，在 lists 中使用的好处是什么？](#什么是-key-在-lists-中使用的好处是什么)
* [React 里的生命周期有哪些？](#react-里的生命周期有哪些)
* [React 组件中，生命周期的各个阶段是什么？](#react-组件中生命周期的各个阶段是什么)
* [在 React 中，状态提升是什么意思？](#在-react-中状态提升是什么意思)
* [在 React 类方式定义的组件中，你如何保证方法得到的 `this` 是正确的？](#在-react-类方式定义的组件中你如何保证方法得到的-this-是正确的)
* [你是怎么给事件处理或回调函数传参的？](#你是怎么给事件处理或回调函数传参的)
* [在 React 中，`portals` 是什么？](#在-react-中portals-是什么)
* [在 React 中，如何校验 `prop`？](#在-react-中如何校验-prop)
* [在 React 里，如何写注释？](#在-react-里如何写注释)
* [什么是 `refs`，我们如何使用它？](#什么是-refs我们如何使用它)
* [什么是有状态组件？](#什么是有状态组件)
* [什么是无状态组件？](#什么是无状态组件)
</details>


### HTML

<details>
<summary>查看内容</summary>

* [图片里的 `alt` 属性是做什么的？](#图片里的-alt-属性是做什么的)
* [`<script>` 标签的 `defer` 和 `async` 是什么？](#script-标签的-defer-和-async-是什么)
* [不采用缓存的目的是什么，你如何实现它？](#不采用缓存的目的是什么你如何实现它)
* [什么是 `DOM`？](#什么是-dom)
* [一个页面里是否可以包含多个 `<header>` 元素， `<footer>` 元素呢？](#一个页面里是否可以包含多个-header-元素-footer-元素呢)
* [讨论下 HTML 规范和浏览器实现之间的区别？](#讨论下-html-规范和浏览器实现之间的区别)
* [相比 HTML，XHTML 有哪些不同？](#相比-htmlxhtml-有哪些不同)
* [简明的阐述下 HTML5 语义标签 `<header>`，`<article>`，`<section>`，`<footer>` 的用法](#简明的阐述下-html5-语义标签-headerarticlesectionfooter-的用法)
* [什么是 HTML5 Web Storage，解释下 `localStorage` 和 `sessionStorage`？](#什么是-html5-web-storage解释下-localstorage-和-sessionstorage)
* [什么时候和为什么使用 `rel="noopener"` 属性？](#什么时候和为什么使用-relnoopener-属性)
</details>


### CSS

<details>
<summary>查看内容</summary>

* [什么是 CSS BEM？](#什么是-css-bem)
* [简要阐述下 CSS 的盒模型，及各个组成部分？](#简要阐述下-css-的盒模型及各个组成部分)
* [用 CSS 预处理的优势是什么？](#用-css-预处理的优势是什么)
* [CSS 里通用兄弟选择器和相邻兄弟选择器的区别？](#css-里通用兄弟选择器和相邻兄弟选择器的区别)
* [你能描述下 CSS 优先级是如何工作的？](#你能描述下-css-优先级是如何工作的)
* [`em` 和 `rem` 单位的区别？](#em-和-rem-单位的区别)
* [使用 flexbox，创建一个 3 列布局，每一列取容器的百分之 `col-{n}`/12 ](#使用-flexbox创建一个-3-列布局每一列取容器的百分之-col-n12)
* [什么是聚焦环，正确的解决方案是什么？](#什么是聚焦环正确的解决方案是什么)
* [你能说出 `@media` 属性的四种类型吗？](#你能说出-media-属性的四种类型吗)
* [CSS 雪碧图的优势在哪里，如何使用？](#css-雪碧图的优势在哪里如何使用)
</details>


### Node

<details>
<summary>查看内容</summary>

* [NodeJS 错误优先回调的模式有什么优势？](#nodejs-错误优先回调的模式有什么优势)
* [什么是 Nodejs 里的事件循环（event loop）？](#什么是-nodejs-里的事件循环event-loop)
* [什么是 `REST`？](#什么是-rest)
</details>


### 安全

<details>
<summary>查看内容</summary>

* [什么是跨站脚本攻击（XSS），你是如何阻止它的？](#什么是跨站脚本攻击xss你是如何阻止它的)
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

使用对象扩展操作符 `...`，对象自己的可枚举属性可以被拷贝到新对象。这将创建一个对象的浅克隆

```js
const obj = { a: 1, b: 2 }
const shallowClone = { ...obj }
```

使用这个技术，原型会被忽略。此外，嵌套对象不能被克隆，但是他们的引用被拷贝了，因此嵌套的对象依然指向和原来相同的对象。深度克隆更复杂，为了高效的克隆嵌套在对象里的任何对象类型（Date，RegExp，Function，Set。等等）

其他的替代方案包括：

* `JSON.parse(JSON.stringify(obj))` 可以用来克隆简单对象，但是它是 CPU 密集型，并且只接受合法的 JSON（因此它会跳过函数，而且不允许循环引用）
* `Object.assign({}, obj)` 是另一个替代方案
* `Object.keys(obj).reduce((acc, key) => (acc[key] = obj[key], acc), {})` 是另一个更冗长的替代方案，它更深层次的展示了这个概念


#### 小贴士


* JavaScript 通过引用传递对象，意味着嵌套对象获取到的是他们引用的副本，而不是他们的值
* 同样的方法可以用来合并两个对象


##### 附加链接


* [MDN docs for Object.assign()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)
* [Clone an object in vanilla JS](http://voidcanvas.com/clone-an-object-in-vanilla-js-in-depth/)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 中，你是如何比较两个对象的？

<details>
<summary>查看答案</summary>

即使两个拥有相同属性相同值的不同对象，当使用 `==` 或 `===` 进行比较时，也不认为他们相等。这就是因为他们是通过引用（内存里的位置）比较的，不像基本类型是通过值比较的

为了测试两个对象的结构是否相等，需要一个辅助函数，它会迭代每个对象每个自己的属性，测试他们是否有相同的值，包括嵌套对象
可选的，通过传递第三个参数 `true` 来测试对象的原型的等价性

注意：这个技术不会尝试测试数据结构的等价性，除了普通对象，数组，函数，日期和基本类型

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


* 像 string 和 number 这样的基本类型是通过值比较的
* 另一方面，对象是通过引用（在内存的位置）来比较的


##### 附加链接


* [Object Equality in JavaScript](http://adripofjavascript.com/blog/drips/object-equality-in-javascript.html)
* [Deep comparison between two values](https://30secondsofcode.org/object#equals)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 `CORS`？

<details>
<summary>查看答案</summary>

CORS（Cross-Origin Resource Sharing，跨域资源共享）是一个使用额外的 HTTP 头授权浏览器访问跨域资源的机制

一个跨域请求的例子，从 `http://mydomain.com` 提供的 web 应用程序使用 AJAX 请求 `http://yourdomain.com` 的资源

出于安全原因，浏览器限制了 JavaScript 发起的 HTTP 跨域请求。`XMLHttpRequest` 和 `fetch` 遵循同源策略，意味着 web 应用使用这些 API 只能请求同源下的 HTTP 资源，除非其他域包括正确的 CORS 头


#### 小贴士


* CORS 行为不是一个错误，它是一种保护用户的安全机制
* CORS 被设计来阻止一个用户可以无意的访问来请求合法网站阅读他们的个人信息或执行他们不想要的操作的恶意网站


##### 附加链接


* [MDN docs for CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是事件代理，为什么它是有用的，你可以举个例子说明如何使用它？

<details>
<summary>查看答案</summary>

事件代理是一个代理事件到一个单一的公共的祖先的技术。由于事件冒泡，事件会向上冒泡到 DOM 树，逐步执行每一个处理程序，直到监听事件的根元素

DOM 事件提供了一个关于发起事件的元素有用的信息 `Event.target`。这允许父元素处理行为，就好像是目标元素在监听事件，而不是所有父元素的子元素或父元素自己

它会提供两个好处：

* 它提高了性能和减少了内存消耗，而且只需要注册一个单事件监听器就可以处理潜在的成千上万的元素
* 如果元素是动态添加到父元素上的，就不需要再为它们注册新的监听器

而不是：

```js
document.querySelectorAll("button").forEach(button => {
  button.addEventListener("click", handleButtonClick)
})
```

事件代理包含一个条件确保匹配到的子元素是我们想要的：

```js
document.addEventListener("click", e => {
  if (e.target.closest("button")) {
    handleButtonClick()
  }
})
```


#### 小贴士


* 事件冒泡和事件捕获的区别


##### 附加链接


* [Event Delegation](https://davidwalsh.name/event-delegate)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 JavaScript 中，表达式和语句的区别？

<details>
<summary>查看答案</summary>

在 JavaScript 中有两种语法范畴：表达式和语句。第三种是两者结合在一起，称为一个表达式语句。它们大概概括如下：

* **表达式**: 产生一个值
* **语句**: 执行一个操作
* **表达式语句**: 产生一个值和执行一个操作

一个通用的经验法则：

> 如果你可以打印或赋值给一个变量，那么它就是一个表达式。如果不能，那它就是一个语句

##### 语句

```js
let x = 0

function declaration() {}

if (true) {
}
```

语句以指令的形式出现，但是不能产生值

```js
// 将 `y` 的绝对值赋给 `x` 
var x
if (y >= 0) {
  x = y
} else {
  x = -y
}
```

上面的代码 `y >= 0` 是唯一的表达式，无论 `true` 或 `false` 都会产生一个值。这个值不是由代码的其他部分产生的

##### 表达式

表达式产生一个值。它们可以传递给函数，因为编译器会将解析的值替代它们

```js
5 + 5 // => 10

lastCharacter("input") // => "t"

true === true // => true
```

##### 表达式语句

这里有一个和之前使用条件表达式设置语句的等价版本：

```js
// 将 `y` 的绝对值赋给 `x` 
var x = y >= 0 ? y : -y
```

这既是一个表达式，又是一个语句，因为我们声明了一个变量 `x`（语句）作为一个求值（表达式）


#### 小贴士


* 函数声明 VS 函数表达式


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


* 一个 `MIME 类型` 通常分为两部分：一个类型和一个子类型（用斜线 “/” 分割）。例如，微软 Word 文档的类型是 `application/msword`（即，类型是 “应用”，子类型是 msword）


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

`Object.create()` 也支持第二个参数，它担当定义新属性的描述符

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

`Promise` 对象代表异步操作最终的完成（或失败），和它的结果值
下面这个代码片段，100 ms 后会在标准输出打印出结果。注意 `catch`，它是用来捕获错误的。`Promise` 是链式调用的

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


* 看一看关于 `Promise` 的其他问题


##### 附加链接


* [Master the JavaScript Interview: What is a Promise?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e772618)

</details>

<br>[⬆ 返回顶部](#目录)

### 原型继承和经典继承方式有何不同？

<details>
<summary>查看答案</summary>

在类继承范式中，对象实例继承从一个类上继承他们的属性和方法，实际上是复制了一份蓝本。对象实例通常通过使用一个构造器和 `new` 关键字创建

在原型继承范式中，对象实例直接从其他对象上继承，通常通过工厂函数或 `Object.create()` 创建


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

短路求值包含逻辑运算符，从左到右求值，而且尽快停止

```js
true || false
```

在上面这个例子使用了逻辑或，JavaScript 不会查找第二个操作数 `false` ，因为表达式无论如何求值都是 `true`。这就是我们熟知短路求值

同样作用于逻辑与

```js
false && true
```

这就意味着如果你对一个表达式求值得到是一个抛出的错误的话，这并不会造成任何问题

```js
true || nonexistentFunction()
false && nonexistentFunction()
```

因为从左到右的求值，多个操作符仍然会得到 `true`

```js
true || nonexistentFunction() || window.nothing.wouldThrowError
true || window.nothing.wouldThrowError
true
```

这种行为一个常用的用法是设置默认值。如果第一个操作数是假值（falsy），那么第二个操作符就会被求值

```js
const options = {}
const setting = options.setting || "default"
setting // "default"
```

另一个常用的例子就是如果第一个操作数是真值（truthy），才将执行表达式

```js
// 替换
addEventListener("click", e => {
  if (e.target.closest("button")) {
    handleButtonClick(e)
  }
})

// 你可以发挥短路运算符的优势
addEventListener(
  "click",
  e => e.target.closest("button") && handleButtonClick(e)
)
```

在上面这个例子中，如果 `e.target` 没有或不包含匹配 `"button"` 选择器的元素时，这个函数就不会被调用。这是因为第一个操作数是假值（falsy）时，第二个操作符就不会被求值


#### 小贴士


* 逻辑操作符不会产生一个布尔值，除非操作数的值执行产生一个布尔值


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


* JavaScript 有一个基于 “事件循环” 的并发模型
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

##### 没有关键字

在变量赋值之前没有关键字存在，要么赋值给一个不存在的全局变量，要么重新分配给已声明的变量。在非严格模式下，如果变量没有声明，它将赋值为全局对象（浏览器中的 `window`）的一个属性。在严格模式下，它将抛出一个错误阻止不需要的全局变量被创建

##### var

直到 ES2015 `var` 仍是默认的声明语句。它创建了一个函数作用域，可以重新分配和重新声明。然而，由于缺少块作用域，如果变量在一个包含异步回调的循环中再次使用的话，他可能会造成问题，因为变量将继续存在于块作用域之外

下面，等到 `setTimeout` 回调执行时，循环已经完成了，而且变量 `i` 的值是 `10`，因此，所有这 10 个回调在这个函数作用域下引用了同一个可用的变量

```js
for (var i = 0; i < 10; i++) {
  setTimeout(() => {
    // 打印 `10` 10 次
    console.log(i)
  })
}

/* 使用 `var` 的解决方案 */
for (var i = 0; i < 10; i++) {
  // 作为参数传递进去
  setTimeout(console.log, 0, i)
}

for (var i = 0; i < 10; i++) {
  // 创建一个函数作用域
  ;(i => {
    setTimeout(() => {
      console.log(i)
    })
  })(i)
}
```

##### let

`let` 在 ES2015 中引入，而且是新的变量声明推荐的方法，它之后将被重新分配。试图重新声明一个变量将会抛出错误。它是块级作用域，因此在循环中可以在迭代中保持它的作用域

```js
for (let i = 0; i < 10; i++) {
  setTimeout(() => {
    // 打印 0, 1, 2, 3, ...
    console.log(i)
  })
}
```

##### const

`const` 在 ES2015 中引入，而且是新的变量声明推荐的方法，它之后不能被重新分配，即使对象是可变的（只要对象的引用不变就行）。它是块级作用域而且不能被重新分配

```js
const myObject = {}
myObject.prop = "hello!" // 没有错误
myObject = "hello" // 抛出错误
```


#### 小贴士


* 所有的声明都会被提升到它们的作用域顶部
* 然而，`let` 和 `const` 有一个叫暂时性死区的概念（TDZ，Temporal Dead Zone）。虽然声明被提升了，但有一段时间在进入作用域和被声明之间它们是不能被访问的
* 给你一个使用 `var` 的常见问题，和 `let` 如何解决它，以及保留 `var` 的解决方案
* `var` 应该尽可能的避免使用，推荐 `const` 作为所有变量的默认声明，除非它们之后会被重新分配，则使用 `let` 


##### 附加链接


* [`let` vs `const`](https://wesbos.com/let-vs-const/)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是大 O 标记法？

<details>
<summary>查看答案</summary>

大 O 标记法是一个在计算机中用来描述算法的时间复杂度。最好的算法会执行很快而且拥有最简单的复杂度

算法并不总是执行相同的操作，随着提供的数据而变化。一些例子会执行很快，而另一些例子，即使处理相同数量的元素也会很慢

在这些例子中，基本的时间是 1 个元素 = `1 ms`

##### O(1)

```js
arr[arr.length - 1]
```

* 1000 个元素 = `1 ms`

常数时间复杂度。无论数组有多少个元素，理论上执行的时间相同（排除实际的变化）

##### O(N)

```js
arr.filter(fn)
```

* 1000 元素 = `1000 ms`

线性时间复杂度。执行时间会随着数组元素的数量线性增加。如果 1000 个元素的数组执行这个函数需要 1ms，那么 7000 个元素的数组将需要执行 7ms。这是因为函数在返回结果之前必须迭代数组的所有元素

##### O([1, N])

```js
arr.some(fn)
```

* 1000 元素 = `1 ms <= x <= 1000 ms`

执行时间依赖于提供给函数的数据变化，它可能很快或很迟返回。最好的情况是 O(1)，最坏的情况是 O(N)

##### O(NlogN)

```js
arr.sort(fn)
```

* 1000 元素 ~= `10000 ms`

浏览器通常在 `sort()` 里使用快速排序实现，而且快速排序的平均时间复杂度是 O(NlgN)。在大的集合下非常高效

##### O(N^2)

```js
for (let i = 0; i < arr.length; i++) {
  for (let j = 0; j < arr.length; j++) {
    // ...
  }
}
```

* 1000 元素 = `1000000 ms`

执行时间随着元素的数量次方增加。通常是嵌套循环的结果

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

* 1000 元素 = `Infinity ms` （实际上） 

即使数组增加一个元素，执行都会增加的极其快


#### 小贴士


* 当执行时间指数式增加时，要当心嵌套循环


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

使用 `async/await` 重构函数返回 `promise` 通常是最佳选择。代替返回深度嵌套的回调，它们返回一个 `promise`，等待数据接受后然后解析，允许下一行代码以同步风格的方式执行

上面的代码重构如下：

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

这里还有许多解决回调地狱问题的方法：

* 模块化：把回调分割为独立函数
* 使用一个控制流的库，像 [async](https://www.npmjs.com/package/async)
* 使用一个带有 `promise` 的生成器
* 使用 async/await (ES2017 版本及以上)


#### 小贴士


* 作为一个高效的 JavaScript 的开发者，你必须避免不断增长的缩进级别，生产出干净的和可读的代码和能够处理复杂的流


##### 附加链接


* [Avoiding Callback Hell in Node.js](http://stackabuse.com/avoiding-callback-hell-in-node-js/)
* [Asynchronous JavaScript: From Callback Hell to Async and Await](https://blog.hellojs.org/asynchronous-javascript-from-callback-hell-to-async-and-await-9b9ceb63c8e8)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是闭包，你可以举一个有用的例子吗？

<details>
<summary>查看答案</summary>

一个闭包是一个定义在另一个函数内部可以访问它的词法作用域，即使是宿主函数在词法作用域外执行。闭包可以在三种作用域中访问变量：

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

### 什么是事件驱动编程？

<details>
<summary>查看答案</summary>

事件驱动编程是一种范式，包含构建发送和接受事件的应用。当程序触发事件时，程序通过运行仍注册了这个事件的回调函数来回应，传递给函数相关的数据。在这个模式中，事件会被触发即使没有函数订阅它也不会抛出错误

DOM 元素事件监听模式的一个常用的例子，例如，`click` 和 `mouseenter`，回调函数会在事件触发时执行

```js
document.addEventListener("click", function(event) {
  // 当用户点击文档时，这个回调函数会执行
})
```

没有 DOM 上下文，这个模式看起来是这样：

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

这个实现，`on` 是 _订阅_ 事件的方法，`emit` 是 _发布_ 事件的方法


#### 小贴士


* 领会发布订阅者模式
* 事件触发时，任何订阅了这个事件的回调函数会响应
* 用 JavaScript 展示如何创建一个简单的发布订阅者的实现


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

这两种编程类型大致概括如下：

* 命令式: **如何** 实现某事
* 声明式: **什么** 应该被实现

一个声明式编程的常用的例子是 CSS。开发者指定 CSS 属性描述某事应该看起开是什么样的而不是如何实现。”如何“ 实现被浏览器抽象出来了

另一方面，命令式编程包含实现某事的必要步骤。在 JavaScript 中，区别可以这样对比：

##### 命令式

```js
const numbers = [1, 2, 3, 4, 5]
const numbersDoubled = []
for (let i = 0; i < numbers.length; i++) {
  numbersDoubled[i] = numbers[i] * 2
}
```

我们手动循环数字数组和赋值双倍的数字给新的索引

##### 声明式

```js
const numbers = [1, 2, 3, 4, 5]
const numbersDoubled = numbers.map(n => n * 2)
```

我们用每个加倍的新值映射到新声明的数组


#### 小贴士


* 声明式编程经常用于函数和表达式。命令式编程频繁地使用语句而且依赖于造成突变的底层特性，而命令式编程注重抽象和纯粹
* 声明式编程更精简和更易处理


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


### 对比下可变与不可变值，可变与不可变方法

<details>
<summary>查看答案</summary>

两个术语的对比：

* 可变：易改变
* 不可变：不能改变

在 JavaScript，对象（object）是可变的，而原始值是不可变的。这就意味着某些方式执行对象操作时可能会改变原始引用，而执行原始值操作时不能改变原始值

所有 `String.prototype` 的方法都会返回一个新的字符串，而不会改变原始字符串，产生副作用。另一方面， 一些 `Array.prototype` 的方法不会改变原始数组引用，而是返回一个新数组，但有些方法会改变

```js
const myString = "hello!"
myString.replace("!", "") // 返回一个新字符串，不会改变原始值

const originalArray = [1, 2, 3]
originalArray.push(4) // 改变了原始数组，现在的值为 [1, 2, 3, 4]
originalArray.concat(4) // 返回一个新数组，不会改变原始数组
```


#### 小贴士


* 列举出改变和不改变原始数组的方法


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

递归是一个应用重复的过程。在 JavaScript 中，递归包含重复调用它们自己的函数，直到达到基本条件，基本条件才会打破递归循环，否则函数将无限的调用自己。当使用包含嵌套的未知深层级的数据结构时，递归是非常有用的

例如，你可以从数据库中得到以平铺数组形式的大量评论数据，但是需要以嵌套的形式显示在 UI 上。每个评论要么是顶级评论（没有父级），要么是一个父评论的回复。评论可能是一个回复的回复的回复…… 我们事先不知道这个评论之前还有多少层次。这时候递归就可以帮到我们

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

在上面的例子中，如果 `filter()` 返回一个空数组，则满足基本条件。链式的 `map()` 也不会被调用包含的递归回调，因此退出循环


#### 小贴士


* 当使用包含未知数量的嵌套的数据结构时，递归是有用的
* 递归必须有一个基本条件被满足以此退出循环，否则将无限的调用自己


##### 附加链接


* [In plain English, what is recursion?](https://softwareengineering.stackexchange.com/questions/25052/in-plain-english-what-is-recursion)

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

这个 `this` 关键字是一个代表执行函数上下文的对象。普通的函数使用 `call()`，`apply()` 和 `bind()` 可以改变他们的 `this` 值。箭头函数隐式的绑定了 `this`，因此它指向它的词法环境的上下文，忽略是否通过 `call()` 方法显示设置了上下文

这有一些常用的 `this` 如何工作的例子：

##### 对象字面量

如果这个对象在函数之前调用，普通函数中的 `this` 指向这个对象自己

属性设置为 `this`，不会指向这个对象

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

myObject.property // 不是 myObject； 而是 词法的 `this`
myObject.arrowFunction() // 不是 myObject； 而是 词法的 `this`
myObject.iife // 不是 myObject； 而是 词法的 `this`
const regularFunction = myObject.regularFunction
regularFunction() // 不是 myObject； 而是 词法的 `this`
```

##### 事件监听器

`this` 指向事件监听的那个元素

```js
document.body.addEventListener("click", function() {
  console.log(this) // document.body
})
```

##### 构造器

`this` 指向新创建的对象

```js
class Example {
  constructor() {
    console.log(this) // myExample
  }
}
const myExample = new Example()
```

##### 手动的

使用 `call()` 和 `apply()`，`this` 指向第一个参数传递的那个对象

```js
var myFunction = function() {
  return this
}
myFunction.call({ customThis: true }) // { customThis: true }
```

##### 意料之外的 `this`

因为 `this` 可以根据作用域改变，当使用普通函数可能得到意想不到的值

```js
var obj = {
  arr: [1, 2, 3],
  doubleArr() {
    return this.arr.map(function(value) {
      // this 现在指的是 this.arr
      return this.double(value)
    })
  },
  double() {
    return value * 2
  }
}
obj.doubleArr() // 抛出错误：this.double 不是一个函数
```


#### 小贴士


* 在非严格模式，全局 `this` 指的是全局对象（在浏览器是 `window`），在严格模式下，全局 `this` 是 `undefined`
* `Function.prototype.call` 和 `Function.prototype.apply` 第一个参数设置执行函数的上下文 `this`，`call` 之后接受不定量的参数，和 `apply` 接受一个数组作为第二个参数以不定量的形式提供给函数
* `Function.prototype.bind` 返回一个新函数，强制第一个参数设置为 `this` 上下文，其他函数不能改变
* 如果一个函数需要它基于如何被调用而改变 `this` 上下文时，你必须使用 `function` 关键字。当你想要 `this` 成为外围（词法）上下文时，请使用箭头函数


##### 附加链接


* [`this` on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)

</details>

<br>[⬆ 返回顶部](#目录)

### 诸如 React，Vue，Angular，Hyperapp 等 JavaScript UI 库/框架的目的是什么？

<details>
<summary>查看答案</summary>

只要的目的是避免直接操作 DOM 和更容易与 UI 保持状态同步。此外，它们提供了创建组件的能力，可以被重复使用，它们拥有相似的功能，只有一些微小的差别，避免了当多次使用的组件的结构需要多个地方改变时，多次的重复改变

当类似 jQuery 操作 DOM 的库工作时，应用的数据维持在 DOM 本身，经常用类名或 `data` 属性。操作 DOM 来更新 UI 会包含许多额外的步骤和随着时间的推移会引入微小的 bug。保持状态分离和让框架来处理当状态改变时的 UI 更新，以减少认知负担。你想要 UI 看起来在状态时是某个值时以某种方式显示是创建一个应用的声明式方式，而不是操作更新 UI 来反映新状态的命令式方式


#### 小贴士


* 虚拟 DOM 是用普通对象表式一个真实 DOM 树的形式，允许一个库编写代码,就像整个文档在每个改变时抛出重建，当真实 DOM 需要改变时才更新。比较新旧虚拟 DOM 更高效 ，相比重新计算虚拟 DOM，改变真实 DOM 节点开销更大 
* JSX 是 JavaScript 提供类似 XML 语法的一种扩展，用来创建虚拟 DOM 对象，通过一个转换器转换为函数调用。它比标签模板字面量简化了控制流（`if` 语句/三元表达式）


##### 附加链接


* [Virtual DOM in Hyperapp](https://github.com/hyperapp/hyperapp#view)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 “严格模式”，它带来哪些关键性的好处？

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

虚拟 DOM（VDOM）是一个用 JavaScript 普通对象形式表示真实 DOM的表现。这些对象使用属性来描述真实 DOM 节点：节点名称，它的属性，和子节点们 

```html
<div class="counter">
  <h1>0</h1>
  <button>-</button>
  <button>+</button>
</div>
```

上面用虚拟 DOM 表示出来可能看起来如下：

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

库/框架使用虚拟 DOM 来提高性能。当应用状态发生改变时，真实 DOM 需要更新来反映它。然而，改变真实 DOM 节点比重新计算虚拟 DOM 花费更高，开销更大。旧虚拟 DOM 和新虚拟 DOM 的比较非常快

一旦旧虚拟 DOM 和新虚拟 DOM 在框架的 diff 引擎下计算出变化，就会尽可能的以最快的有效的方式附加到真实的 DOM 上来匹配应用的新状态


#### 小贴士


* 为何访问 DOM 会如此昂贵


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

当几个组件需要分享数据时，它更推荐把共享状态提升到它们最近的公共祖先。例如，如果两个组件共享相同数据时，更推荐将共享状态移到它们的父组件，而不是在各自子组件内部维护


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
  嗨 {用户}, 写些酷酷的注释吧
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

在 `setState` 设置完成和组件渲染完时，会调用这个回调函数。因为 `setState` 是异步操作，所以这个回调函数可以用来做任何 post 操作

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

* 在 HTML 中，`return false` 可以阻止默认行为发生，然而在 React 中，必须显示调用 `preventDefault` 才能阻止默认行为

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

`key` 是一个特殊属性帮助 React 区分哪些元素是已经修改的，添加的，或移除的。当渲染数组元素时，它们提供一个稳定的标识。每一个元素的 `key` 必须时唯一的（例如，ID 用数据或索引作为最后选择）

```jsx
const todoItems = todos.map(todo => <li key={todo.id}>{todo.text}</li>)
```

* 使用索引作为顺序可变元素的 `key` 并不推荐，因为可能对性能带来负面影响，而且可能造成组件状态问题
* 如果你把列表项提取为一个组件，你应该把 `key` 绑定到列表（例如，`<ul>`，`<ol>`）上，而不是 `<li>` 标签上


#### 小贴士


* `key` 给予集合中的元素一个稳定的标识，帮助 React 区分改变
* 如果你的元素顺序是可变的，最好避免使用索引作为 `key` 
* 如果你把列表提取为一个组件时，你应该把 `key` 提升到组件上，而不是 `<li>` 元素


##### 附加链接


* [React docs on Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)

</details>

<br>[⬆ 返回顶部](#目录)

### React 里的生命周期有哪些？

<details>
<summary>查看答案</summary>

`getDerivedStateFromProps`: 在初始挂载和所有组件更新渲染之前执行。用于随着 props 的改变更新 state。有很少的使用情况，像在生命周期中跟踪组件动画。它们只有很少的例子，在其他生命周期方法使用是有意义的。它期望返回一个对象用来设置新的 state，或者返回 `null` 是什么也不会更新。这个方法还不能访问组件实例

`componentDidMount`: 在第一渲染之后执行，这里可以发送所有 AJAX 请求，DOM 或 state 的更新，和设置事件监听器

`shouldComponentUpdate`: 决定是否更新组件。默认情况下，它返回 `true`。如果你确定在 state 或 props 更新之后组件不需要重新渲染的话，你可以返回一个假值。它是提升性能的好地方，允许你在组件接受的新的 prop 时阻止组件重新渲染

`getSnapshotBeforeUpdate`: 在 `componentDidUpdate` 之前的更新将导致组件渲染之后立即调用，返回的任何值将会传给 `componentDidUpdate`

`componentDidUpdate`: 大多数用于更新 DOM 来响应 prop 或 state 的改变

`componentWillUnmount`: 它将取消任何已经发出的网络请求，或移除所有与组件关联的事件监听器

`componentDidCatch`: 在错误边界（实现这个方法的组件）里使用。它允许组件捕获子组件树（这个组件之下）任何地方的 JavaScript 错误，记录错误，并且用 UI 的信息的形式展示出来


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

相比 `findDOMNode()` API，回调 `refs` 更推荐使用，由于实际上 `findDOMNode()` 阻止了 React 未来的某些确定的改进

```jsx
/* 使用遗留方法 findDOMNode() */
class MyComponent extends Component {
  componentDidMount() {
    findDOMNode(this).scrollIntoView()
  }

  render() {
    return <div />
  }
}

/* 更推荐使用 回调 refs */
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


* 回调 `refs` 比 `findDOMNode()` 更推荐使用


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

### 在 React 中，什么是 `context`？

<details>
<summary>查看答案</summary>

`Context` 提供了一种无需手动在组件树每层都通过 `props` 传递数据的方式。例如，在应用中许多组件要访问用户授权，地区首选项，UI 主题

```jsx
const { Provider, Consumer } = React.createContext(defaultValue)
```


#### 小贴士


* `Context` 提供了一种通过 React 组件树传递数据的方式，而不需要手动传递 `props`
* `Context` 是被设计用来共享数据（对于 React 组件树来说的全局数据）


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

### 在 React 类方式定义的组件中，你如何保证方法得到的 `this` 是正确的？

<details>
<summary>查看答案</summary>

* 在 JavaScript 类中，方法不是默认被绑定的。这就意味着它们 `this` 上下文可以被改变（在事件处理例子里，指向监听事件的那个元素）和将不会指向组件实例。为了解决这个问题，`Function.prototype.bind()` 可以强制把 `this`  上下文绑定到组件实例上

```jsx
constructor(props) {
  super(props);
  this.handleClick = this.handleClick.bind(this);
}

handleClick() {
  // 执行一些逻辑
}
```

* `bind` 方法可能是冗长的，而且必须在 `constructor` 中定义，因此更推荐新的公共类字段语法：

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

* 你也可以使用内联箭头函数，因为词法 `this`（指向组件实例） 被保留里下来：

```jsx
<button onClick={e => this.handleClick(e)}>Click me</button>
```

注意重新渲染会被发生，由于在渲染期间又创建了新的函数，它会破坏 `shouldComponentUpdate` / `PureComponent` 的浅比较来阻止重新渲染。在性能很重要的情况下，优先使用在构造器中使用 `bind`，或者使用公共类字段语法方法，因为函数引用保持不变


#### 小贴士


* 你要么使用在构造器中用 `bind` 方法绑定组件实例，使用公共类方法字段语法，要么使用内联箭头函数


##### 附加链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)
* [React docs on Passing Functions to Components](https://reactjs.org/docs/faq-functions.html#how-do-i-bind-a-function-to-a-component-instance)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 中，`portals` 是什么？

<details>
<summary>查看答案</summary>
Portal 是一种子组件存在于父组件的 DOM 结构层级外的渲染推荐方式

```jsx
ReactDOM.createPortal(child, container)
```

第一个参数（`child`）是可渲染的 React 子元素，例如，一个元素，字符串或文档片段。第二个参数（`container`）是一个 DOM 元素


#### 小贴士




##### 附加链接


* [React docs on Portals](https://reactjs.org/docs/portals.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 在 React 中，如何校验 `prop`？

<details>
<summary>查看答案</summary>

当应用运行在开发模式下时，React 会自动检查我们在组件上设置的所有 `props` 以确保它们得到的是正确的数据类型。对于不正确的数据类型，在开发模式下它将在控制台产生一个警告信息，然而由于性能的影响它在生产模式下是禁用的。必选的 `prop` 需要定义 `isRequired`

预定义的 `prop` 类型如下：

-`PropTypes.string` -`PropTypes.number` -`PropTypes.func` -`PropTypes.node` -`PropTypes.bool`

例如，我们可以在组件上如下这么定义：

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


* 我们可以自己自定义 `PropTypes`
* 使用 `PropTypes` 不是强制的，但这是最佳实践


##### 附加链接



</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 `refs`，我们如何使用它？

<details>
<summary>查看答案</summary>

Refs 提供一种在 render 方法中访问 DOM 节点或 React 元素的方法。Refs 应该少用，但是有一些好的使用例子，例如：

* 管理获取焦点，文本选择，或者媒体回放
* 触发不可避免的动画
* 集成三方 DOM 库

用 `React.createRef()` 创建一个引用，然后通过 `ref` 属性附到 React 元素上。为了贯穿整个组件使用 refs，需要在构造器中注册 `ref` 的实例：

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

Refs 也可以在闭包的帮助下在函数式组件下使用


#### 小贴士


* Refs 用来返回一个元素的引用
* Refs 不应该被过渡使用
* 你可以用 `React.createRef()` 创建一个引用，然后通过 `ref` 属性附到 React 元素上


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

浏览器有一个临时的存储网站文件的缓存，所以他们不需要在切换或重新加载同一个页面时再次重新下载。服务器设置发送头信息告诉浏览器在给定的一段时间内使用存储文件。这极大加快了网站的速度和节省了带宽

然而，当开发人员网站更新时，因为用户的缓存依然指向旧的文件，这会造成问题。如果缓存的 CSS 和 JavaScript 文件引用的元素不再存在，已移除或已重命名时，它会保留原有功能或破坏网站

禁用缓存是一个强制浏览器下载新文件的过程。通过命名来区分于旧文件

一个常用的强制浏览器重新下载文件的技术是在文件的结尾处增加一个查询字符串

* `src="js/script.js"` => `src="js/script.js?v=2"`

浏览器认为这是一个不同的文件但是避免了修改文件名的必要


#### 小贴士

##### 附加链接


* [Strategies for cache-busting CSS](https://css-tricks.com/strategies-for-cache-busting-css/)

</details>

<br>[⬆ 返回顶部](#目录)

### 一个页面里是否可以包含多个 `<header>` 元素， `<footer>` 元素呢？

<details>
<summary>查看答案</summary>

都可以。W3C 文档声明这些标签代表离它们最近祖先区域的页眉（`<header>`）和页脚（`<footer>`）。因此，不只是可以在页面的 `<body>` 里包含页眉和页脚，而且每一个 `<article>` 和 `<section>` 元素都可以包含


#### 小贴士


* W3C 推荐你想用多少就用多少，但是每一个页面的区域只能有一个，即，body，section 等等

##### 附加链接


* [StackOverflow Using header or footer tag twice](https://stackoverflow.com/questions/4837269/html5-using-header-or-footer-tag-twice?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa)

</details>

<br>[⬆ 返回顶部](#目录)

### 简明的阐述下 HTML5 语义标签 `<header>`，`<article>`，`<section>`，`<footer>` 的用法

<details>
<summary>查看答案</summary>

* `<header>` 是被用来包含介绍和导航信息页面的一部分。这部分包含章节标题，作者姓名，发布日期和时间，目录，或其他导航信息

* `<article>` 是一个逻辑独立的复合体，可以在页面外部重新创建而不会失去其意义。个人博客文章或新闻故事就是很好的例子

* `<section>` 是一个灵活的容器，用来保存分享公共信息主题或目的的内容

* `<footer>` 是被用来保存应该显示内容部分的尾部信息和这个章节的附加信息。作者的姓名，版权信息，和相关链接就是典型的例子


#### 小贴士


* 其他的语义化元素 `<form>` 和 `<table>`


##### 附加链接


* [HTML 5 Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)

</details>

<br>[⬆ 返回顶部](#目录)

### `<script>` 标签的 `defer` 和 `async` 是什么？

<details>
<summary>查看答案</summary>

如果两个属性都没有的话，脚本将同步下载和执行，并且会阻塞 document 解析，直到脚本执行完成（默认行为）。脚本下载和执行按它们书写的顺序进行

`defer` 属性在 document 解析的过程中下载脚本，但是在 document 解析完成之前执行，等价于执行了一个内置的事件监听器 `DOMContentLoaded`。`defer` 脚本顺序执行

`async` 属性在 document 解析过程中下载脚本，但是会暂停解析器，直到脚本解析执行完成。`async` 不一定按顺序执行

注意：两个属性必须在脚本拥有 `src` 属性时才起作用（即，在内联脚本不起作用）

```html
<script src="myscript.js"></script>
<script src="myscript.js" defer></script>
<script src="myscript.js" async></script>
```


#### 小贴士


* 请用 `<head>` 中放置一个 `defer`，允许浏览器在页面还在解析过程中下载脚本，因此把脚本放到 `body` 之前是更好的选择
* 如果脚本之间相互依赖，请用 `defer`.
* 如果脚本是独立的，请用 `async`.
* 如果 DOM 必须加载完并且内容还未放置到 `DOMContentLoaded` 监听器中时，请用 `defer` 


##### 附加链接


* [async vs defer attributes](http://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是 `DOM`？

<details>
<summary>查看答案</summary>

DOM（Document Object Model，文档对象模型）是一个跨平台的 API，将 HTML 和 XML 文档视为一个节点组成的数结构。这些节点（例如，元素和文本节点）是可编程的对象，并且任何的改变都会反射到文档中。在一个浏览器，这个 API 对于 JavaScript 是可用的，DOM 节点可以被操作来改变它们在文档中的样式，内容，位置，或者交互的事件监听器


#### 小贴士


* DOM 被设计为是一个独立于任何流行编程语言，使文档从一个单一的，一致的 API 可获得的结构表现
* 当页面加载时，DOM 在浏览器中是渐进式的构建T，这就是为何脚本通常放置在页面的底部，在 `<head>` 带着 `defer` 属性，或者在 `DOMContentLoaded` 监听器的内部。脚本应该在 DOM 加载完操作 DOM 节点，以避免发生错误
* `document.getElementById()` 和 `document.querySelector()` 是常用的 DOM 节点查找函数
* 设置一个新值给 `innerHTML` 属性，通过 HTML 解析器来执行这个字符串，提供一个更方便的方法来给节点添加动态的 HTML 内容


##### 附加链接


* [MDN docs for DOM](https://developer.mozilla.org/en-US/docs/DOM)

</details>

<br>[⬆ 返回顶部](#目录)

### 讨论下 HTML 规范和浏览器实现之间的区别？

<details>
<summary>查看答案</summary>

HTML 规范，例如 `HTML5` 定义一个规则集，一个文档必须遵守为了根据规范达到 “有效”。此外，一个规范提供了一个浏览器如何解析和渲染一个文档的说明

如果浏览器有效的根据规范处理文档，那个就称为 “支持” 这个规范。至今，还没有所有浏览器实现了 `HTML5` 规范的所有部分（尽管大部分主流浏览器支持大多数规范），结果是，它需要开发者确认他们使用的是否支持所有浏览器来显示他们希望显示的内容。这就是为何对于开发者来说跨浏览器支持仍然是一个头疼的问题，即使改进了规范

#### 小贴士


* `HTML5` 为非法的 `HTML5` 文档定义了一些规则（即，包含语法错误）
* 然而，非法文档可能包含任何东西，因此规范不可能全面地处理所有的可能性
* 因此，许多畸形的文档处理决定就交给了浏览器


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

### 什么时候和为什么使用 `rel="noopener"` 属性？

<details>
<summary>查看答案</summary>

`rel="noopener"`是 `<a>` 元素（超链接）的一个属性。它阻止页面拥有 `window.opener` 属性，否则它将指向源页面（超链接所在的页），并且允许操作源页面


#### 小贴士


* `rel="noopener"` 应用于超链接
* `rel="noopener"` 阻止已打开的页面操作源页面

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

BEM 方法论是一个CSS 类的命名约定，为了更好的维护，通过定义命名空间来解决作用域的问题。BEM 代表 Block（块），Element（元素），Modifier（修饰符），这是对它结构的解释。 一个 Block（块）是单独组件，可以跨项目使用，而且它作为子组件（Element（元素））的命名空间。Modifier（修饰符）被用来标识一个 Block（块）或 Element（元素）是某个状态或不同结构或样式

```css
/* 块 组件 */
.block {
}

/* 元素 */
.block__element {
}

/* 修饰符 */
.block__element--modifier {
}
```

有一个标记类名的例子：

```html
<nav class="navbar">
  <a href="/" class="navbar__link navbar__link--active"></a>
  <a href="/" class="navbar__link"></a>
  <a href="/" class="navbar__link"></a>
</nav>
```

在这个例子中，`navbar` 是 Block（块），`navbar__link`是一个在 `navbar` 组件外部毫无意义的 Element（元素），`navbar__link--active` 是一个修饰符代表 `navbar__link` Element（元素）的不同状态

因为修饰符太啰嗦，大多选择使用 `is-*` 标识代替修饰符

```html
<a href="/" class="navbar__link is-active"></a>
```

这样必须使用链式到 Element（元素）后，不能单独使用，否则将出现作用域问题

```css
.navbar__link.is-active {
}
```


#### 小贴士


* 一个可替换的选择解决方案就是使用像 CSS-in-JS 这种


##### 附加链接


* [Writing clean and maintainable CSS](https://hackernoon.com/writing-clean-and-maintainable-css-using-bem-methodology-1dcbf810a664)

</details>

<br>[⬆ 返回顶部](#目录)

### 用 CSS 预处理的优势是什么？

<details>
<summary>查看答案</summary>

CSS 预处理器添加了原生 CSS 所不能做的有用的功能，而且通过使用 DRY（Don't Repeat Yourself，不要重复造轮子）规则生成更整洁的和可维护的 CSS。它们简洁的嵌套的选择器语法削减了重复的代码。对于一致的主题，它们提供了变量（然而，CSS 变量已经很大程度上可以替代这个功能了）和附加的工具，比如颜色函数（`lighten`, `darken`, `transparentize`, 等等），还有混合和循环功能，使得 CSS 更像一个真实的编程语言，赋予开发者更多能力去实现复杂的 CSS


#### 小贴士


* 它们允许我们编写更易维护和可扩展的 CSS
* 使用 CSS 预处理器的缺点（设置，重新编译可能会很慢）


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

### `em` 和 `rem` 单位的区别？

<details>
<summary>查看答案</summary>

`em` 和 `rem` 单位都是 CSS 属性 `font-size` 的基础。它们的唯一区别是它们的继承来源

* `em` 单位继承自它的父元素 `font-size` 的值
* `rem` 单位继承自根元素（`html`） `font-size` 的值

在多大数浏览器中，根元素的 `font-size` 默认设置为 `16px`


#### 小贴士


* 使用 `em` 和 `rem` 单位的好处


##### 附加链接


* [CSS units for font-size: px | em | rem](https://medium.com/code-better/css-units-for-font-size-px-em-rem-79f7e592bb97)

</details>

<br>[⬆ 返回顶部](#目录)

### CSS 雪碧图的优势在哪里，如何使用？

<details>
<summary>查看答案</summary>

CSS 雪碧图把多个图片组合到一张图片中，限制了浏览器 HTTP 请求的数量，因此提升了加载速度。甚至在新的 HTTP/2 协议中，这仍然正确

在 HTTP/1.1 下，每个 TCP 连接最多允许一个请求。HTTP/1.1，现代浏览器可以打开多个并行连接，但有限制（2 到 8 个）。HTTP/2，所在浏览器和服务器之间的请求都可以使用一个单独的 TCP 连接多路复用。这就意味着打开和关闭多个连接的开销被减轻了，结果是更好的利用了 TCP 连接和限制了客户端和服务器之间的潜在影响。在同一个 TCP 连接中同步加载 10 张图片成为可能

然而，根据 [基准结果](https://blog.octo.com/en/http2-arrives-but-sprite-sets-aint-no-dead/)，尽管 HTTP/2 比 HTTP/1.1 提高了 50% 的性能，但大多树情况使用雪碧图比独立使用图片加载更快

为了在 CSS 使用雪碧图，可以使用某些属性，例如 `background-image`，`background-position` 和 `background-size` 根本上改变了元素的 `background`

#### 小贴士


* `background-image`，`background-position` 和 `background-size` 可以使用于一个雪碧图中


##### 附加链接


* [CSS Sprites explained by CSS Tricks](https://css-tricks.com/css-sprites/)

</details>

<br>[⬆ 返回顶部](#目录)

###  CSS 里通用兄弟选择器和相邻兄弟选择器的区别？

<details>
<summary>查看答案</summary>

通用兄弟选择器 `~` 会选择指定元素的所有兄弟元素

下面的例子会选择 `<div>` 元素的所有 `<p>` 兄弟元素：

```css
div ~ p {
  background-color: blue;
}
```

相邻兄弟选择器 `+` 会选择指定元素的相邻兄弟元素

下面的例子会选择紧接在 `<div>` 元素后的 `<p>` 元素：

```css
div + p {
  background-color: red;
}
```

#### 小贴士


##### 附加链接


* [W3School's CSS Combinators Page](https://www.w3schools.com/css/css_combinators.asp)
* [Mozilla's Combinators and groups of selectors page](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors)

</details>

<br>[⬆ 返回顶部](#目录)

### 你能描述下 CSS 优先级是如何工作的？

<details>
<summary>查看答案</summary>

假设浏览器已经定义好了元素的规则集，为每一个元素分配一个矩阵值，它的优先级从高到低对应如下：

* 内联规则（二进制 1 或 0）
* id 选择器的数量
* 类选择器，伪类选择器和属性选择器的数量
* 标签选择器和伪元素选择器的数量

当两个选择器进行比较，比较设计基于每一列的基础上（例如，一个 id 选择器永远比 任何数量的类选择器级别高，id 比类选择器拥有更高优先级）。在多个级别相等的多个规则中，出现在页面样式表的最后那个规则被认为优先级更高，因此它会应用于元素上


#### 小贴士


* 优先级矩阵：[内联，id，类/伪类/属性，标签/伪元素]
* 在相同级别的情况下，后面的规则优先

##### 附加链接


* [CSS Specificity](https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/)

</details>

<br>[⬆ 返回顶部](#目录)

### 什么是聚焦环，正确的解决方案是什么？

<details>
<summary>查看答案</summary>

当使用按钮或链接标签获得焦点时，会得到一个可见的外边框，这就是聚焦环。它的种类依赖于根据浏览器提供商，但通常会显示一个蓝色的外边框包围在元素的周围，以表明它当前获得了焦点

在过去，许多人指定 `outline: 0;` 来去除元素上的聚焦环。然而，由于不可见会对键盘用户访问性造成困扰。当不指定时，它会形成一个不吸引人的蓝色环显示在元素周围

在最近，像 Bootstrap 之类的框架有一个选择，就是通过使用一个更吸引人的 `box-shadow` 外边框替代默认的聚焦环。然而，对鼠标用户仍不完美

最好的解决方案是一个即将到来的伪类选择器 `:focus-visible`，今天它仍需要 JavaScript 打补丁才能实现。它只会出现在用户在使用键盘时，并且对于鼠标用户会在失去焦点后隐藏。它同时保留了鼠标用户的美学和键盘用户的可访问性


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
    // 处理错误，return 在这里非常重要，因此执行在这里终止
    return console.log(err)
  }
  // 使用 data 对象
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

### 什么是 `REST`？

<details>
<summary>查看答案</summary>

RSET（REpresentational State Transfer 表述性状态转移）是一个用于网络架构的软件设计模式。一个 RESTful web 应用以它的资源信息形式公开数据

通常，这个概念用于 web 应用管理状态。在大多数应用中，有一个共同的内容，查，增，改，删数据。数据被模块化的分割为表，像 `posts`，`users`，`comments`，一个 RESTful API 以这种形式公开访问数据：

* 一个资源的 id。被认为是资源的端点或 URL
* 服务器应该按照这个资源的 HTTP 方法或动词来执行相应操作。常用的 HTTP 方法有 GET，POST，PUT，和 DELETE

这有一个带有 `posts` 资源的 URL 和 HTTP 方法的例子：

* 查：`/posts/` => GET
* 增：`/posts/new` => POST
* 改：`/posts/:id` => PUT
* 删：`/posts/:id` => DELETE


#### 小贴士


* 可以用如 GraphQL 模式替换


##### 附加链接


*   ](https://medium.com/extend/what-is-rest-a-simple-explanation-for-beginners-part-1-introduction-b4a072f8740f)

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


## 安全
### 什么是跨站脚本攻击（XSS），你是如何阻止它的？

<details>
<summary>查看答案</summary>

XSS 指的是客户端代码注入，攻击者在一个合法网站或 web 应用注入恶意脚本。它得以实现的原因通常是应用没有校验用户的输入和自由注入动态的 HTML 内容

例如，一个评论系统如果不对用户的输入做校验或转义的话，将处于风险中。如果评论内容包含未转义的 HTML，评论里可以注入一个 `<script>` 标签到网站中，那么该网站的其他用户在它们看到这条评论时就会再次执行

* 恶意的脚本可以获取到 cookie（通常用来存储 session 的令牌）。如果攻击者可以获取到用户的会话 cookie 的话，他们就可以模仿用户登陆
* 脚本可以任意操控正在执行的脚本的页面的 DOM，允许攻击者插入看起来是真实网站的一部分的内容
* 脚本可以使用 AJAX 携带任意内容发送 HTTP 请求到任意的地方


#### 小贴士


* 在客户端，使用 `textContent` 替代 `innerHTML`，阻止浏览器运行通过 HTML 解析器执行其中的脚本的字符串
* 在服务端，转义 HTML 标签来阻止浏览器解析用户实际输入的 HTML，因此也不会执行脚本


##### 附加链接


* [Cross-Site Scripting Attack (XSS)](https://www.acunetix.com/websitesecurity/cross-site-scripting/)

</details>

<br>[⬆ 返回顶部](#目录)


## 协议

[MIT](LICENSE). Copyright (c) [Stefan Feješ](https://stefanfejes.com/).





> - 本文仅代表原作者个人观点，译者不发表任何观点
> - Markdown 文件由译者手动整理，如有勘误，欢迎指正
> - 译文和原文采用一样协议，侵删
