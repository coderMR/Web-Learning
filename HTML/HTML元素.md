# HTML 元素

---

### HTML 文档是由 HTML 元素定义的。

---

### HTML 元素

HTML 元素指的是从开始标签（start tag）到结束标签（end tag）的所有代码。

| 开始标签               | 元素内容            | 结束标签
|------------------------|---------------------|-----------
| &lt;p&gt;              | this is a paragraph | &lt;/p&gt;
| &lt;a href="www.baidu.com"&gt; | 百度        | &lt;/a&gt;
| &lt;br /&gt;           |                     |

注释：开始标签常被称为开放标签（opening tag），结束标签常称为闭合标签（closing tag）。

---

### HTML 元素语法

* HTML 元素以开始标签起始
* HTML 元素以结束标签终止
* 元素的内容是开始标签与结束标签之间的内容
* 某些 HTML 元素具有空内容（empty content）
* 空元素在开始标签中进行关闭（以开始标签的结束而结束）
* 大多数 HTML 元素可拥有属性

---

### 嵌套的 HTML 标签

大多数 HTML 元素可以嵌套（可以包含其他 HTML 元素）。

HTML 文档由嵌套的 HTML 元素构成。

### HTML 文档实例

```
<html>

<body>
<p>this is my first paragraph.</p>
</body>

</html>
```

上面的 HTML 文档 包含三个 HTML 元素。

---

### HTML 实例解释

#### &lt;p&gt; 元素：

```
<p>this is my first paragraph.</p>
```

这个 &lt;p&gt; 元素定义了 HTML 文档中的一个段落。

这个元素拥有一个开始标签 &lt;p&gt;，以及一个结束标签 &lt;/p&gt;

元素内容是：this is my first paragraph。

#### &lt;body&gt; 元素

```
<body>
<p>this is my first paragraph.</p>
</body>
```

&lt;body&gt; 元素定义了 HTML 文档的主体。

这个元素拥有一个开始标签 &lt;body&gt;，以及一个结束标签 &lt;/p&gt;。

元素内容是另一个 HTML 元素（p 元素）。

#### &lt;html&gt; 元素

```
<html>

<body>
<p>this is my first paragraph.</p>
</body>

</html>
```

&lt;html&gt; 元素定义了整个 HTML 文档。

这个元素拥有一个开始标签 &lt;html&gt;，以及一个结束标签 &lt;/html&gt;。

元素内容是另一个 HTML 元素（body 元素）。

---

### 不要忘记结束标签

即使忘记使用结束标签，大多数浏览器也能正确的显示 HTML：

```
<p>this is a paragraph.
<p>this is a paragraph.
```

上面的例子在大多数浏览器都没有问题，但不要依赖这种做法。忘记使用结束标签会产生不可预料的结果或错误。

注释：在未来的 HTML 版本不允许省略结束标签。

