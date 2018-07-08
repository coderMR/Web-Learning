# XHTML 语法

---

### 编写 XHTML 需要更纯净的 HTML 语法。

---

### 更多的 XHTML 语法规则：

* 属性名称必须小写
* 属性值必须加引号
* 属性不能简写
* 用 id 属性代替 name 属性
* XHTML DTD 定义了强制使用的 HTML 元素

---

### 属性名称必须小写

这是错误的：

```
<table WIDTH="100%">
```

这是正确的：

```
<table width="100%">
```

---

### 属性值必须加引号

这是错误的：

```
<table width=100%>
```

这是正确的：

```
<table width="100%">
```

---

### 属性不能简写

这是错误的：

```
<input checked>
<input readonly>
<input disabled>
<option selected>
<frame noresize>
```

这是正确的：

```
<input checked="checked" />
<input readonly="readonly" />
<input disabled="disabled" />
<option selected="selected" />
<frame noresize="noresize" />
```

下面是一个 HTML 的简写属性列表，以及在 XHTML 中的改写：

| HTML | XHTML
|------|------
| compact | compact="compact"
| checked | checked="checked"
| declare | declare="declare"
| readonly | readonly="readonly"
| disabled | disabled="disabled"
| selected | selected="selected"
| defer | defer="defer"
| ismap | ismap="ismap"
| nohref | nohref="nohref"
| noshade | noshade="noshade"
| nowrap | nowrap="nowrap"
| multiple | multiple="multiple"
| noresize | noresize="noresize"

---

### 用 id 属性代替 name 属性

HTML 4.01 针对下列元素定义 name 属性：a、applet、frame、iframe、img、map。

在 XHTML 中不鼓励使用 name 属性，应该使用 id 取而代之。

这是错误的：

```
<img src="picture.gif" name="picture1" />
```

这是正确的：

```
<img src="picture.gif" id="picture1" />
```

重要的兼容性提示：

应该在 '/' 符号前添加一个额外的空格，以使 XHTML 与当今的浏览器相兼容。

---

### 语言属性（lang）

lang 属性应用于几乎所有的 XHTML 元素。它定义元素内部的内容的所用语言类型。

如果在某元素中使用 lang 属性，就必须添加额外的  xml:lang，像这样：

```
<div lang="no" xml:lang="no">Heia Norge!</div>
```

---

### 强制使用的 XHTML 元素

所有 XHTML 文档必须进行文件类型声明（DOCTYPE declaration）。在 XHTML 文档中必须存在 html、head、body元素，而 title 元素必须位于在 head 元素中。

下面是一个最小化的 XHTML 文件模板：

```
<!DOCTYPE Doctype goes here>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>Title goes here</title>
</head>

<body>
</body>

</html>
```

提示：文件类型声明并非 XHTML 文档自身的组成部分。它并不是 XHTML 元素，也没有关闭标签。

提示：在 XHTML 中，&lt;html&gt; 标签内的 xmlns 属性是必须的。

---
