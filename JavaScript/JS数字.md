# JavaScript Number 对象

---

JavaScript 只有一种数字类型。

可以使用也可以不使用小数点来书写数字。

---

### JavaScript 数字

JavaScript 数字可以使用也可以不使用小数点来书写：

```
var pi = 3.14
var x = 34;
```

极大或极小的数字可通过科学（指数）计数法来写：

```
var y = 123e5; // 12300000
var z = 123e-5; // 0.00123
```

---

### 所有 JavaScript 数字均为 64 位


JavaScript 不是类型语言。与许多其他编程语言不同，JavaScript 不定义不同类型的数字，比如整数、短、长、浮点等等。

JavaScript 中的所有数字都存储为根为 10 的 64 位（8 比特），浮点数。

---

### 精度

整数（不使用小数点或指数计数法）最多为 15 位。

小数的最大位数是 17，但是浮点运算并不总是 100% 准确：

---

### 创建 Number 对象

```
var myNum=new Number(value);
var myNum=Number(value);
```

参数：参数 value 是要创建的 Number 对象的数值，或是要转换成数字的值。

返回值：当 Number() 和运算符 new 一起作为构造函数使用时，它返回一个新创建的 Number 对象。如果不用 new 运算符，把 Number() 作为一个函数来调用，它将把自己的参数转换成一个原始的数值，并且返回这个值（如果转换失败，则返回 NaN）。

---

### 数字对象属性和方法

属性：

* MAX VALUE
* MIN VALUE
* NEGATIVE INFINITIVE
* POSITIVE INFINITIVE
* NaN
* prototype
* constructor

方法：

* toExponential()
* toFixed()
* toPrecision()
* toString()
* valueOf()

| 属性 | 描述
|------|-----
| constructor | 返回对创建此对象的 Number 函数的引用
| MAX_VALUE | 可表示的最大的数
| MIN_VALUE | 可表示的最小的数
| NaN | 非数字值
| NEGATIVE_INFINITY | 负无穷大，溢出时返回该值
| POSITIVE_INFINITY | 正无穷大，溢出时返回该值
| prototype | 使您有能力向对象添加属性和方法

| 方法 | 描述
| toString | 把数字转换为字符串
| toLocaleString | 把数字转换为字符串，使用本地数字格式顺序
| toFixed | 把数字转换为字符串，结果的小数点后有指定位数的数字
| toExponential | 把对象的值转换为指数计数法
| toPrecision | 把数字格式化指定的长度
| valueOf | 返回一个 Number 对象的基本数字值

---
