# XHTML 结构化之二：案例分析：W3school 的结构化标记

---

无论如何，不要跳过本节。阅读本章将增进你的技能，为你的网页减肥，并且使你对标记与设计之间的差异有更清晰的认识。本章中的理念是易于学习的，但是却能极大的提高网站的性能，以及设计、制作和更新网站的便利性。

在本节，你将学到如何撰写合乎逻辑的、紧凑的标记，使得你有能力将带宽流量降低50%左右，在减少服务器负担和压力的同时，减少网站的加载时间。通过去除那些表现元素，并改掉那些没有任何好处的坏习惯，我们就可以达到上述的目的。

这些坏习惯折磨着网络中的许多站点，特别是那些将 CSS 代码与主要基于表格的布局混合在一起的站点。这种做法笨拙且不经济，即使是对于那些在其他领域很有经验的设计师来说。同时，出现这个问题的几率是均等的，不论是那些手写代码的站点，还是利用可见编辑工具，比如 Dreamweaver 和 GoLive，来创建的站点。

本节会提出这些常见的错误，这样你就可以识别和防范它们，并且学会如何改正错误。我们详细阐述唯一标识符属性 (id) - ，并展示它如何使你可以编写极其紧凑的 XHTML 代码，不论你创建的是混合布局还是纯粹的 CSS 布局。

---

### 每个元素都必须结构化吗？

正如上一节中我们讲到的那样，每个元素都可以被结构化，CSS 可使得一个有序或无序的列表显示为彻头彻尾的导航栏，其中还拥有反转按钮效果。文档的内容可以通过普通的元素进行标记，这些元素通过特定的结构化属性标志来指示出它们在网站设计中所扮演的语义角色。

我们在公元 2006 年创建了 W3School 的第一个中文测试版，我们在一开始就使用了 CSS 进行布局，并使用 XHTML 来结构化文档。每一个其中的元素都是结构化的，从标题到列表，乃至段落。你可以在 w3school 的每个页面看到具有反转效果的首页按钮和二级菜单按钮。下面是这两个组件的 XHTML 代码：

```
<div id="header"><h1><a href="/">w3school在线教程</a></h1></div>
<div id="navfirst">
<ul id="menu">
<li id="h"><a href="/h.asp" title="html教程">html教程</a></li>
<li id="x"><a href="/x.asp" title="XML教程">XML教程</a></li>
<li id="b"><a href="/b.asp" title="浏览器脚本">浏览器脚本</a></li>
<li id="s"><a href="/s.asp" title="服务器脚本">服务器脚本</a></li>
<li id="d"><a href="/d.asp" title="dot net教程">dot net教程</a></li>
<li id="m"><a href="/m.asp" title="多媒体教程">多媒体教程</a></li>
<li id="w"><a href="/w.asp" title="建站手册">建站手册</a></li>
</ul>
</div>
```

---

### div、id 和其他帮手


如果被正确地使用，div 可以成为结构化标记的好帮手，而 id 则是一种令人惊讶的小工具，它使你有能力编写极其紧凑的 XHTML，以及巧妙地利用 CSS，并通过标准文档对象模型 (DOM) 向站点添加复杂精巧的行为。

W3C 在其最新的 XHTML2 草案的 XHTML 结构模型中这样定义 div：

div 元素，通过与 id、class 及 role 属性配合，提供向文档添加额外结构的通用机制。这个元素不会将表现的风格定义于内容。所以，创作者可以通过将这个元素与样式表、xml:lang、属性等配合使用，使 XHTML 适应他们自身的需求和口味。

div 是 division 的简写。division 意为分割、区域、分组。比方说，当你将一系列的链接组合在一起，就形成了文档的一个 division。

### 确定结构的通用机制

所有编写 HTML 的人对段落和标题这类常见的元素都很熟悉，但是有些人对 div 就可能不那么熟悉了。在W3C的描述中我们可以找到理解 div 元素的关键，“一种添加结构的通用机制。”

在本站的首页，我们将教程目录列表封装于一个 div 之中，这是因为教程目录并不是正文的任何元素的一部分。其中，h2元素标记每个教程的标题，同时 ul 列表元素标记每个教程的详细列表。但是在更大更具体的意义中，这个教程目录扮演了一个结构化的角色，即二级导航组件。为了强调这个角色，我们使用 navsecond 这个 id 标注这个 div。

```
<div id="navsecond">

<h2>HTML教程</h2>
<ul>
<li><a href="/html/index.asp" title="HTML教程">HTML</a></li>
<li><a href="/xhtml/index.asp" title="XHTML教程">XHTML</a></li>
<li><a href="/css/index.asp" title="CSS教程">CSS</a></li>
<li><a href="/tcpip/index.asp" title="TCP/IP教程">TCP/IP</a></li>
</ul>

<h2>XML教程</h2>
<ul>
<li><a href="/xml/index.asp" title="XML教程">XML</a></li>
<li><a href="/xsl/xsl_languages.asp" title="XSL语言">XSL</a></li>
... ...
... ...

</div>
```

你可以使用任何命名。"Gladys" 和 "orangebox"都完全符合 XHTML 的命名规则。但是语义的 (semantic) 或者元结构化 (meta-structural) 的命名是最好的（即能够解释其中元素所执行功能的命名）。

当客户决定使用蓝色时，你会觉得将站点某部分命名为 orangebox（橙色框）会非常地傻。下面的这种情况中，你会觉得自己更傻，当距离最后交付只有六个月时，你开始调校样式表，却怎么也想不起来 "Gladys"（格拉迪斯，女子名）到底代表导航区、侧栏还是搜索框。

因此，将 id 标注为 "menu"、"content" 或者 "searchform"会帮助你回忆。进一步讲，标记不等同于设计，结构良好的的页面可以被格式化为你希望的任何样子。这样做的结果是，无论你使用纯粹 CSS 布局或者混合布局，你都会彻底改掉使用表现标记进行思考和创作的习惯。

### id Vs. class

id 属性对于 XHTML 并不新鲜；class 属性或者 div 元素也一样。它们都可以回溯到 HTML 时代。id 属性为一个元素分配一个唯一的名字。每个名字只能在被赋予的页面使用一次。（例如，假如你的页面包含 id 为 content 的 div，那么另外一个 div 或者其他别的元素都不能使用这个名字。相反地，class 属性可以被一遍又一遍地使用在页面中（例如，页面中的五个段落都可以使用名为 "small" 或者"footnote" 的 class 名称）。下面的标记将有助于阐明 id 和 class 的差异：

```
<div id="searchform">Search form components go here. This
section of the page is unique.</div>
<div class="blogentry">
   <h2>Today's blog post</h2>
   <p>Blog content goes here.</p>
   <p>Here is another paragraph of blog content.</p>
   <p>Just as there can be many paragraphs on a page, so too
   there may be many entries in a blog. A blog page could use
   multiple instances of the class "blogentry" (or any other
   class).</p>
</div>

<div class="blogentry">
   <h2>Yesterday's blog post</h2>
   <p>In fact, here we are inside another div of class
   "blogentry."</p>
   <p>They reproduce like rabbits.</p>
   <p>If there are ten blog posts on this page, there might
   be ten divs of class "blogentry" as well.</p>
</div>
```


在这个例子中，名为 searchform 的 div 被用来封装包含搜索表单的页面区域，而 div class="blogentry" 则用来封装 blog 中的每个文章入口。在页面中只有一个搜索表单，所以我们选择 id 标注这个唯一的组件。但是 blog 则拥有许多的（文章）入口，所以 class 属性被应用于这种情况。同样地，新闻站点通常拥有多个 div，这些 div 的 class 可以命名为 "newsitem" 或者别的什么。

然而不是所有的站点都需要 div。blog 站点可以仅仅使用 h1, H2, 和 h2 标题和 &lt;p&gt; 段落，新闻站点也一样。我们在这里展示 class 为 blogentry 的 div，并不是鼓励你在站点中塞满 div，而仅仅是为了向你展示这个原则：在同一个 HTML 文档中，使用多次 class，但只能使用一次 id。

### 粘性贴纸理论

把 id 属性比作粘性贴纸来进行思考应该是有帮助的。我会在冰箱上拍一张贴纸来提醒自己去买牛奶，电话上面也会贴一张，提醒我给一位逾期缴纳的客户打电话。还有一个，被贴在账本夹上面，来提醒我这个月 15 号之前必须缴纳的账单。

id同样会标注文档中的特殊区域，以便提醒你哪个区域需要特殊的处理，在这点上，id属性与粘性贴纸是相似的。为了实现所谓的特殊处理，你需要使用这个特殊的id在样式表中编写若干规则，或者在JavaScript文件中添加几行代码。比方说，你的CSS文件中有一些特定的规则，这些规则只应用于id名为searchform的div内的元素。

当某一 id 属性作为一个有磁性的东西（磁铁）被用于一系列特定的 CSS 规则时，它被称为CSS选择器。有许多创建选择器的方法，不过 id 是很容易使用的，并且有多的用途。

### id 的力量

id 属性不可思议地强有力。它具有以下的能力：

* 作为样式表选择器，使我们有能力创作紧凑的最小化的 XHTML。
* 作为超文本的目标锚，取代过时的 name 属性。
* 作为从基于 DOM 的脚本来定位特定元素的方法。
* 作为对象元素的名称。
* 作为一种综合用途处理 (general purpose processing) 的工具（在 W3C 的例子中，“当把数据从HTML页面中提取到数据库，或将 HTML 文档转换为其他格式等情况下，作为域识别工具来使用。”）

### id 的规则

id 值必须以字母或者下划线开始；不能以数字开始。虽然 W3C 验证不会捕获这个错误，但是 XML 解析器会的。同时，如果你将 id 与 JavaScript 在表单中配合使用，那么 id 名称和值必须是合法的 JavaScript 变量。空格和连字号，特别是连字号，是不被允许的。不仅如此，将下划线用于 class 或者 id 名都不是个好主意，这是由于在 CSS2.0（以及某些浏览器）中的限制。

---

### 语义标记和可用性

现在，我们已经讨论过了用途广泛的 XHTML 元素（特别是 div 和 id），让我们在看看关于本站首页的例子。首先让我们回顾一下这个位于报头位置的菜单：

```
<div id="navfirst">
<ul id="menu">
<li id="h"><a href="/h.asp" title="html教程">html教程</a></li>
<li id="x"><a href="/x.asp" title="XML教程">XML教程</a></li>
<li id="b"><a href="/b.asp" title="浏览器脚本">浏览器脚本</a></li>
<li id="s"><a href="/s.asp" title="服务器脚本">服务器脚本</a></li>
<li id="d"><a href="/d.asp" title="dot net教程">dot net教程</a></li>
<li id="m"><a href="/m.asp" title="多媒体教程">多媒体教程</a></li>
<li id="w"><a href="/w.asp" title="建站手册">建站手册</a></li>
</ul>
</div>
```

我们拥有七个链接，每个链接被分配一个id来对应相应的内容：例如名为 h 的 id 对应 HTML 教程，以此类推。同时这些链接被封装于名为 menu 的列表元素内，名为 menu 的 id 标明了这个列表的职能 - 一个菜单列表，而更外围的名为 navfirst 的 div 则用来标注页面中的这个节 (section)，将之与诸如主要内容 (maincontent)、侧栏 (sidebar) 和页脚 (footer) 之类的元素区别开来。

div 和 ul 两个元素提供了真实的结构，即标明了其中内容的职能（导航栏）和它在文档中所属的位置（页面的报头位置）。相反地，传统的表格布局无法提供有关数据的任何语义信息，同时会轻松地吃掉三倍的带宽。

请注意这些标记没有包含img标签，所以不会牵扯到 width、height、background 或者 border 等等属性。同时它没有使用表格单元格，也不会涉及相关的一系列属性。它非常地干净小巧，同时提供了所有可供理解它的信息。

通过与 CSS 配合使用，这些标记向网站访问者提供了可靠的可快速加载的布局。同时也提供了为访问者创造更灵活多样的外观的可能性。并且在无 CSS 的环境中，我们的结构良好的标记依然可以毫不混乱地提供所有的内容。

目光敏锐的读者也许已经发现，a 元素中包含的文本并没有被浏览器显示出来，这也要归功于结构化标记与 CSS 的完美配合，使我们可以通过几行 CSS 规则来定义一个触发机制，当用户使用图形浏览器时，他们会看到漂亮的导航按钮，而当用户使用纯文本的阅读器时，他们也可以得到全部的文本，这样，对所有的用户来说，内容都是一样的。

并且，由于标记没有包含图像和表格单元，这个导航栏组件可以在不改变结构的情况下被站点内的任何页面所引用，同时赋予它不同的视觉效果。简而言之，通过对代码进行模块化，我们提高了代码的复用性。

---
