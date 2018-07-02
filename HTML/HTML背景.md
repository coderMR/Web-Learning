# HTML 背景

---

### 背景（Backgrounds）

&lt;body&gt; 拥有两个配置背景的属性。背景可以是颜色或者图像。

---

### 背景颜色（Bgcolor）

背景颜色属性将背景设置为某种颜色。属性值可以是某种颜色的英文单词、十六进制色、RGB值。

```
<body bgcolor="black"></body>
<body bgcolor="#FFFFFF"></body>
<body bgcolor="rgb(111, 222, 333)"></body>
```

---

### 背景（Background）

背景属性将背景设置为图像。属性值为地址的图片的资料路径（相对路径/绝对路径/URL）。如果图片小于屏幕尺寸，那么图片将在页面中进行重复显示。

```
<body background="./background.png">
<body background="~/Desktop/background.png">
<body background="http://www.w3school.com.cn/clouds.gif">
```

---

### 基本的注意事项 - 有用的提示

&lt;body&gt; 标签中的 bgcolor、background、text 属性在最新的 HTML 标准（HTML 4 和 XHTML）中已被废弃。W3C 在它们的推荐标准库中已删除这些属性。

应该使用层叠样式表（CSS）来定义 HTML 元素的布局和显示属性。

---
