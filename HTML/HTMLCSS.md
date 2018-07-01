# HTML CSS

---

### 通过使用 HTML4.0，所有的格式化代码均可迁移出 HTML 文档，然后移入一个独立的样式表。

---

### 如何使用样式表

当浏览器读到一个样式表时，就会按照样式表对文档进行格式化。有以下三种方式来插入样式表：

#### 外部样式表

当样式需要被应用到很多页面时，外部样式表将是最理想的选择。使用外部样式表，就可以通过更改一个文件来改变整个站点的外观。

```
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```

#### 内部样式表

当单个文件需要特别样式时，就可以使用内部样式表。可以在 head 部分通过 &lt;style&gt; 标签定义内部样式表。

```
<head>
<style type="text/css">
body {background-color:red}
p {margin-left:20px}
</style>
</head>
```

#### 内敛样式

当特殊的样式需要应用到个别元素时，就可以使用内联样式。使用内联样式的方法是在相关的标签中使用样式属性。样式属性可以包含任何 CSS 属性。以下实例显示出如何改变段落的颜色和左外边距。

```
<p style="color:red; margin-left:10px">
this is a paragraph
</p>
```

---

| 标签 | 描述
|------|-----
| &lt;style&gt; | 定义样式
| &lt;link&gt; | 定义资源引用
| &lt;div&gt; | 定义文档中的节或区域（块级）
| &lt;span&gt; | 定义文档中的行内小块或区域
| &lt;font&gt; | 定义文本的字体，字体尺寸，字体颜色。不赞成使用，请使用样式代替
| &lt;basefont&gt; | 定义基准字体。不赞成使用，请使用样式代替
| &lt;center&gt; | 对文本进行水平居中。不赞成使用，请使用样式代替

---
