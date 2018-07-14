# CSS 网络安全字体组合

---

### 常用的字体组合

font-family 属性应该使用若干种字体名称作为回退系统，以确保浏览器/操作系统之间的最大兼容性。如果浏览器不支持第一个字体，则会尝试下一个。

请以您喜欢的字体开始，并以通用字体系列结束，以便使浏览器在通用系统中挑选相似的字体，如果没有其他字体可用的话：

```
p {
    font-family: 'Times New Roman', Times, serif;
}
```

下面是最常用的字体组合，根据通用系统进行汇总：

<table class="dataintable">
<tr>
<th style="width:60%;">font-family</th>
<th>示例文本</th>
</tr>

<tr>
<td>Georgia, serif</td>
<td>
	<h2 style="font-family:Georgia, serif;">This is a heading</h2>
	<p style="font-family:Georgia, serif;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>'Palatino Linotype', 'Book Antiqua', Palatino, serif</td>
<td>
	<h2 style="font-family:'Palatino Linotype', 'Book Antiqua', Palatino, serif;">This is a heading</h2>
	<p style="font-family:'Palatino Linotype', 'Book Antiqua', Palatino, serif;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>'Times New Roman', Times, serif</td>
<td>
	<h2 style="font-family:'Times New Roman', Times, serif;">This is a heading</h2>
	<p style="font-family:'Times New Roman', Times, serif;">This is a paragraph</p>
</td>
</tr>
</table>

---

### Sans-Serif 字体

<table class="dataintable">
<tr>
<th style="width:60%;">font-family</th>
<th>示例文本</th>
</tr>

<tr>
<td>Arial, Helvetica, sans-serif</td>
<td>
	<h2 style="font-family:Arial, Helvetica, sans-serif;">This is a heading</h2>
	<p style="font-family:Arial, Helvetica, sans-serif;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>'Arial Black', Gadget, sans-serif</td>
<td>
	<h2 style="font-family:'Arial Black', Gadget, sans-serif;">This is a heading</h2>
	<p style="font-family:'Arial Black', Gadget, sans-serif;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>'Comic Sans MS', cursive, sans-serif</td>
<td>
	<h2 style="font-family:'Comic Sans MS', cursive, sans-serif;">This is a heading</h2>
	<p style="font-family:'Comic Sans MS', cursive, sans-serif;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>Impact, Charcoal, sans-serif</td>
<td>
	<h2 style="font-family:Impact, Charcoal, sans-serif;">This is a heading</h2>
	<p style="font-family:Impact, Charcoal, sans-serif;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>'Lucida Sans Unicode', 'Lucida Grande', sans-serif</td>
<td>
	<h2 style="font-family:'Lucida Sans Unicode', 'Lucida Grande', sans-serif;">This is a heading</h2>
	<p style="font-family:'Lucida Sans Unicode', 'Lucida Grande', sans-serif;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>Tahoma, Geneva, sans-serif</td>
<td>
	<h2 style="font-family:Tahoma, Geneva, sans-serif;">This is a heading</h2>
	<p style="font-family:Tahoma, Geneva, sans-serif;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>'Trebuchet MS', Helvetica, sans-serif</td>
<td>
	<h2 style="font-family:'Trebuchet MS', Helvetica, sans-serif;">This is a heading</h2>
	<p style="font-family:'Trebuchet MS', Helvetica, sans-serif;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>Verdana, Geneva, sans-serif</td>
<td>
	<h2 style="font-family:Verdana, Geneva, sans-serif;">This is a heading</h2>
	<p style="font-family:Verdana, Geneva, sans-serif;">This is a paragraph</p>
</td>
</tr>
</table>

---

### Monospace 字体

<table class="dataintable">
<tr>
<th style="width:60%;">font-family</th>
<th>示例文本</th>
</tr>

<tr>
<td>'Courier New', Courier, monospace</td>
<td>
	<h2 style="font-family:'Courier New', Courier, monospace;">This is a heading</h2>
	<p style="font-family:'Courier New', Courier, monospace;">This is a paragraph</p>
</td>
</tr>

<tr>
<td>'Lucida Console', Monaco, monospace</td>
<td>
	<h2 style="font-family:'Lucida Console', Monaco, monospace;">This is a heading</h2>
	<p style="font-family:'Lucida Console', Monaco, monospace;">This is a paragraph</p>
</td>
</tr>
</table>

---
