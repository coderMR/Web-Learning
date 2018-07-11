# HTML 5 音频

---

### HTML5 提供了播放音频的标准。

---

### Web 上的音频

直到现在，仍然不存在一项旨在网页上播放音频的标准。

今天，大多数音频是通过插件（比如 Flash）来播放的。然而，并非所有浏览器都拥有同样的插件。

HTML5 规定了一种通过 audio 元素来包含音频的标准方法。

audio 元素能够播放声音文件或者音频流。

---

### 音频格式

当前，audio 元素支持三种音频格式：

<table class="dataintable">
<tr>
<th>&nbsp;</th>
<th style="width:16%;">IE 9</th>
<th style="width:16%;">Firefox 3.5</th>
<th style="width:16%;">Opera 10.5</th>
<th style="width:16%;">Chrome 3.0</th>
<th style="width:16%;">Safari 3.0</th>
</tr>

<tr>
<td>Ogg Vorbis</td>
<td>&nbsp;</td>
<td>&#8730;</td>
<td>&#8730;</td>
<td>&#8730;</td>
<td>&nbsp;</td>
</tr>

<tr>
<td>MP3</td>
<td>&#8730;</td>
<td>&nbsp;</td>
<td>&nbsp;</td>
<td>&#8730;</td>
<td>&#8730;</td>
</tr>

<tr>
<td>Wav</td>
<td>&nbsp;</td>
<td>&#8730;</td>
<td>&#8730;</td>
<td>&nbsp;</td>
<td>&#8730;</td>
</tr>
</table>

---

### 如何工作

如需在 HTML5 中播放音频，您需要：

```
<audio src="http://www.w3school.com.cn/i/movie.ogg" controls="controls">
</audio>
```

control 属性供添加播放、暂停和音量控件。

&lt;audio&gt; 与 &lt;/audio&gt; 之间插入的内容是供不支持 audio 元素的浏览器显示的。

```
<!DOCTYPE HTML>
<html>
<body>

<audio src="http://www.w3school.com.cn/i/song.ogg" controls="controls">
Your browser does not support the audio element.
</audio>

</body>
</html>
```

上面的例子使用一个 Ogg 文件，适用于Firefox、Opera 以及 Chrome 浏览器。

要确保适用于 Safari 浏览器，音频文件必须是 MP3 或 Wav 类型。

audio 元素允许多个 source 元素。source 元素可以链接不同的音频文件。浏览器将使用第一个可识别的格式：

```
<!DOCTYPE html>
<html>
<head>
    <title>
        audio
    </title>
    <meta charset="utf-8">
</head>
<body>
    <audio controls="controls">
        <source src="http://www.w3school.com.cn/i/song.ogg" type="audio/ogg">
        <source src="http://www.w3school.com.cn/i/song.mp3" type="audio/mpeg">
        Your browser does not support the audio tag.
    </audio>
</body>
</html>
```

---

### Internet Explorer

Internet Explorer 8 不支持 audio 元素。在 IE 9 中，将提供对 audio 元素的支持。

---

### &lt;audio&gt; 标签的属性

| 属性 | 值 | 描述
|------|----|-----
| [autoplay]() ![h5](img/h5.png) | autoplay | 如果出现该属性，则音频在就绪后马上播放
| [controls]() ![h5](img/h5.png) | controls | 如果出现该属性，则向用户显示控件，比如播放按钮
| [loop]() ![h5](img/h5.png) | loop | 如果出现该属性，则每当音频结束时重新开始播放
| [preload]() ![h5](img/h5.png) | preload | 如果出现该属性，则音频在页面加载时进行加载，并预备播放，如果使用 "autoplay"，则忽略该属性
| [src]() ![h5](img/h5.png) | url | 要播放的音频 URL

---
