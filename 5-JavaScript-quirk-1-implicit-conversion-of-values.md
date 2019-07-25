## JavaScript quirk 1: implicit conversion of values

> - 原文地址：https://2ality.com/2013/04/quirk-implicit-conversion.html
> - 原文作者：[Dr. Axel Rauschmayer](https://github.com/rauschma)
> - 译者：[Yangfan2016](https://github.com/Yangfan2016)


#### This post is part of a [series](http://2ality.com/2013/04/12quirks.html) on JavaScript quirks

JavaScript is very tolerant when it comes to accepting values. For example, everywhere it expects a number, it does not reject values from other types, but tries to convert them:

```
    > '5' - '2'
    3
    > '5' * '2'
    10
```

Automatic conversion to boolean is rarely problematic and often useful. It is covered here as a preparation for later – we’ll use it to work around quirks. Automatic conversion to string, however, can cause problems.

### 1. Implicit conversion to boolean: “truthy” and “falsy” values

Whenever JavaScript expects a boolean value (e.g. for the condition of an if statement), any value can be used. It will be interpreted as either true or false. The following values are interpreted as false:

```
undefined, null
Boolean: false
Number: -0, +0, NaN
String: ''
```

All other values are considered true. Values interpreted as false are called falsy, values interpreted as true are called truthy. You can use Boolean as a function to test how a value is interpreted. It converts its argument to boolean:
    
```    
    > Boolean(undefined)
    false
    > Boolean(0)
    false
    > Boolean(3)
    true
```

### 2. Implicit conversion of strings

In web development, you often get values as strings that are actually numbers or booleans. For example, when users enter this kind of data in a form. If you forget to explicitly convert these strings then JavaScript will surprise you negatively in two ways: First, there will be no warning. Second, the values will be converted automatically, but wrongly. The plus operator (+), for instance, is problematic, because it concatenates strings as soon as one of its operands is a string. During the following interaction with JavaScript, the assumption is that we are adding 1 to 5. Instead, we are concatenating the strings '5' and '1'.

```
    > var x = '5';  // wrong assumption: x is a number
    > x + 1
    '51'
```

Furthermore, there are a few falsy values that are truthy if converted to string. Example: false.

```
    > Boolean(false)  // truthy?
    false
    > String(false)
    'false'
    > Boolean('false')  // truthy?
    true
Example: undefined.
    > Boolean(undefined)  // truthy?
    false
    > String(undefined)
    'undefined'
    > Boolean('undefined')  // truthy?
    true
```


### 3. Implicit conversion of objects

Objects are only implicitly converted if JavaScript expects a number or a string. In the former case, the conversion takes three steps:

1. Call valueOf(). If the result is primitive (not an object) then use it and convert it to a number.
2. Otherwise, call toString(). If the result is primitive, use it and convert it to a number.
3. Otherwise, throw a TypeError.


Example for step 1:

```
    > 3 * { valueOf: function () { return 5 } }
    15
```


Example for step 3:

```
    > function returnObject() { return {} }
    > 3 * { valueOf: returnObject, toString: returnObject }
    TypeError: Cannot convert object to primitive value
```

If JavaScript converts to string, steps 1 and 2 are swapped: toString() is tried first, valueOf() second.

### 4. Best practice: explicit conversion

It is best to explicitly convert values to the desired types before using them. A minimal solution is to use the functions Boolean(), Number() and String():

```
    function handleFormData(formData) {
        var givenName = String(formData.givenName);
        var age = Number(formData.age);
        ...
    }
```

These functions always return a value (they never throw an exception). However, Number() returns the error value NaN \[1\] if it can’t convert a value:

```
    > Number('xyz')
    NaN
    > Number(undefined)
    NaN
    > Number(null)
    0
    > Number(true)
    1
```

A more elaborate solution would be to first check whether the value you are converting has the correct format (e.g. someone shouldn’t enter 'xyz' as their age) and to take appropriate measures if it doesn’t.

### 5. Reference

1. [NaN and Infinity in JavaScript](https://2ality.com/2012/02/nan-infinity.html)
