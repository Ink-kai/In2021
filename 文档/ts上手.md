## [基础类型](https://www.tslang.cn/docs/handbook/basic##types.html)

+ 布尔值

+ 数字

  和JavaScript一样，TypeScript里的所有数字都是浮点数。 这些浮点数的类型是 `number`。 除了支持十进制和十六进制字面量，TypeScript还支持ECMAScript 2015中引入的二进制和八进制字面量

+ 字符串

+ 数组

+ 元组

+ 枚举

+ Any

  有时候，我们会想要为那些在编程阶段还不清楚类型的变量指定一个类型。 这些值可能来自于动态的内容，比如来自用户输入或第三方代码库。 这种情况下，我们不希望类型检查器对这些值进行检查而是直接让它们通过编译阶段的检查。 那么我们可以使用 `any`类型来标记这些变量

+ Void

  某种程度上来说，`void`类型像是与`any`类型相反，它表示没有任何类型。 当一个函数没有返回值时，你通常会见到其返回值类型是 `void`

+ Null 和 Undefined

  TypeScript里，`undefined`和`null`两者各自有自己的类型分别叫做`undefined`和`null`。 和 `void`相似，它们的本身的类型用处不是很大

+ Never

  `never`类型表示的是那些永不存在的值的类型。 例如， `never`类型是那些总是会抛出异常或根本就不会有返回值的函数表达式或箭头函数表达式的返回值类型； 变量也可能是 `never`类型，当它们被永不为真的类型保护所约束时

  never`类型是任何类型的子类型，也可以赋值给任何类型；然而，*没有*类型是`never`的子类型或可以赋值给`never`类型（除了`never`本身之外）。 即使 `any`也不可以赋值给`never

+ Object

  `object`表示非原始类型，也就是除`number`，`string`，`boolean`，`symbol`，`null`或`undefined`之外的类型。

  使用`object`类型，就可以更好的表示像`Object.create`这样的API

+ 类型断言

  通过*类型断言*这种方式可以告诉编译器，“相信我，我知道自己在干什么”。 类型断言好比其它语言里的类型转换，但是不进行特殊的数据检查和解构。 它没有运行时的影响，只是在编译阶段起作用。 TypeScript会假设你，程序员，已经进行了必须的检查

## [变量声明](https://www.tslang.cn/docs/handbook/variable##declarations.html)

## [接口](https://www.tslang.cn/docs/handbook/interfaces.html)
## [类](https://www.tslang.cn/docs/handbook/classes.html)

## [函数](https://www.tslang.cn/docs/handbook/functions.html)
## [泛型](https://www.tslang.cn/docs/handbook/generics.html)
## [枚举](https://www.tslang.cn/docs/handbook/enums.html)
## [类型推论](https://www.tslang.cn/docs/handbook/type##inference.html)
## [类型兼容性](https://www.tslang.cn/docs/handbook/type##compatibility.html)
## [高级类型](https://www.tslang.cn/docs/handbook/advanced##types.html)
## [Symbols](https://www.tslang.cn/docs/handbook/symbols.html)
## [迭代器和生成器](https://www.tslang.cn/docs/handbook/iterators##and##generators.html)
## [模块](https://www.tslang.cn/docs/handbook/modules.html)
## [命名空间](https://www.tslang.cn/docs/handbook/namespaces.html)
## [命名空间和模块](https://www.tslang.cn/docs/handbook/namespaces##and##modules.html)
## [模块解析](https://www.tslang.cn/docs/handbook/module##resolution.html)
## [声明合并](https://www.tslang.cn/docs/handbook/declaration##merging.html)
## [JSX](https://www.tslang.cn/docs/handbook/jsx.html)
## [装饰器](https://www.tslang.cn/docs/handbook/decorators.html)
## [Mixins](https://www.tslang.cn/docs/handbook/mixins.html)
## [三斜线指令](https://www.tslang.cn/docs/handbook/triple##slash##directives.html)
## [JavaScript文件类型检查](https://www.tslang.cn/docs/handbook/type##checking##javascript##files.html)