# JavaScript 数据类型

---

### 字符串、数字、布尔、数组、对象、Null、Undefined

---

### JavaScript 拥有动态类型

JavaScript 拥有与 python 相似的动态类型，这意味着相同的变量可用作不同的类型：

```
var x                // x 为 undefined
var x = 6;           // x 为数字
var x = "Bill";      // x 为字符串
```

---

### JavaScript 字符串

字符串可以是引号中的任意文本。您可以使用单引号或双引号：

```
var carname="Bill Gates";
var carname='Bill Gates';
```

---

### JavaScript 数字

JavaScript 只有一种数字类型。数字可以带小数点，也可以不带：

```
var x1=34.00;      //使用小数点来写
var x2=34;         //不使用小数点来写
```

极大或极小的数字可以通过科学（指数）计数法来书写：

```
var y=123e5;      // 12300000
var z=123e-5;     // 0.00123
```

---

### JavaScript 布尔

```
var x=true
var y=false
```

---

### JavaScript 数组

```
var cars=new Array();
cars[0]="Audi";
cars[1]="BMW";
cars[2]="Volvo";
```

或者

```
var cars=new Array("Audi","BMW","Volvo");
```

或者 

```
var cars=["Audi","BMW","Volvo"];
```

---

### JavaScript 对象

对象由花括号分隔。在括号内部，对象的属性以名称和值对的形式 (name : value) 来定义。属性由逗号分隔：

```
var person={firstname:"Bill", lastname:"Gates", id:5566};
```

对象属性有两种寻址方式：

```
name=person.lastname;
name=person["lastname"];
```

---

### Undefined 和 Null

Undefined 这个值表示变量不含有值。

可以通过将变量的值设置为 null 来清空变量。

```
cars=null;
person=null;
```

---

### 声明变量类型

当您声明新变量时，可以使用关键词 "new" 来声明其类型：

```
var carname=new String;
var x=      new Number;
var y=      new Boolean;
var cars=   new Array;
var person= new Object;
```

JavaScript 变量均为对象。当您声明一个变量时，就创建了一个新的对象。

---

