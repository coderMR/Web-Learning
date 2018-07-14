# CSS3 边框

---

### CSS3 边框

通过 CSS3，可以创建圆角边框，向矩形添加阴影，使用图片来绘制边框 - 并且不需使用设计软件。

本节讲解以下边框属性：

* border-radius
* box-shadow
* border-image

---

Internet Explorer 9+ 支持 border-radius 和 box-shadow 属性。

Firefox、Chrome 以及 Safari 支持所有新的边框属性。

注释：对于 border-image，Safari 5 以及更老的版本需要前缀 -webkit-。

Opera 支持 border-radius 和 box-shadow 属性，但是对于 border-image 需要前缀 -o-。

---

### CSS3 圆角边框

在 CSS2 中添加圆角矩形需要技巧。我们必须为每个圆角使用不同的图片。

在 CSS3 中，创建圆角是非常容易的。

在 CSS3 中，border-radius 属性用于创建圆角：

向 div 元素添加圆角：

```
div {
    border: 2px solid;
    border-radius: 25px;
    -moz-border-radius: 25px;
}
```

---

### CSS3 边框阴影

在 CSS3 中，box-shadow 用于向方框添加阴影：

```
div {
    box-shadow: 10px 10px 5px #888888;
}
```

---

### CSS3 边框图片

通过 CSS3 的 border-image 属性，可以使用图片来创建边框：

```
div
{
    border-image:url(border.png) 30 30 round;
    -moz-border-image:url(border.png) 30 30 round; /* 老的 Firefox */
    -webkit-border-image:url(border.png) 30 30 round; /* Safari 和 Chrome */
    -o-border-image:url(border.png) 30 30 round; /* Opera */
}
```

### 新的边框属性

| 属性 | 描述 | CSS
|------|------|----
| [border-image]() | 设置所有 border-image-* 属性的简写属性。 | 3
| [border-radius]() | 设置所有四个 border-*-radius 属性的简写属性。| 3
| [border-shadow]() | 向方框添加一个或多个阴影。 | 3

---
