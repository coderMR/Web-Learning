# CSS3 3D 转换

---

### 3D 转换

CSS3 允许您使用 3D 转换来对元素进行格式化。

在本章中，您将学到其中的一些 3D 转换方法

* rotateX()
* rotateY()

转换是使元素改变形状、尺寸和位置的一种效果。

您可以使用 2D 或 3D 转换来转换您的元素。

---

Internet Explorer 10 和 Firefox 支持 3D 转换。

Chrome 和 Safari 需要前缀 -webkit-。

Opera 仍然不支持 3D 转换（它只支持 2D 转换）。

---

### rotateX() 方法

通过 rotateX() 方法，元素围绕其 X 轴以给定的度数进行旋转。

```
div
{
transform: rotateX(120deg);
-webkit-transform: rotateX(120deg);	/* Safari 和 Chrome */
-moz-transform: rotateX(120deg);	/* Firefox */
}
```

---

### rotateY() 旋转

通过 rotateY() 方法，元素围绕其 Y 轴以给定的度数进行旋转。

```
div
{
transform: rotateY(130deg);
-webkit-transform: rotateY(130deg);	/* Safari 和 Chrome */
-moz-transform: rotateY(130deg);	/* Firefox */
}
```

### 转换属性

下面的表格列出了所有的转换属性：

<table class="dataintable">
<tr>
<th style="width:25%;">属性</th>
<th>描述</th>
<th style="width:5%;">CSS</th>
</tr>

<tr>
<td><a href="/cssref/pr_transform.asp" title="CSS3 transform 属性">transform</a></td>
<td>向元素应用 2D 或 3D 转换。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_transform-origin.asp" title="CSS3 transform-origin 属性">transform-origin</a></td>
<td>允许你改变被转换元素的位置。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_transform-style.asp" title="CSS3 transform-style 属性">transform-style</a></td>
<td>规定被嵌套元素如何在 3D 空间中显示。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_perspective.asp" title="CSS3 perspective 属性">perspective</a></td>
<td>规定 3D 元素的透视效果。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_perspective-origin.asp" title="CSS3 perspective-origin 属性">perspective-origin</a></td>
<td>规定 3D 元素的底部位置。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_backface-visibility.asp" title="CSS3 backface-visibility 属性">backface-visibility</a></td>
<td>定义元素在不面对屏幕时是否可见。</td>
<td>3</td>
</tr>

</table>

---

### 2D Transform 方法

m 方法</h2>

<table class="dataintable">
<tr>
<th style="width:25%;">函数</th>
<th>描述</th>
</tr>

<tr>
<td>matrix3d(<i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>,<br/><i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>,<i>n</i>)</td>
<td>定义 3D 转换，使用 16 个值的 4x4 矩阵。</td>
</tr>

<tr>
<td>translate3d(<i>x</i>,<i>y</i>,<i>z</i>)</td>
<td>定义 3D 转化。</td>
</tr>

<tr>
<td>translateX(<i>x</i>)</td>
<td>定义 3D 转化，仅使用用于 X 轴的值。</td>
</tr>

<tr>
<td>translateY(<i>y</i>)</td>
<td>定义 3D 转化，仅使用用于 Y 轴的值。</td>
</tr>

<tr>
<td>translateZ(<i>z</i>)</td>
<td>定义 3D 转化，仅使用用于 Z 轴的值。</td>
</tr>

<tr>
<td>scale3d(<i>x</i>,<i>y</i>,<i>z</i>)</td>
<td>定义 3D 缩放转换。</td>
</tr>

<tr>
<td>scaleX(<i>x</i>)</td>
<td>定义 3D 缩放转换，通过给定一个 X 轴的值。</td>
</tr>

<tr>
<td>scaleY(<i>y</i>)</td>
<td>定义 3D 缩放转换，通过给定一个 Y 轴的值。</td>
</tr>

<tr>
<td>scaleZ(<i>z</i>)</td>
<td>定义 3D 缩放转换，通过给定一个 Z 轴的值。</td>
</tr>

<tr>
<td>rotate3d(<i>x</i>,<i>y</i>,<i>z</i>,<i>angle</i>)</td>
<td>定义 3D 旋转。</td>
</tr>

<tr>
<td>rotateX(<i>angle</i>)</td>
<td>定义沿 X 轴的 3D 旋转。</td>
</tr>

<tr>
<td>rotateY(<i>angle</i>)</td>
<td>定义沿 Y 轴的 3D 旋转。</td>
</tr>

<tr>
<td>rotateZ(<i>angle</i>)</td>
<td>定义沿 Z 轴的 3D 旋转。</td>
</tr>

<tr>
<td>perspective(<i>n</i>)</td>
<td>定义 3D 转换元素的透视视图。</td>
</tr>
</table>

---
