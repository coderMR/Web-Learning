# CSS 伪元素

---

### CSS 伪元素用于向某些选择器设置特殊效果。

---

#### 语法

```
selector:pseudo-element {
    property: value;
}
```

CSS 类也可以与伪元素配合使用：

```
selector.class:pseudo-element {
    property: value;
}
```

---

### :first-line 伪元素

first-line 伪元素用于向文本的首行设置特殊样式。

在下面的例子中，浏览器会根据 first-line 伪元素中的样式对 p 元素的第一行文本进行格式化：

```
p:first-line {
    color: #FF0000;
    font-variant: small-caps;
}
```

注释："first-line" 伪元素只能用于块级元素。

注释：下面的属性可应用于 "first-line" 伪元素：

* font
* color
* background
* word-spacing
* letter-spacing
* text-decoration
* vertical-align
* text-transform
* line-height
* line-height
* clear

---

### :first-letter 伪元素

first-letter 伪元素用于向文本的首字母设置特殊样式：

```
p:first-letter {
    color: #FF0000;
    font-size: xx-large;
}
```

注释："first-letter" 伪元素只能用于块级元素。

注释：下面的属性可应用于 "first-letter" 伪元素：

* font
* color
* background
* margin
* padding
* border
* text-decoration
* verical-align (仅当 float 为 none 时)
* line-height
* float
* clear

---

### 伪元素和 CSS 类

伪元素可以与 CSS 类配合使用：

```
p.article:first-letter {
    color: #FF0000;
}

<p class="article">this is a paragraph</p>
```

上面的例子会使所有 class 为 atricle 的段落的首字母变为红色。

---

### 多重微元素

可以结合多个伪元素来使用。

在下面的例子中，段落的第一个字母将显示为红色，其字体大小为 xx-large。第一行中的其余文本将为蓝色，并以小型大写字母显示。段落中的其余文本将以默认字体大小和颜色来显示：

```
p:first-letter {
    color: #FF0000;
    font-size: xx-large;
}

p:first-line {
    color: #0000FF;
    font-variant: small-caps;  
}
```

---

### CSS2 - :before 伪元素

":before" 伪元素可以在元素的内容前面插入新内容。

下面的例子在每个 &lt;h1&gt; 元素的前面插入一副图片：

```
h1:before {
    content:url(logo.gif);
}
```

---

### CSS2 -:after 伪元素

":after" 伪元素可以在元素的内容之后插入新内容。

下面的例子在每个 &lt;h1&gt; 元素后面插入一副图片：

```
h1:after {
    content:url(logo.gif);
}
```

---

### 伪元素

W3C："W3C" 列指示出该属性在哪个 CSS 版本中定义（CSS1 还是 CSS2）。

| 属性 | 描述 | CSS
|------|------|-----
| :first-letter | 向文本的第一个字母添加特殊样式 | 1
| :first-line | 向文本的首行添加特殊样式 | 1
| :before | 在元素之前添加内容 | 2
| :after | 在元素之后添加内容 | 2

---
