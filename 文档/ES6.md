ES6语法我只是过一遍，因为很多语法、方法都是新增的嘛，稍微记一下笔记

## 字符串新增方法

+ includes()：返回Boolean，表示是否找到字符串

+ startsWith()：返回Boolean，表示参数字符串是否在原字符串的头部

+ endsWith()：返回布尔值，表示参数字符串是否在原字符串的尾部。

+ repeat()：返回一个新字符串，表示将原字符串重复`n`次。

+ ES2017 引入了字符串补全长度的功能

  `padStart()`用于头部补全，`padEnd()`用于尾部补全。一共接受两个参数，第一个参数是字符串补全生效的最大长度，第二个参数是用来补全的字符串。

+ [ES2019](https://github.com/tc39/proposal-string-left-right-trim) 对字符串实例新增了`trimStart()`和`trimEnd()`这两个方法

  `trimStart()`消除字符串头部的空格，`trimEnd()`消除尾部的空格。它们返回的都是新字符串，不会修改原始字符串。

+ replace()：只能替换第一个匹配，返回一个新字符串，不会改变原字符串

+ replaceAll()：可以一次性替换所有匹配，返回一个新字符串，不会改变原字符串

## 数值扩展

+ `Number.isFinite()`用来检查一个数值是否为有限的（finite），即不是`Infinity`。
+ `Number.isNaN()`用来检查一个值是否为`NaN`。
+ ES6 将全局方法`parseInt()`和`parseFloat()`，移植到`Number`对象上面，行为完全保持不变
+ `Number.isInteger()`用来判断一个数值是否为整数

## 数组

+ Array.from()：用于将两类对象转为真正的数组：类似数组的对象（array-like object）和可遍历（iterable）的对象（包括 ES6 新增的数据结构 Set 和 Map）

+ Array.of()：用于将一组值，转换为数组。

+ coupyWithin()：在当前数组内部，将指定位置的成员复制到其他位置（会覆盖原有成员），然后返回当前数组。

  - target（必需）：从该位置开始替换数据。如果为负值，表示倒数。
  - start（可选）：从该位置开始读取数据，默认为 0。如果为负值，表示从末尾开始计算。
  - end（可选）：到该位置前停止读取数据，默认等于数组长度。如果为负值，表示从末尾开始计算。

+ find()：用于找出第一个符合条件的数组成员。它的参数是一个回调函数，所有数组成员依次执行该回调函数，直到找出第一个返回值为`true`的成员，然后返回该成员。如果没有符合条件的成员，则返回`undefined`。

  `find`方法的回调函数可以接受三个参数，依次为当前的值、当前的位置和原数组。

+ findIndex()：与`find`方法非常类似，返回第一个符合条件的数组成员的位置，如果所有成员都不符合条件，则返回`-1`。

+ fill()：使用给定值，填充一个数组。

+ ES6 提供三个新的方法——`entries()`，`keys()`和`values()`——用于遍历数组。

  唯一的区别是`keys()`是对键名的遍历、`values()`是对键值的遍历，`entries()`是对键值对的遍历。

+ includes()：返回一个布尔值，表示某个数组是否包含给定的值

+ flat()：用于将嵌套的数组“拉平”，变成一维的数组。该方法返回一个新数组，对原数据没有影响。

+ flatMap()：对原数组的每个成员执行一个函数（相当于执行`Array.prototype.map()`），然后对返回值组成的数组执行`flat()`方法。该方法返回一个新数组，不改变原数组。

## 对象新增方法

+ Object.is()：用来比较两个值是否严格相等，与严格比较运算符（===）的行为基本一致。
+ Object.assign()：用于对象的合并，将源对象（source）的所有可枚举属性，复制到目标对象（target）。
+ getOwnPropertyDescriptor()：ES5 的`Object.getOwnPropertyDescriptor()`方法会返回某个对象属性的描述对象（descriptor）。ES2017 引入了`Object.getOwnPropertyDescriptors()`方法，返回指定对象所有自身属性（非继承属性）的描述对象。
+ fromEntries()：用于将一个键值对数组转为对象。