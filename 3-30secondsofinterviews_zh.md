<a href="https://30secondsofinterviews.org"><img src="https://github.com/30-seconds/30-seconds-of-interviews/raw/master/logo.jpg" alt="30 Seconds of Interviews logo"></a>

<h1 align="center">
  面试 30 秒
</h1>

<h4 align="center">一个面试常用的问题精选集，帮助你准备下一次面试</h4>


> - 原文地址：https://github.com/30-seconds/30-seconds-of-interviews/blob/master/README.md
> - 原文作者：https://github.com/fejes713  
> - 译者：[Yangfan2016](https://github.com/Yangfan2016)
> - 备注：删除了重复部分，整理和精简了原文档的索引部分

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

算法并不总是执行相同的操作，基于提供的数据变化。而一些例子会执行很快，而另一些例子，即使处理相同数量的元素也会很慢

在这些例子中，基本的时间是 1 个元素 = `1ms`

##### O(1)

```js
arr[arr.length - 1]
```

* 1000 个元素 = `1ms`

常数时间复杂度。无论数组有多少个元素，理论上执行的时间的相同（排除实际的变化）

##### O(N)

```js
arr.filter(fn)
```

* 1000 元素 = `1000ms`

线性时间复杂度。执行时间会随着数组元素的数量线性增加。如果 1000 个元素的数组执行这个函数需要 1ms，那么 7000 个元素的数组将需要执行 7ms。这是因为函数在返回结果之前必须迭代数组的所有元素

##### O([1, N])

```js
arr.some(fn)
```

* 1000 元素 = `1ms <= x <= 1000ms`

执行时间依赖于提供给函数的数据变化，它可能很快或很迟返回。最好的情况是 O(1)，最坏的情况是 O(N)

##### O(NlogN)

```js
arr.sort(fn)
```

* 1000 元素 ~= `10000ms`

浏览器通常在 `sort()` 里使用快速排序实现，而且快速排序的平均时间复杂度是 O(NlgN)。在大的集合下非常高效

##### O(N^2)

```js
for (let i = 0; i < arr.length; i++) {
  for (let j = 0; j < arr.length; j++) {
    // ...
  }
}
```

* 1000 元素 = `1000000ms`

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

* 1000 元素 = `Infinity` （实际上） ms

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

此外，闭包是唯一一种存储私有数据不能被外部访问的方式。它们是 UMD（
