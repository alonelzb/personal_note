# 创建 JavaScript 对象

JavaScript 对象就是一个 **name:value** 集合。

> 在 JavaScript 中，几乎所有的对象都是 Object 类型的实例，它们都会从 Object.prototype 继承属性和方法

1. 使用 Object 定义并创建对象的实例。
2. 使用函数来定义对象，然后创建新的对象实例。

JavaScript for...in 语句循环遍历对象的属性。

## 对象属性

> 可以说 "JavaScript 对象是变量的容器"。
>
> 但是，我们通常认为 "JavaScript 对象是键值对的容器"。
>
> 键值对通常写法为 **name : value** (键与值以冒号分割)。
>
> 键值对在 JavaScript 对象通常称为 **对象属性**。
>
> 对象键值对的写法类似于：
>
> - PHP 中的关联数组
> - Python 中的字典
> - C 语言中的哈希表
> - Java 中的哈希映射
> - Ruby 和 Perl 中的哈希表

# 类？

JavaScript 是面向对象的语言，但 JavaScript 不使用类。

在 JavaScript 中，不会创建类，也不会通过类来创建对象（就像在其他面向对象的语言中那样）。

JavaScript 基于 prototype，而不是基于类的。

# JavaScript 的对象是可变的

https://www.runoob.com/js/js-object-prototype.html

对象是可变的，它们是通过引用来传递的。

以下实例的 person 对象不会创建副本：

```javascript
var x = person;  // 不会创建 person 的副本，是引用

// 如果修改来 x ，person 的属性也会改变：
var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"}
var x = person;
x.age = 10;           //  x.age 和 person.age 都会改变
```

# JavaScript prototype（原型对象）

所有的 JavaScript 对象都会从一个 prototype（原型对象）中继承属性和方法。

# string 对象

字符串可以是引号中的任意文本。您可以使用单引号或双引号：

字符串使用 indexOf() 来定位字符串中某一个指定的字符首次出现的位置：

如果没找到对应的字符函数返回-1

**match()**函数用来查找字符串中特定的字符，并且如果找到的话，则返回这个字符。

属性:

- length
- prototype
- constructor

方法:

- charAt()
- charCodeAt()
- concat()
- fromCharCode()
- indexOf()

# Date（日期） 对象

getTime() 返回从 1970 年 1 月 1 日至今的毫秒数。

# Array（数组） 对象

创建一个数组，有三种方法。

1: 常规方式:

var myCars=new Array();
myCars[0]="Saab";   
myCars[1]="Volvo";
myCars[2]="BMW";

2: 简洁方式:

var myCars=new Array("Saab","Volvo","BMW");

3: 字面:

var myCars=["Saab","Volvo","BMW"];

# Boolean（布尔）对象

用于将非布尔值转换为布尔值（true 或者 false）。

如果布尔对象无初始值或者其值为:

- 0
- -0
- null
- ""
- false
- undefined
- NaN

那么对象的值为 false。否则，其值为 true（即使当变量值为字符串 "false" 时）！

