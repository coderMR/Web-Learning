# CSS 图像透明

---

通过 CSS 创建透明图像是很容易的。

注释：CSS opacity 属性是 W3C CSS 推荐标准的一部分。

---

### 实例 1 - 创建透明图像

定义透明效果的 CSS3 属性是 opacity。

首先，我们将展示如何通过 CSS 来创建透明图像。

常规图像：

![tulip_peach_blossom_w_s](img/tulip_peach_blossom_w_s.jpg)

带有透明度的相同图像：

<img src="img/tulip_peach_blossom_w_s.jpg" style="opacity: 0.4" />

情况下面的 CSS：

```
img
{
opacity:0.4;
filter:alpha(opacity=40); /* 针对 IE8 以及更早的版本 */
}
```

IE9, Firefox, Chrome, Opera 和 Safari 使用属性 opacity 来设定透明度。opacity 属性能够设置的值从 0.0 到 1.0。值越小，越透明。

IE8 以及更早的版本使用滤镜 filter:alpha(opacity=x)。x 能够取的值从 0 到 100。值越小，越透明。

---

### 实例 2 - 图片透明度 - Hover 效果

<style>
.hov
{
opacity:0.4;
filter:alpha(opacity=40); /* 针对 IE8 以及更早的版本 */
}
img.hov:hover
{
opacity:1.0;
filter:alpha(opacity=100); /* 针对 IE8 以及更早的版本 */
}
</style>

<img class="hov" src="img/tulip_peach_blossom_w_s.jpg" />

CSS 是这样的：

```
img
{
opacity:0.4;
filter:alpha(opacity=40); /* 针对 IE8 以及更早的版本 */
}
img:hover
{
opacity:1.0;
filter:alpha(opacity=100); /* 针对 IE8 以及更早的版本 */
}
```

第一个 CSS 代码块类似实例 1 中的代码。此外，我们已经设置了当鼠标指针位于图像上时的样式。在这个例子中，当指针移动到图像上时，我们希望图像是不透明的。

对应的 CSS 是：opacity=1。

IE8 以及更早的浏览器：filter:alpha(opacity=100)。

当鼠标指针移出图像后，图像会再次透明。

---

### 实例 3 - 透明框中的文本

<style>
div.background
{
  width: 400px;
  height: 266px;
  background: url(img/tulip_peach_blossom_w_s.jpg) no-repeat;
  border: 1px solid black;
}

div.transbox
{
  width: 338px;
  height: 204px;
  margin:30px;
  background-color: #ffffff;
  border: 1px solid black;
  /* for IE */
  filter:alpha(opacity=60);
  /* CSS3 standard */
  opacity:0.6;
}

div.transbox p
{
  margin: 30px 40px;
}
</style>
</head>

<body>

<div class="background">
<div class="transbox">
<p>
This is some text that is placed in the transparent box.
This is some text that is placed in the transparent box.
This is some text that is placed in the transparent box.
This is some text that is placed in the transparent box.
This is some text that is placed in the transparent box.
</p>
</div>
</div>

首先，我们创建一个 div 元素 (class="background")，它有固定的高度和宽度、背景图像，以及边框。然后我们在第一个 div 内创建稍小的 div (class="transbox")。"transbox" div 有固定的宽度、背景色和边框 - 并且它是透明的。在透明 div 内部，我们在 p 元素中加入了一些文本。

---
