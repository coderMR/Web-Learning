# CSS3 文本效果

---

### CSS3 文本效果

CSS3 包含多个新的文本特性。

在本章中，您将学到如下文本属性：

* text-shadow
* word-wrap

---

Internet Explorer 10、Firefox、Chrome、Safari 以及 Opera 支持 text-shadow 属性。

所有主流浏览器都支持 word-wrap 属性。

注释：Internet Explorer 9 以及更早的版本，不支持 text-shadow 属性。

---

### CSS3 文本阴影

在 CSS3 中，text-shadow 可向文本应用阴影。

您能够规定水平阴影、垂直阴影、模糊距离，以及阴影的颜色：

向标题添加阴影：

```
h1 {
    text-shadow: 5px 5px 5px #FF0000;
}
```

---

### CSS3 自动换行

单词太长的话就可能无法超出某个区域：

在 CSS3 中，word-wrap 属性允许文本强制进行换行 - 即使这意味着会对单词进行拆分：

```
p {
    word-wrap: break-word;
}
```

---

### 新的文本属性

<table class="dataintable">
<tr>
<th style="width:25%;">属性</th>
<th>描述</th>
<th style="width:5%;">CSS</th>
</tr>

<tr>
<td><a href="/cssref/pr_hanging-punctuation.asp" title="CSS3 hanging-punctuation 属性">hanging-punctuation</a></td>
<td>规定标点字符是否位于线框之外。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_punctuation-trim.asp" title="CSS3 punctuation-trim 属性">punctuation-trim</a></td>
<td>规定是否对标点字符进行修剪。</td>
<td>3</td>
</tr>

<tr>
<td>text-align-last</td>
<td>设置如何对齐最后一行或紧挨着强制换行符之前的行。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_text-emphasis.asp" title="CSS3 text-emphasis 属性">text-emphasis</a></td>
<td>向元素的文本应用重点标记以及重点标记的前景色。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_text-justify.asp" title="CSS3 text-justify 属性">text-justify</a></td>
<td>规定当  text-align 设置为 &quot;justify&quot; 时所使用的对齐方法。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_text-outline.asp" title="CSS3 text-outline 属性">text-outline</a></td>
<td>规定文本的轮廓。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_text-overflow.asp" title="CSS3 text-overflow 属性">text-overflow</a></td>
<td>规定当文本溢出包含元素时发生的事情。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_text-shadow.asp" title="CSS3 text-shadow 属性">text-shadow</a></td>
<td>向文本添加阴影。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_text-wrap.asp" title="CSS3 text-wrap 属性">text-wrap</a></td>
<td>规定文本的换行规则。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_word-break.asp" title="CSS3 word-break 属性">word-break</a></td>
<td>规定非中日韩文本的换行规则。</td>
<td>3</td>
</tr>

<tr>
<td><a href="/cssref/pr_word-wrap.asp" title="CSS3 word-wrap 属性">word-wrap</a></td>
<td>允许对长的不可分割的单词进行分割并换行到下一行。</td>
<td>3</td>
</tr>
</table>

---
