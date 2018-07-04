# HTML5 迁移

---

从 HTML4 迁移至 HTML5

本节讲解如何把一张已有的 HTML4 页面转换为 HTML5 页面，在不破坏原始内容和结构的情况下。

注释：您可以使用相同的技巧从 HTML4 以及 XHTML 迁移至 HTML5。


<table style="text-align:center; font-size:14px; border-collapse:separate; border-spacing:15px;" class="dataintable">
<tr>
<th style="width:50%; text-align:center; background-color:#fff; border:0px;">典型的 HTML4</th>
<th style="width:50%; text-align:center; background-color:#fff; border:0px;">典型的 HTML5</th>
</tr>

<tr>
<td>&lt;div id=&quot;header&quot;&gt;</td>
<td>&lt;header&gt;</td>
</tr>

<tr>
<td>&lt;div id=&quot;menu&quot;&gt;</td>
<td>&lt;nav&gt;</td>
</tr>

<tr>
<td>&lt;div id=&quot;content&quot;&gt;</td>
<td>&lt;section&gt;</td>
</tr>

<tr>
<td>&lt;div id=&quot;post&quot;&gt;</td>
<td>&lt;article&gt;</td>
</tr>

<tr>
<td>&lt;div id=&quot;footer&quot;&gt;</td>
<td>&lt;footer&gt;</td>
</tr>
</table>

---

### 典型的 HTML4 页面

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" 
"http://www.w3.org/TR/html4/loose.dtd">
<html lang="en">
<head>
    <meta http-equiv="Content-Type" content="text/html;charset=utf-8">
    <title>HTML4</title>
    <style>
        body {
            font-family:Verdana,
            sans-serif;
            font-size:0.8em;
        }
        div#header,div#footer,div#content,div#post {
            border:1px solid grey;
            margin:5px;
            margin-bottom:15px;
            padding:8px;
            background-color:white;
        }
        div#header,div#footer {
            color:white;
            background-color:#444;
            margin-bottom:5px;
        }
        div#content {
            background-color:#ddd;
        }
        div#menu ul {
            margin:0;padding:0;
        }
        div#menu ul li {
            display:inline; margin:5px;
        }
    </style>
</head>
<body>
    <div id="header">
        <h1>Monday Times</h1>
    </div>

    <div id="menu">
        <ul>
            <li>News</li>
            <li>Sports</li>
            <li>Weather</li>
        </ul>
    </div>

    <div id="content">
        <h2>News Section</h2>

        <div id="post">
            <h2>News Article</h2>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
        </div>

        <div id="post">
            <h2>News Article</h2>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
        </div>

    </div>

    <div id="footer">
        <p>&copy; 2014 Monday Times. All rights reserved.</p>
    </div>

</body>
</html>
```

### 更改为 HTML5 DOCTYPE

修改文档类型，从 HTML4 DOCTYPE：

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

修改为 HTML5 DOCTYPE：

```
<!DOCTYPE html>
```

### 更改为 HTML5 编码

修改编码信息，从HTML4：

```
<meta http-equiv="Content-Type" content="text/html;charset=utf-8">
```

改为 HTML5：

```
<meta charset="utf-8">
```

---

### 添加 shiv

所有现代浏览器都支持 HTML5 语义元素。

此外，您可以“教授”老式浏览器如何处理“未知元素”。

为 Internet Explorer 支持而添加的 shiv：

```
<!--[if lt IE 9]>
  <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
<![endif]-->
```

### 为 HTML5 语义元素添加 CSS

请看已有的 CSS 样式

```

div#header,div#footer,div#content,div#post {
    border:1px solid grey;
    margin:5px;
    margin-bottom:15px;padding:8px;
    background-color:white;
}
div#header,div#footer {
    color:white;
    background-color:#444;
    margin-bottom:5px;
}
div#content {
    background-color:#ddd;
}
div#menu ul {
    margin:0;
    padding:0;
}
div#menu ul li {
    display:inline; 
    margin:5px;
}

Duplicate with equal CSS styles for HTML5 semantic elements:

header,footer,section,article {
    border:1px solid grey;
    margin:5px;
    margin-bottom:15px;
    padding:8px;
    background-color:white;
}
header,footer {
    color:white;
    background-color:#444;
    margin-bottom:5px;
}
section {
    background-color:#ddd;
}
nav ul  {
    margin:0;padding:0;
}
nav ul li {
    display:inline; margin:5px;
}
```

### 更改为 HTML5 &lt;header&gt; 和 &lt;footer&gt;

把 id="header" 和 id="footer" 的 &lt;div&gt; 元素：

```
<div id="header">
    <h1>Monday Times</h1>
</div>
    ...
<div id="footer">
    <p>&copy; 2014 W3Schools. All rights reserved.</p>
</div>
```

修改为 HTML5 语义元素 &lt;header&gt; 和 &lt;footer&gt; ：

```
<header>
    <h1>Monday Times</h1>
</header>
    ...
<footer>
    <p>© 2014 W3Schools. All rights reserved.</p>
</footer>
```

---

### 更改为 HTML5 &lt;nav&gt;

把 id="menu" 的 &lt;div&gt; 元素：

```
<div id="menu">
    <ul>
        <li>News</li>
        <li>Sports</a></li>
        <li>Weather</li>
    </ul>
</div>
```

修改为 HTML5 语义元素 &lt;nav&gt;：

```
<nav>
    <ul>
        <li>News</li>
        <li>Sports</a></li>
        <li>Weather</li>
    </ul>
</nav>
```

### 更改为 HTML5 &lt;section&gt;

把 id="content" 的 the &lt;div&gt; 元素：

```
<div id="content">
    ...
</div>
```

修改为 HTML5 语义元素 &lt;section&gt;：

```
<section>
    ...
</section>
```

### 更改为 HTML5 &lt;article&gt;

把 class="post" 的所有 &lt;div&gt; 元素：

```
<div class="post">
    <h2>News Article</h2>
    <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
</div>
```

修改为 HTML5 语义元素 &lt;article&gt;：

```
<article>
    <h2>News Article</h2>
    <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
</article>
```

删除不在需要的样式：

```
div#header,div#footer,div#content,div#post {
    border:1px solid grey;
    margin:5px;
    margin-bottom:15px;padding:8px;
    background-color:white;
}
div#header,div#footer {
    color:white;
    background-color:#444;
    margin-bottom:5px;
}
div#content {
    background-color:#ddd;
}
div#menu ul {
    margin:0;
    padding:0;
}
div#menu ul li {
    display:inline; 
    margin:5px;
}
```

---

### 典型的 HTML5 页面

最后您可以删除 &lt;head&gt; 标签。HTML5 中不再需要它们：

```
<!DOCTYPE html>
<html lang="en">
    <title>HTML5</title>
    <meta charset="utf-8">
    <!--[if lt IE 9]>
        <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
    <style>
        body {
            font-family:Verdana,sans-serif;
            font-size:0.8em;
        }
        header,footer,section,article {
            border:1px solid grey;
            margin:5px;
            margin-bottom:15px;
            padding:8px;
            background-color:white;
        }
        header,footer {
            color:white;
            background-color:#444;
            margin-bottom:5px;
        }
        section {
            background-color:#ddd;
        }
        nav ul {
            margin:0;padding:0;
        }
        nav ul li {
            display:inline;
            margin:5px;
        }
    </style>
<body>
    <header>
        <h1>Monday Times</h1>
    </header>
    <nav>
        <ul>
            <li>News</li>
            <li>Sports</li>
            <li>Weather</li>
        </ul>
    </nav>
    <section>
        <h2>News Section</h2>
        <article>
            <h2>News Article</h2>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
        <article>
        <article>
            <h2>News Article</h2>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
            <p>Ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum ipsum lurum hurum turum.</p>
        </article>
    </section>
    <footer>
        <p>&copy; 2014 Monday Times. All rights reserved.</p>
    </footer>
</body>
</html>
```

---

### &lt;article&gt; &lt;section&gt; 与 &lt;div&gt; 之间的差异

在 HTML5 标准中，&lt;article&gt; &lt;section&gt; 与 &lt;div&gt; 之间的差异很小，令人困惑。

在 HTML5 标准中，&lt;section&gt; 元素被定位为相关元素的块。

&lt;article&gt; 元素被定义为相关元素的完整的自包含块。

&lt;div&gt; 元素被定义为子元素的块。

如何理解呢？

在上面的例子中，我们曾使用 &lt;section&gt; 作为相关 &lt;article&gt; 的容器。

但是，我们也能够把 &lt;article&gt; 用作文章的容器。

下面是一些不同的例子：

```
<article> 中的 <article>：

<article>

    <h2>Famous Cities</h2>

    <article>
        <h2>London</h2>
        <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
    </article>

    <article>
        <h2>Paris</h2>
        <p>Paris is the capital and most populous city of France.</p>
    </article>

    <article>
        <h2>Tokyo</h2>
        <p>Tokyo is the capital of Japan, the center of the Greater Tokyo Area, and the most populous metropolitan area in the world.</p>
    </article>

</article>
```

```
<article> 中的 <div>：

<article>

    <h2>Famous Cities</h2>

    <div class="city">
        <h2>London</h2>
        <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
    </div>

    <div class="city">
        <h2>Paris</h2>
        <p>Paris is the capital and most populous city of France.</p>
    </div>

    <div class="city">
        <h2>Tokyo</h2>
        <p>Tokyo is the capital of Japan, the center of the Greater Tokyo Area, and the most populous metropolitan area in the world.</p>
    </div>

</article>
```

```
<article> 中的 <section> 中的 <div>：

<article>

    <section>
        <h2>Famous Cities</h2>

        <div class="city">
            <h2>London</h2>
            <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
        </div>

        <div class="city">
            <h2>Paris</h2>
            <p>Paris is the capital and most populous city of France.</p>
        </div>

        <div class="city">
            <h2>Tokyo</h2>
            <p>Tokyo is the capital of Japan, the center of the Greater Tokyo Area, and the most populous metropolitan area in the world.</p>
        </div>
    </section>

    <section>
        <h2>Famous Countries</h2>

        <div class="country">
            <h2>England</h2>
            <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
        </div>

        <div class="country">
            <h2>France</h2>
            <p>Paris is the capital and most populous city of France.</p>
        </div>

        <div class="country">
            <h2>Japan</h2>
            <p>Tokyo is the capital of Japan, the center of the Greater Tokyo Area, and the most populous metropolitan area in the world.</p>
        </div>
    </section>

</article>
```

---
