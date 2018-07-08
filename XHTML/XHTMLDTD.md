# XHTML DTD

---

### XHTML 定义了三种文件类型声明

### 使用最普遍的 XHTML Transitional

---

### &lt;!DOCTYPY&gt; 是强制使用的。

一个 XHTML 文档有三个主要部分组成

* DOCTYPE
* Head
* Body

基本的文档结构是这样的：

```
<!DOCTYPE ...>
<html>
<head>
<title>... </title>
</head>
<body> ... </body>
</html>
```

在 XHTML 文档中，文档类型声明总是位于首行。

---

一个 XHTML 的实例

这是一个简单的 XHTML 文档：

```
<!DOCTYPE html
PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html>
<head>
<title>simple document</title>
</head>
<body>
<p>a simple paragraph</p>
</body>
</html>
```

文档类似声明定义文档的类型：

```
<!DOCTYPE html
PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

文档的其余部分类似 HTML：

```
<html>
<head>
<title>simple document</title>
</head>
<body>
<p>a simple paragraph</p>
</body>
</html>
```

---

### 三种文档类型声明

* DTD规定了使用通用标记语言（SGML）的网页的语法。
* 注入 HTML 这样的通用标记语言应该使用 DTD 来规定应用于某种特定文档中的标签的规则，这些规则包括一些列的元素和实体的声明。
* 在通用标记语言（SGML）的文档类型声明或 DTD 中，XHTML 被详细的进行了描述。
* XHTML DTD 使用精确到可被计算机读取的语言来描述合法的 XHTML 标记的语法和句法。

### 存在三种 XHTML 文档类型：

* STRICT（严格类型）
* TRANSITIONAL（过度类型）
* FRAMESET（框架类型）

---

### XHTML 1.0 的三种 XML 文档类型

### XHTML 1.0 规定了三种 XML 文档类型，以对应上述三种 DTD。

XHTML 1.0 Strict

```
<!DOCTYPE html
PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" 
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

在此情况下使用：需要干净的标记，避免表现上的混乱。请与层叠样式表配合使用。

XHTML 1.0 Transitional

```
<!DOCTYPE html
PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```

在此情况下使用：当需要利用 HTML 在表现上的特性是，并且当需要为那些不支持层叠样式表的浏览器编写 XHTML 时。

XHTML 1.0 Frameset

```
<!DOCTYPE html
PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd">
```

在此的情况下使用：需要使用 HTML 框架将浏览器窗口分割为两部分或更多框架时。
