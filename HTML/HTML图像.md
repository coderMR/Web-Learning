# HTML 图像

---

### 通过使用 HTML，可以在文档中显示图像。

---

### 图像标签（&lt;img&gt;）和源属性（Src）

在 HTML 中，图像由 &lt;img&gt; 标签定义。

&lt;img&gt; 是空标签，只包含属性，没有闭合标签。

要在页面上显示图像，你需要使用源属性（src）。src 指 "source"。源属性的值是图像的 URL 地址。

语法：

```
<img src="url" />
```

URL 指存储图片的位置。如果名为 "boat.gif" 的图片位于 www.w3school.com.cn 的 images 目录中，那么其 URL 为 http://www.w3school.com.cn/images/boat.gif。

---

### 基本的注意事项 - 有用的提示

假如某个 HTML 文件包含十个图像，那么为了正确显示这个页面，需要加载 11 个文件。加载图片是需要时间的，所以我们的建议是：慎用图片。

---

### 背景图片

本例演示如何向 HTML 页面添加背景图片。

```
<body background="img/background.png">
</body>
```

注释：如果图片小于页面，图片会重复。

---

### 排列图片

本例演示如何在文字中排列图片

```
<p>图像<img src="img/image.png" />在文本中</p>
<p>图像<img src="img/image.png" align="bottom" />在文本中</p>
<p>图像<img src="img/image.png" align="middle" />在文本中</p>
<p>图像<img src="img/image.png" align="top" />在文本中</p>
```

注释：默认为 bottom 的对齐方式。

---

### 浮动图片

本例演示如何使图片浮动至段落的左边或右边。

```
<p><img src="img/image/png" align="left /">带有图像的一个段落。图像的 align 属性设置为 "left"。图像将浮动到文本的左侧。</p>
<p><img src="img/image/png" align="right /">带有图像的一个段落。图像的 align 属性设置为 "right"。图像将浮动到文本的左侧。</p>
```

---

### 调整图片尺寸

本例演示如何使图片调整到不同尺寸。

```
<img src="img/image.png" width="100" height="200" />
<img src="img/image.png" width="200" height="400" />
<img src="img/image.png" width="300" height="600" />
```

注释：通过改变 &lt;img&gt; 标签的 height 和 width 属性值，可以放大缩小图片。

---

### 为图片替换文本

本例演示如何为图片替换文本。在浏览器无法载入图片时，替换文本属性告诉读者们丢失的信息。为页面的图片添加上替换文本是个好习惯。

```
<img src="img/image.png" alt="这是替换文本" />
```

注释：大多数浏览器，将鼠标移动至图片，会显示其替换文本内容。

---

### 创建图像映射

本例演示如何创建带有可供点击区域的图像地图，其中的每一个区域都是一个超链接。

```
<img src="http://www.w3school.com.cn/i/eg_planets.jpg" usemap="#planetmap" alt="Planets"/>

<map name="planetmap" id="planetmap">

<area shape="circle" coords=="180,139,14" href="https://www.baidu.com" target="_blank"/>
<area shape="circle" coords="129,161,10" href ="https://www.baidu.com" target ="_blank" />
<area shape="rect" coords="0,0,110,260" href ="https://www.baidu.com" target ="_blank" />
```

注释：img 元素中的 usemap 属性引用 map 元素中的 id 或者 name 属性（根据浏览器），所以我们同时为 map 元素添加了 id 和 name 属性。

---

### 把图片转换为图片映射

本例显示如何把一副普通的图片设置为图片映射。

```
<a href="http://www.w3school.com.cn/example/html/html_ismap.html">
<img src="http://www.w3school.com.cn/i/eg_planets.jpg" ismap />
</a>
```

--- 

### 图像标签

| 标签 | 描述
|------|-----
| &lt;img&gt; | 定义图片
| &lt;map&gt; | 定义图片地图
| &lt;area&gt; | 定义图片中可点击的区域

---
