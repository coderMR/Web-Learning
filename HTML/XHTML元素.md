# XHTML 元素

---

### XHTML 元素是以 XML 格式编写的 HTML 元素

---

### XHTML 元素语法规则

* XHTML 元素必须正确嵌套
* XHTML 元素必须始终关闭
* XHTML 元素必须小写
* XHTML 文档必须有一个根元素

---

### XHTML 元素必须正确嵌套

在 HTML 中，某些元素可以不正确的彼此嵌套在一起，就像这样：

```
<b><i>this text is bold and italic</b></i>
```

在 XHTML 中，所有元素必须正确的彼此嵌套：

```
<b><i>this text is bold and italic</i></b>
```

---

### XHTML 元素必须始终关闭

这是错误的：

```
<p>this is a paragraph.
<p>this is another paragraph.
```

这是正确的：

```
<p>this is a paragraph.</p>
<p>this is another paragraph.</p>
```

---

### 空元素也必须关闭

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

