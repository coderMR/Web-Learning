# CSS ID 选择器详解

---

### ID 选择器允许以一种独立于文档元素的方式来指定样式。

---

### CSS ID 选择器

在某些方面，id 选择器类似于类选择器，不过也有一些重要差别。

#### 语法

首先，id 选择器前面有一个 # 号 - 也称为棋盘号或井号。

请看下面的规则：

```
*#intro {
    font-weight: bold;
}
```

与类选择器一样，id 选择器中可以忽略通配选择器，前面的例子也可以写作：

```
#intro {
    font-weight: bold;
}
```

这个选择器的效果将是一样的。

第二个区别是 id 选择器不引用 class 属性的值，毫无疑问，它要引用 id 属性中的值。

以下是一个实际 id 选择器的例子：

```
<p id="intro">
this is a paragraph
</p>
```

---

### 类选择器还是 id 选择器？

在类选择器这一节中我们曾将结果，可以任意多个元素指定类。前一节类名 important 被应用到 p 和 h1 元素，而且它还可以应用到更多元素。

#### 区别1：只能在文档中使用一次

与类不同，在一个 HTML 文档中，id 选择器会使用一次，而且仅一次。

#### 区别2：不能使用 id 词列表

不同于类选择器，id 选择器不能结合使用，因为 id 属性不允许以空格分隔的词列表。

#### 区别3：id 能包含更多含义

类似于类，可以独立元素来选择 id。有些情况下，您指定文档中会出现某个特定 id 值，但是并不知道它会出现在哪个元素上，所有你想声明独立的 id 选择器。例如，您可能知道在一个给定的文档中会有一个 id 值为 mostImportant 的元素。您不知道这个最重要的东西是一个段落、一个短语、一个列表项还是一个小节标题。您只知道每个文档都会有这么一个最重要的内容，它可能在任何元素中，而且只能出现一个。在这种情况下，可以编写如下规则：

```
#mostImportant {
    color: red;
    background: yellow;
}
```

这个规则会与以下各个元素匹配（这些元素不能在同一个文档中同时出现，因为它们都有相同的 id 值）：

```
<h1 id="mostImportant">This is important!</h1>
<em id="mostImportant">This is important!</em>
<ul id="mostImportant">This is important!</ul>
```

---

### 区分大小写

请注意，类选择器和 id 选择器可能是区分大小写的。这取决于文档的语言。HTML 和 XHTML 将类和 id 值定义为区分大小写，所以类和 id 值得大小写必须与文档中的相应值匹配。

因此，对于以下的 CSS 和 HTML，元素不会变成粗体：

```
#intro {
    font-weight: bold;
}

<p id="Intro">this is a paragraph</p>
```

由于字母 i 的大小写不同，所以选择器不会匹配上面的元素。

---
