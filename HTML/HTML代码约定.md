# HTML5 样式指南和代码约定

---

### HTML 代码约定

web 开发者常常不确定在 HTML 中使用的代码样式和语法。

在 2000 年至 2010 年之间，许多 web 开发者从 HTML 转换为 XHTML。

通过 XHTML，开发者不得不编写有效的"格式良好的"代码。

HTML5 在代码验证时会更宽松一点。

通过 HTML5，您必须创建属于自己的最佳实践、样式指南和代码约定。

---

### 智能且有未来保证

对样式的合乎逻辑的使用，可以令其他人更容易理解和使用您的 HTML。

在未来，诸如 XML 阅读器之类的程序，也许需要阅读您的 HTML。

使用格式良好的"近似 XHTML"的语法，能够更只能。

注释：请示中保持您的样式智能、整洁、纯净、格式良好。

---

### 请使用正确的文档类型

请始终在文档的首行声明文档类型：

```
<!DOCTYPE html>
```

如果您一贯坚持小写标签，那么可以使用：

```
<!doctype html>
```

---

### 请使用小写元素名

HTML5 允许在元素名中使用混合大小写字母。

我们推荐使用小写元素名：

* 混合大小写名称并不友好
* 开发者习惯使用小写名（比如在 XHTML 中）
* 小写看起来更纯净
* 小写更易书写

---

### 关闭所有 HTML 元素

在 HTML5 中，您不必关闭所有元素（例如 &lt;p&gt; 元素）。

我们建议关闭所有 HTML 元素。

---

### 关闭空的 HTML 元素

在 HTML5 中，关闭空元素是可选的。

允许这样：

```
<meta charset="utf-8">
```

也允许这样：

```
<meta charset="utf-8" />
```

斜杠（/）在 XHTML 和 XML 中是必需的。

如果您期望 XML 软件访问您的页面，请保持这个习惯。

---

### 使用小写属性名

HTML5 允许大小写混合的属性名。

我们建议使用小写属性名：

* 混合属性名并不友好
* 开发者习惯于使用小写属性名（比如在 XHTML 中）
* 小写属性名看起来更纯净
* 小写属性名更易书写

---

### 属性值加引号

HTML5 允许不加引号的属性值。

我们推荐属性值加引号：

* 如果属性值包含值，则必须使用引号。
* 混合样式绝对不好
* 加引号的值更易阅读

这个属性值无效，因为值中包含空格：

```
<table class=table striped>
```

这样是有效的：

```
<table class="table striped">
```

---

### 必需的属性

请始终对图像使用 alt 属性。当图像无法显示时该属性很重要。

```
<img src="html5.gif" alt="HTML5" style="width:128px;height:128px" />
```

请始终定义图像尺寸。这样会减少闪烁，因为浏览器会在图像加载之前为图像预留空间。

```
<img src="html5.gif" alt="HTML5" style="width:128px;height:128px" />
```

---

### 空格和等号

等号两边的空格是合法的：

```
<link rel = "stylesheet" href = "style.css">
```

但是精简空格更易阅读：

```
<link rel="stylesheet" href="style.css">
```

---

### 避免长代码行

当使用 HTML 编辑器时，通过左右滚动来阅读 HTML 代码很不方便。

请尽量避免代码行超过 80 个字符。

---

### 空行和缩进

请勿毫无理由的增加空行。

为了提高可读性，请增加空行来分隔大型或逻辑代码块。

为提高可读性，请增加两个空格的缩进，请勿使用 TAB（这条很傻比，我是 TAB 党）。

请勿使用没有必要的空行和缩进。

---

### 我们不推荐省略 &lt;html&gt; 和 &lt;body&gt; 标签。

&lt;html&gt; 元素是文本的根元素，它是规定页面语义的理想位置。

```
<!DOCTYPE html>
<html lang="en-US">
```

对于可访问引用程序和搜索引擎，声明语言很重要。

省略 &lt;html&gt; 或 &lt;body&gt; 可令 DOM 和 XML 软件崩溃。

省略 &lt;body&gt; 会在老式浏览器（IE9）中产生错误。

---

### 省略 &lt;head&gt; ？

在 HTML5 标准中，&lt;head&gt; 标签也能被省略。

默认的，浏览器会把 &lt;body&gt; 之前的所有元素添加到默认的 &lt;head&gt; 元素。

通过省略 &lt;head&gt;，您能够降低 HTML 的复杂性（这能降低多少？这条也很傻逼）。

---

### 元数据

&lt;title&gt; 元素在 HTML5 中是必须的。请尽可能制作有意义的标题。

为了确保恰当的解释，以及正确的搜索引擎索引，在文档中对语言和字符编码定义越早越好。

```
<!DOCTYPE html>
<html lang="en-US">
<head>
    <meta charset="UTF-8">
    <title>HTML5 Syntax and Coding Style</title>
</head>
```

---

### HTML 注释：

短注释应该在单行中书写，并在 <!-- 之后增加一个空格，在 <!-- 之前增加一个空格：

```
<!-- This is a comment -->
```

长注释，跨越多行，应该通过 <!-- 和 --> 在独立的行中书写：

```
<!-- 
  This is a long comment example. This is a long comment example. This is a long comment example.
  This is a long comment example. This is a long comment example. This is a long comment example.
-->
```

---

### 样式表

请使用简单的语法来链接样式表（type 属性不是必需的）：

```
<link rel="stylesheet" href="style.css" />
```

段规则可以压缩为一行，就像这样：

```
p.into {font-family:"Verdana"; fot-size:16em;}
```

长规则应该分为多行：

```
body {
    background-color: lightgrey;
    font-family: "Arial Black", Helvetica, sans-serif;
    font-size: 16em;
    color: black;
}
```

* 开括号与选择器位于同一行
* 在开括号之前用一个空格
* 使用两个字符的缩进（我习惯使用4个）
* 在每个逗号或分号之后使用空格
* 在每个属性值对（包括最后一个）之后使用分好
* 只在值包含空格时使用引号来包围值
* 把闭括号放在新的一行，之前不适用空格
* 避免每行超过 80 个字符

---

### 在 HTML 中加载 JavaScript

请使用简单的语法来加载外部脚本（type 属性不是必需的）：

```
<script src="myscript.js"></script>
```

---

### 通过 JavaScript 访问 HTML 元素

使用 "不整洁" 的 HTML 样式的后果，是可能会导致 JavaScript 错误。

这两个 JavaScript 语句会产生不同的结果：

```
var obj = getElementById("Demo")
var obj = getElementById("demo")
```

如果可能，请在 HTML 中使用（与 JavaScript）相同的命名约定。

---

### 使用小写文件名

大多数 web 服务器（Apache、Nginx）对文件名的大小写敏感（因为 操作系统 与 服务端编程语言 对文件名的大小写敏感）：

不能以 london.jpg 访问 London.jpg。

其他 web 服务器（微软，IIS）对大小写不敏感（微软就是个奇葩，什么都要跟别人不一样点，而且不如别人）：

能够以 london.jpg 或 London.jpg 访问 London.jpg。

如果使用混合大小写，name您必须保持高度的一致性。

如果您从对大小写不敏感的服务器转到一台对大小写敏感的服务器上，这些小错误将破坏您的网站。

为了避免这些问题，请始终使用小写文件名（如果可以的话）。

---

### 文件扩展名

HTML 文件名应该使用扩展名 .html（而不是 .htm）。

CSS 文件应该使用扩展名 .css。

JavaScript 文件应该使用扩展名 .js。
