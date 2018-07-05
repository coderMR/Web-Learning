# HTML 音频

---

### 在 HTML 中播放声音的方法有很多种。

---

### 问题，以及解决方法

在 HTML 中播放音频并不容易。

您需要谙熟大量技巧，以确保您的音频文件在所有浏览器中（Internet Explorer，Chrome，Firefox，Safari，Opera）和所有硬件上（PC，Mac，iPad，iPhone）都能够播放。

---

### 使用插件

浏览器插件是一种扩展浏览器标准功能的小型计算机程序。

插件有很多用途：播放音乐、显示地图、验证银行账户、控制输入等等。

可使用 &lt;object&gt; 或 &lt;embed&gt; 标签来将插件添加到 HTML 页面。

这些标签定义资源（通常非 HTML 资源）的容器，根据类型，它们即会由浏览器显示，也会由外部插件显示。

---

### 使用 &lt;embed&gt; 元素

---

&lt;embed&gt; 标签定义外部（非 HTML）内容的容器。这是一个 HTML5 标签，在 HTML4 中是非法的，但所有浏览器中都有效。

下面的代码能够显示嵌入网页中的 MP3 文件：

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title></title>
</head>
<body>
    <embed height="100" width="100" src="song.mp3" />
</body>
</html>
```

### 问题：

* &lt;embed&gt; 标签在 HTML 4 中是无效的。页面无法通过 HTML 4 验证。
* 不同的浏览器对音频格式的支持也不同。
* 如果浏览器不支持该文件格式，没有插件的话就无法播放该音频。
* 如果用户的计算机未安装插件，无法播放音频。
* 如果把文件转换为其他格式，仍然无法在所有浏览器中播放

---

### 使用 &lt;object&gt; 元素

&lt;object tag&gt; 标签也可以定义外部（非 HTML）内容的容器。

下面的代码能够显示嵌入网页中的 MP3 文件：

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title></title>
</head>
<body>
    <object height="100" width="100" data="song.mp3"></object>
</body>
</html>
```

### 问题：

* 不同的浏览器对音频格式支持也不同。
* 如果浏览器不支持该文件格式，没有插件的话就无法播放该音频。
* 如果用户的计算机未安装插件，无法播放音频。
* 如果该文件转换为其他格式，仍然无法再所有浏览器中播放。

---

### 使用 HTML5 &lt;audio&gt; 元素

&lt;audio&gt; 元素是一个 HTML5 元素，在 HTML 4 中是非法的，但在所有浏览器中都有效。

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title></title>
</head>
<body>
    <audio controls="controls">
        <source src="song.mp3" type="audio/mp3" />
        <source src="song.ogg" type="audio/ogg" />
        Your browser does not support this audio format.
    </audio>
</body>
</html>
```

上面的例子使用了一个 mp3 文件，这样它在 Internet Explorer、Chrome、Safari 中是有效的。

为了使这段音频在 Firefox 和 Opera 中同样有效，添加了一个 ogg 类型文件，如果失败，会显示错误消息。

### 问题：

* &lt;audio&gt; 标签在 HTML 4中是无效的。您的页面无法通过HTML 4验证。
* 您必须把音频文件转换为不同的格式。
* &lt;audio&gt; 元素在老式浏览器中不起作用。

---

### 最好的 HTML 解决方法

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title></title>
</head>
<body>
    <audio controls="controls" height="100" width="100">
        <source src="song.mp3" type="audio/mp3" />
        <source src="song.ogg" type="audio/ogg" />
        <embed height="100" width="100" src="song.mp3" />
    </audio>
</body>
</html>
```

上面的例子使用了两个不同的音频格式。HTML5 &lt;audio&gt; 元素会尝试以 mp3 或 ogg 来播放音频。如果失败，代码将回退尝试 &lt;embed&gt; 元素。

### 问题：

* 您必须把音频转换为不同的格式。
* &lt;audio&gt; 元素无法通过 HTML 4 和 XHTML 验证。
* &lt;embed&gt; 元素无法通过 HTML 4 和 XHTML 验证。
* &lt;embed&gt; 元素无法回退来显示错误信息。

---

### 向网站添加音频的最简单方法

向网友添加音频的最简单的方法是什么？

雅虎的媒体播放器绝对算其中之一。

使用雅虎媒体播放器是一个不同的途径。只需简单的让雅虎来完成歌曲播放工作就好了。

它能播放 mp3 以及一系列其他格式。通过一行简单的代码，就可以把它添加到网页中，轻松的将 HTML 页面转变为专业的播放列表。

---

### 雅虎媒体播放器

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title></title>
</head>
<body>
    <a href="10295.wav">Play Sound</a>
    <script type="text/javascript" src="http://mediaplayer.yahoo.com/js">
    </script>
</body>
</html>
```

使用雅虎播放器是免费的，如需使用它，只需把这段 JavaScript 插入网页底部。

```
<script type="text/javascript" src="http://mediaplayer.yahoo.com/js"></script>
```

然后只需简单的把 MP3 文件链接到 HTML 中，JavaScript 会自动的为每首歌创建播放按钮：

```
<a href="song1.mp3">Play Song 1</a>
<a href="song2.mp3">Play Song 2</a>
```

雅虎媒体播放器为您的用户提供的是一个小型的播放按钮，而不是完整的播放器。不过，当您点击该按钮，会弹出完整的播放器。

请注意，这个播放器始终停靠在窗框底部。只需点击它，就可将其滑出。

---

### 使用超链接

如果网页包含指向媒体文件的超链接，大多数浏览器会使用"辅助应用程序"来播放文件。

以下代码片段显示指向 wav 文件的超链接。如果用户点击该链接，浏览器会启动"辅助应用程序"来播放该文件：

```
<a href="song.mp3">Play the sound</a>
```

---

### 内联的声音

当您在网页中包含声音，或者作为网页的组成部分时，它被称为内联声音。

如果您打算在 web 应用程序中使用内联声音，您需要意识到很多人都觉得内联声音很恼火。同时请注意，用户可能已经关闭了浏览器中的内联声音选项。

我们最好的建议是在用户希望听到内联声音的地方包含它们。一个正面的例子是，在用户需要听到录音并点击某个链接时，会打开页面然后播放录音。

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


