# HTML 视频

---

### 在 HTML 中播放视频的方法有很多种。

---

### 问题，以及解决方法

在 HTML 中播放视频并不容易。

您需要谙熟大量技巧，以确保您的视频文件在所有浏览器中（Internet Explorer, Chrome, Firefox, Safari, Opera）和所有硬件上（PC, Mac , iPad, iPhone）都能够播放。

在本节，总结了问题和解决方法。

---

### 使用 &lt;embed&gt; 标签

&lt;embed&gt; 标签的作用是在 HTML 页面中嵌入多媒体元素。

下面的 HTML 代码显示嵌入网页的 Flash 视频：


```
<embed src="movie.swf" height="200" width="200" />
```

### 问题：

* HTML4 无法识别 &lt;embed&gt; 标签。您的页面无法通过验证。
* 如果浏览器不支持 Flash，name视频将无法播放。
* iPad 和 iPhone 不能显示 Flash 视频。
* 如果您将视频转换为其他格式，那么它仍然不能在所有浏览器中播放。

---

### 使用 &lt;object&gt; 标签

&lt;object&gt; 标签的作用是在 HTML 页面中嵌入多媒体元素。

```
<object data="movie.swf" height="200" width="200"/>
```

* 如果浏览器不支持 Flash，name视频将无法播放。
* iPad 和 iPhone 不能显示 Flash 视频。
* 如果您将视频转换为其他格式，那么它仍然不能在所有浏览器中播放。

---

### 使用 &lt;video&gt; 标签

&lt;video&gt; 是 HTML 5 中的新标签。

&lt;video&gt; 标签的作用是在 HTML 页面中嵌入视频元素。

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title></title>
</head>
<body>
    <video width="320" height="240" controls="controls">
        <source src="movie.mp4" type="video/mp4" />
        <source src="movie.ogg" type="video/ogg" />
        <source src="movie.webm" type="video/webm" />
        Your browser does not support the video tag.
    </video>
</body>
</html>
```

### 问题：

* 您必须把视频转换为很多不同的格式。
* &lt;video&gt; 元素在老式浏览器中无效。
* &lt;video&gt; 元素无法通过 HTML 4 和 XHTML 验证。

---

### 最好的 HTML 解决方法

HTML5 + &lt;object&gt; + &lt;embed&gt;

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title></title>
</head>
<body>
    <video width="320" height="240" controls="controls">
        <source src="movie.mp4" type="video/mp4" />
        <source src="movie.ogg" type="video/ogg" />
        <source src="movie.webm" type="video/webm" />
        <object data="movie.mp4" width="320" height="240">
            <embed src="movie.swf" width="320" height="240" />
        </object>
    </video>
</body>
</html>
```

上例中使用了 4 种不同的视频格式。HTML5 &lt;video&gt; 元素会尝试播放以 mp4、ogg 或 webm 格式中的一种来播放视频。如果均失败，则回退到 &lt;embed&gt; 元素。

### 问题：

* 您必须把视频转换为很多不同的格式。
* &lt;video&gt; 元素无法通过 HTML 4 和 XHTML 验证。
* &lt;embed&gt; 元素无法通过 HTML 4 和 XHTML 验证。

---

### 优酷解决方案

在 HTML 中显示视频的最简单的方法是使用优酷等视频网站。
如果您希望在网页中播放视频，那么您可以把视频上传到优酷等视频网站，然后在您的网页中插入 HTML 代码即可播放视频：

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title></title>
</head>
<body>
    <embed src="http://player.youku.com/player.php/sid/XMzI2NTc4NTMy/v.swf" width="480" height="400" type="application/x-shockwave-flash">
    </embed>
</body>
</html>
```

---

### 使用超链接

如果网页包含指向媒体文件的超链接，大多数浏览器会使用“辅助应用程序”来播放文件。
以下代码片段显示指向 AVI 文件的链接。如果用户点击该链接，浏览器会启动“辅助应用程序”，比如 Windows Media Player 来播放这个 AVI 文件：

```
<a href="movie.swf">Play a video file</a>
```

---

### 关于内联视频的一段注释

当视频被包含在网页中时，它被称为内联视频。

如果您打算在 web 应用程序中使用内联视频，您需要意识到很多人都觉得内联视频令人恼火。

同时请注意，用户可能已经关闭了浏览器中的内联视频选项。

我们最好的建议是只在用户希望看到内联视频的地方包含它们。一个正面的例子是，在用户需要看到视频并点击某个链接时，会打开页面然后播放视频。

---


### HTML 4.01 多媒体标签

| 标签 | 描述
|------|-----
| &lt;apple&gt; | 不赞成。定义内嵌 applet
| &lt;embed&gt; | HTML4 中不赞成，HTML5 中赞成。定义内嵌对象。
| &lt;object&lt; | 定义内嵌对象
| &lt;param&gt; | 定义对象的参数

### HTML 5 多媒体标签

| 标签 | 描述
|------|-----
| &lt;audio&gt; | 标签定义声音，比如音乐或其他音频流。
| &lt;embed&gt; | 标签定义嵌入的内容，比如插件。

