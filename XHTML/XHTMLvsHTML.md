# XHTML 与 HTML 之间的差异

---

### 通过开始编写严格的 HTML，你可以为 XHTML 做好准备。

---

### 如何为 XHTML 做好准备

XHTML 与 HTML 4.01 标准没有太多的不同。

所以将你的代码升级至 4.01 是个不错的开始。

另外，你应该马上使用小写字母编写 HTML 代码，同时绝不要养成忽略类似 &lt;/p&gt; 标签的坏习惯。

---

### 最主要的不同：

* XHTML 元素必须被正确的嵌套。
* XHTML 元素必须被闭合。
* 标签名必须用小写字母。
* XHTML 文档必须拥有根元素。

---

### 元素必须被正确的嵌套

在 HTML 中，某些元素可以像这样彼此不正确的嵌套：

```
<b><i>This text is bold and italic</b></i>
```

在 XHTML 中，所有元素必须像这样彼此正确的嵌套：

```
<b><i>This text is bold and italic</i></b>
```

---

### XHTML 元素必须被关闭

非空标签必须使用结束标签。

这是错误的：

```
<p>This is a paragraph
<p>This is another paragraph
```

这是正确的：

```
<p>This is a paragraph</p>
<p>This is another paragraph</p>
```

---

### 空标签也必须被关闭

空标签也必须使用结束标签，或者其开始标签必须使用 /> 结尾。

这是错误的：

```
A break: <br>
A horizontal rule: <hr>
An image: <img src="happy.gif" alt="Happy face">
```

这是正确的：

```
A break: <br />
A horizontal rule: <hr />
An image: <img src="happy.gif" alt="Happy face" />
```

---

### XHTML 元素必须小写

XHTML 规范定义：标签名和属性对大小写敏感。

这是错误的：

```
<BODY>
<P>This is a paragraph</P>
</BODY>
```

这是正确的：

```
<body>
<p>This is a paragraph</p>
</body>
```

---

### XHTML 文档必须拥有一个根元素

所有的 XHTML 元素必须被嵌套于 &lt;html&gt; 根元素中。其余所有的元素均可有子元素。子元素必须是成对的且被嵌套在其父元素之中。基本的文档结构如下：

```
<html>
<head> ... </head>
<body> ... </body>
</html>
```

---
