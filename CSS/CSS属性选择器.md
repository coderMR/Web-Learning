# CSS 属性选择器

---

### 对带有指定属性的 HTML

可以为拥有指定属性的 HTML 元素设置样式，而不仅限于 class 和 id 属性。

注释：只有在规定了 ！DOCTYPE 时，IE7 和 IE8 才支持属性选择器。在 IE6 及更低的版本中，不支持属性选择。

---

### 属性选择器

下面的例子为带有 title 属性的所有元素设置样式：

```
[title]
{
    color: red;
}
```

### 属性和值选择器

下面的例子为 title="W3School" 的所有元素设置样式：

```
[title=W3School]
{
border: 5px solid blue;
}
```

---

### 属性和值选择器 - 多个值

```
[title~=hello]
{
    color: red;
}
```

下面的例子为带有包含指定值的 lang 属性的所有元素设置样式。适用于由连字符分割的属性值：

```
[lang |=en]
{
    color: red;
}
```

---

### 设置表单的样式

属性选择器在为不带有 class 或 id 的表单设置样式时特别有用：

```
input[type="text"]
{
    width: 150px;
    display: block;
    margin-bottom: 10px;
    background-color: yellow;
    font-family: Verdana, Arial;
}

input[type="button"]
{
    width: 120px;
    margin-left: 35px;
    display: block;
    font-family: Verdana, Arial;
}
```

---

### CSS 选择器参考手册

| 选择器 | 描述
|--------|-----
| [attribute] | 用于选取带有指定属性的元素。
| [attribute=value] | 用于选取带有指定属性和值的元素。
| [attribute~=value] | 用于选取属性值中包含指定词汇的元素。
| [attribute|=value] | 用于选取带有以指定值开头的属性值的元素，该值必须是整个单词。
| [attribute^=value] | 匹配属性值以指定值开头的每个元素。
| [attribute$=value] | 匹配属性值以指定值结尾的每个元素。
| [attribute*=value] | 匹配属性值中包含指定值的每个元素。

---
