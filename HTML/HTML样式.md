# HTML 样式

---

style 属性用来改变 HTML 元素的样式。

---

### HTML 的 style 属性

style 属性提供了一种改变所有 HTML 元素的样式的通用方法。

样式是 HTML 4引入的，它是一种新的首选的改变 HTML 元素样式的方式。通过 HTML 样式，能够通过使用 style 属性直接将样式添加到 HTML 元素，或者间接的在独立的样式表中进行定义。

---

### 不赞成使用的标签和属性

在 HTML 4中，有若干的标签和属性是被废弃的。被废弃的（Deprecated）意思是在未来版本的 HTML 和 XML 中将不支持这些标签和属性。

这里传达的意思很明确：请避免使用这些废弃的标签和属性。

应该避免使用以下的这些标签和属性：

| 标签 | 描述
|------|-----
| &lt;center&gt; | 定义居中的内容
| &lt;font&gt; 和 &lt;basefont&gt; | 定义 HTML 字体
| &lt;s&gt; 和 &lt;strike&gt; | 定义删除文本
| &lt;u&gt; | 定义下划线文本

| 属性 | 描述
|------|-----
| align | 定义文本的对齐方式
| bgcolor | 定义背景颜色
| color | 定义文本颜色

对于以上的这些标签和属性：请使用样式代替！

---

### HTML 样式实例 - 背景颜色

background-color 属性为元素定义了背景颜色：

```
<html>

<body style="background-color:yellow">
<h1 style="background-color:red">this is a heading</h1>
<p style="background-color:green">this is a paragraph</p>
</body>

</html>
```

注释：style 属性淘汰了旧的 bgcolor 属性。

---

### HTML 样式实例 - 字体、颜色和尺寸

font-family、color以及font-size 属性分别定义了元素中文本的字体、颜色和字体尺寸：

```
<html>

<body>
<h1 style="font-family:verdana">this is a heading</h1>
<p style="font-family:arial;color:red;font-size:20px">this is a paragraph</p>
</body>

</html>
```

注释：style 属性淘汰了旧的 &lt;font&gt; 标签与 color 属性。

---

### HTML 样式实例 - 文本对齐

text-align 属性规定了元素中文本的水平对齐方式：

```
<html>

<body>
<h1 style="text-align:center">this is a heading</h1>
</body>

</html>
```

注释：style 属性淘汰了旧的 &lt;center&gt; 标签与 align 属性。
