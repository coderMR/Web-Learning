# HTML5 语义元素

---

### 什么是语义元素？

语义元素清楚地向浏览器和开发者描述其意义。

非语义元素的例子：&lt;div&gt; 和 &lt;span&gt; - 无法提供关于其内容的信息。

语义元素的例子：&lt;form&gt;、&lt;table&gt; 以及 &lt;img&gt; - 清晰地定义其内容。

---

### HTML5 中新的语义元素

许多网站包含了指示导航、页眉以及页脚的 HTML 代码，例如这些：&lt;div id="nav"&gt; &lt;div class="header"&gt; &lt;div id="footer"&gt;。

HTML5 提供了定义页面不同部分的新语义元素：

* &lt;article&gt;
* &lt;aside&gt;
* &lt;details&gt;
* &lt;figcaption&gt;
* &lt;footer&gt;
* &lt;header&gt;
* &lt;main&gt;
* &lt;mark&gt;
* &lt;nav&gt;
* &lt;section&gt;
* &lt;summary&gt;
* &lt;time&gt;

---

### HTML5 &lt;section&gt; 元素

&lt;section&gt; 元素定义文档中的节。

根据 W3C 的 HTML 文献："节（section）是由主题的内容组，通常具有标题"。

可以将网站首页划分为简介、内容、联系信息等节。

```
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
    <section>
       <h1>WWF</h1>
       <p>The World Wide Fund for Nature (WWF) is....</p>
    </section> 
</body>
</html>
```

--- 

### HTML5 &lt;article&gt; 元素

&lt;article&gt; 元素规定独立的自包含内容。

文档有其自身的意义，并且可以独立于网站其他内容进行阅读。

&lt;article&gt; 元素的应用场景：

* 论坛
* 博客
* 新闻

```
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
    <article>
        <h1>What Does WWF Do?</h1>
        <p>WWF's mission is to stop the degradation of our planet's natural environment, and build a future in which humans live in harmony with nature.</p>
    </article> 
</body>
</html>
```

### 嵌套语义元素

在 HTML5 标准中， &lt;article&gt; 元素定义完整的相关元素自包含块。

&lt;section&gt; 元素被定义为相关元素块。

我们能够使用该定义来决定如何嵌套元素吗？不，我们不能！

在网上，您会发现 &lt;section&gt; 元素包含 &lt;article&gt; 元素的 HTML 页面，还有 &lt;article&gt; 元素包含 &lt;section&gt; 元素的页面。您还会发现 &lt;section&gt; 元素包含 &lt;section&gt; 元素，同时 &lt;article&gt; 元素包含 &lt;article&gt; 元素。

---

### HTML5 &lt;header&gt; 元素

&lt;header&gt; 元素为文档或节规定页眉。

&lt;header&gt; 元素应该被用作介绍性内容的容器。

一个文档中可以有多个 &lt;header&gt; 元素。

下例为一篇文章定义了页眉：

```
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
    <article>
        <header>
            <h1>What Does WWF Do?</h1>
            <p>WWF's mission:</p>
        </header>
        <p>WWF's mission is to stop the degradation of our planet's natural environment, and build a future in which humans live in harmony with nature.</p>
    </article> 
</body>
</html>
```

---

### HTML5 &lt;footer&gt; 元素

&lt;footer&gt; 元素为文档或节规定页脚。

&lt;footer&gt; 元素应该提供有关其包含元素的信息。

页脚通常包含文档的作者、版权信息、使用条款链接、联系信息等等。

您可以在一个文档中使用多个 &lt;footer&gt; 元素。

```
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
    <footer>
        <p>Posted by: Hege Refsnes</p>
        <p>Contact information: <a href="mailto:someone@example.com">
        someone@example.com</a>.</p>
    </footer> 
</body>
</html>
```

### HTML5 &lt;nav&gt; 元素

&lt;nav&gt; 元素定义导航链接集合。

&lt;nav&gt; 元素旨在定义大型的导航链接块。不过，并非文档中所有链接都应该位于 &lt;nav&gt; 元素中！

```
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
    <nav>
        <a href="/html/">HTML</a> |
        <a href="/css/">CSS</a> |
        <a href="/js/">JavaScript</a> |
        <a href="/jquery/">jQuery</a>
    </nav> 
</body>
</html>
```

### HTML5 &lt;aside&gt; 元素

&lt;aside&gt; 元素页面主内容之外的某些内容，比如侧栏。

aside 内容应该与周围内容相关。

```
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
    <p>My family and I visited The Epcot center this summer.</p>

    <aside>
        <h4>Epcot Center</h4>
        <p>The Epcot Center is a theme park in Disney World, Florida.</p>
    </aside> 
</body>
</html>
```

---

### HTML5 &lt;figure&gt; 和 &lt;figcaption&gt; 元素

在书籍和报纸中，与图片搭配的标题很常见。

标题（caption）的作用是为图片添加可见的解释。

通过 HTML5，图片和标题能够组合在 &lt;figure&gt; 元素中。

```
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
    <figure>
       <img src="https://www.baidu.com/img/bd_logo1.png" alt="The Pulpit Rock" width="304" height="228">
       <figcaption>Fig1. - The Pulpit Pock, Norway.</figcaption>
    </figure> 
</body>
</html>
```

注释：&lt;img&gt; 元素定义图片，&lt;figure&gt; 元素定义标题。

---

### 为何使用 HTML5 元素 ？

如果使用 HTML4 的话，开发者会使用他们喜爱的属性名来设置页面元素的样式：header、top、bottom、footer、menu、navigation、main、container、content、article、sidebar、topnav...

如此，浏览器便无法识别正确的网页内容。

而通过 HTML5 元素，比如：&lt;header&gt; &lt;footer&gt; &lt;nav&gt; &lt;section&gt; &lt;article&gt; 此问题就迎刃而解。

根据 W3C，语义网：允许跨应用程序、企业和团体对数据进行分享和重用。

---

### HTML5 中的语义元素


| 标签 | 描述
|------|-----
| &lt;article&gt; | 定义文档内的文章
| &lt;aside&gt; | 定义页面内容之外的内容
| &lt;details&gt; | 定义用户可查看或隐藏的额外细节
| &lt;figcaption&gt; | 定义 &lt;figure&gt; 元素的标题
| &lt;figure&gt; | 定义自包含内容，比如图示、图标、照片、代码清单等等
| &lt;footer&gt; | 定义文档或节的页脚
| &lt;header&gt; | 定义文档或节的页眉
| &lt;main&gt; | 定义文档的主内容
| &lt;mark&gt; | 定义重要或强调的内容
| &lt;nav&gt; | 定义文档内的导航链接
| &lt;section&gt; | 定义文档中的节
| &lt;summary&gt; | 定义 &lt;details&gt; 元素的可见标题
| &lt;time&gt; | 定义日期/时间

---
