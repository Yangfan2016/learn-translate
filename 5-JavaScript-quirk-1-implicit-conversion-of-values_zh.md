## JavaScript 怪异 1：值的隐式转换

> - 原文地址：https://2ality.com/2013/04/quirk-implicit-conversion.html
> - 原文作者：[Dr. Axel Rauschmayer](https://github.com/rauschma)
> - Markdown 地址：https://github.com/Yangfan2016/learn-translate/blob/master/5-JavaScript-quirk-1-implicit-conversion-of-values.md
> - 译者：[Yangfan2016](https://github.com/Yangfan2016)


#### 这篇文章是 JavaScript 怪异[系列](http://2ality.com/2013/04/12quirks.html)的一部分

JavaScript 是对值的接受是非常宽松的。例如在任何期待一个 number 类型的值的地方，它不会拒绝来自其他类型的值，而是会试图转换它们：

```js
> '5' - '2'
3
> '5' * '2'
10
```

自动转换成 boolean 值是很少出问题并且很有用。这里先埋下个伏笔（我们将用它解决一些怪异问题）。然而，自动转换为 string 可能会造成一些问题

### 1. 隐式转换为 boolean 值：“truthy” 还是 “falsy”

不管何时 JavaScript 接受一个 boolean 值时（例如，if 语句的条件），任何值都可以用。它要么解释为 true，要么解释为 false。下面的值都会被解释为 false：

```js
undefined, null
Boolean: false
Number: -0, +0, NaN
String: ''
```

其他所有的值都会被当作 true。值被解释为 false 的称作 falsy（假值），值被解释为 true 的称作 truthy（真值）。你可以使用 Boolean 函数来测试一个值会被解释为什么。它会把它的参数转换为 boolean 值：
    
```js    
> Boolean(undefined)
false
> Boolean(0)
false
> Boolean(3)
true
```

### 2. string 的隐式转换

在 web 开发中，你会经常获取到实际上是 number 或 boolean 而当作 string 类型的值。例如，当用户在表单输入一些数据时。如果你忘记了显式转换这些 string 的话，JavaScript 会给你带来两个消极方面的惊喜：首先，不会有任何警告。其次，值会被自动转换，但是是错的。例如，操作符加号（+）就有问题，因为只要操作符的一边是 string 类型的，它就会当成字符串连接符。在下面的例子中，假设我们执行的是 1 和 5 相加，而实际上，我们执行的是 ‘1’ 和 ‘5’ 字符串连接

```js
> var x = '5';  // 错误假设：x 是 number 类型
> x + 1
'51'
```

此外，还有一些极少数的 falsy 值，如果被转换为 string 类型的，就会被当成 truthy，例如：false

```js
> Boolean(false)  // truthy?
false
> String(false)
'false'
> Boolean('false')  // truthy?
true
```


例如：undefined

```js
> Boolean(undefined)  // truthy?
false
> String(undefined)
'undefined'
> Boolean('undefined')  // truthy?
true
```


### 3. object 的隐式转换

如果 JavaScript 期待的是 number 或 string 类型的值的时候，object 才会发生隐式转换。第一种情况下（期待 number），会按照三个步骤进行转换：

1. ~~调用 valueOf() 方法，如果结果是原始类型（非 object），那么继续调用 ToNumber~~
2. ~~否则，调用 toString() 方法。如果结果是原始类型，那么继续那么继续调用 ToNumber~~
3. ~~否则，抛出一个 TypeError 错误~~


> 译者改：  
0. 调用 ToPrimitive， 如果是原始类型，直接返回
1. 调用 valueOf() 方法，如果结果是原始类型，那么继续调用 ToNumber
2. 否则，调用 toString() 方法。如果结果是原始类型，那么继续调用 ToNumber
3. 否则，抛出一个 TypeError 错误

> 译者注：这里注意 Date 对象（object）特殊，valueOf 和 toString 调用顺序不同

![note](https://user-gold-cdn.xitu.io/2019/7/26/16c2e51e8f21f5b0?w=1696&h=274&f=png&s=116000) 


第 1 步的例子：

```js
> 3 * { valueOf: function () { return 5 } }
15
```


第 3 步的例子：

```js
> function returnObject() { return {} }
> 3 * { valueOf: returnObject, toString: returnObject }
TypeError: 无法将 object 转换为原始类型
```

如果是 JavaScript 转换为 string 类型，那步骤 1 和步骤 2 进行交换：首先试图调用 toString() 方法，然后调用 valueOf() 方法

### 4. 最佳实践：显式转换

最好的办法是在使用它们之前就显式转换为期望的类型。一个迷你的解决方案是用 Boolean()，Number() 和 String() 方法：

```js
function handleFormData(formData) {
    var givenName = String(formData.givenName);
    var age = Number(formData.age);
    ...
}
```

这些函数总会返回一个值（它们永远都不会抛出异常）。然而 Number() 函数在它不能转换一个值时会返回 `NaN` \[1\]：

```js
> Number('xyz')
NaN
> Number(undefined)
NaN
> Number(null)
0
> Number(true)
1
```

更详细的解决方案是在你转换这些值时，先检查下它们的格式（例如，人们不能把 ‘xyz’ 作为它们的年龄），如果不对，要采取适当的解决措施

### 5. 引用

1. [NaN and Infinity in JavaScript](https://2ality.com/2012/02/nan-infinity.html)




### 译者注

 
感谢@hsy0 的评论，原文作者这里没有讲清楚，毕竟一千个人一千个哈姆雷特，我们还是直接看标准吧 [ecma-262/6.0/#sec-toprimitive](https://www.ecma-international.org/ecma-262/6.0/#sec-toprimitive)  

其实真实转换过程如下（作者在另一篇文章中提到了，😂，和标准一致），就不翻译了  
> An object obj is converted to a number by calling ToPrimitive(obj, Number) and then applying ToNumber() to the (primitive) result.  
An object obj is converted to a number by calling ToPrimitive(obj, String) and then applying ToString() to the (primitive) result.


