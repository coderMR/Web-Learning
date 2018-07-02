# XHTML 简介

---

### XHTML 是以 XML 格式编写的 HTML

---

### 什么是 XHTML ？

* XHTML 指的是可扩展超文本标记语言
* XHTML 与 HTML 4.01 几乎是相同的
* XHTML 是更严格更纯净的 HTML 版本
* XHTML 是以 XML 应用的方式定义的 HTML
* XHTML 得到所有主流浏览器的支持

---

### 为什么使用 XHTML ？

Internet上很多页面包含了糟糕的 HTML。

如果在浏览器中查看，下面的 HTML 代码运行起来非常正常（即使它并未遵守 HTML 规则）。

```
<html>
    <head>
        <title>This is bad HTML</title>
    <body>
        <h1>Bad HTML
        <p>This is a paragraph
    </body>
```

XML 是一种必须正确标记且格式良好的标记语言。

今日的科学界存在一些不同的浏览器技术，其中一些在计算机上运行，而另一些可能在移动设备或其他小型设备上运行。小型设备往往缺乏处理"糟糕"的标记语言的资源和能力。

所以，通过结合 XML 和 HTML 的长处，开发出了 XHTML，XHTML 是作为 XML 被重新设计的 HTML。

与 HTML 相比最重要的区别：

#### 文档结构

* XHTML DOCTYPE 是强制性的
* &lt;html&gt; 中的 XML namespace 属性是强制性的
* &lt;html&gt;、&lt;head&gt、&lt;title&gt; 以及 &lt;body&gt; 也是强制性的

#### 元素语法

* XHTML 元素必须正确嵌套
* XHTML 元素必须始终关闭
* XHTML 元素必须小写
* XHTML 文档必须有一个根元素

#### 属性语法

* XHTML 属性必须使用小写
* XHTML 属性值必须用引号包围
* XHTML 属性最小化也是禁止的

---

### &lt;!DOCTYPE&gt; 是强制性的

XHTML 文档必须进行 XHTML 文档类型声明

&lt;html&gt;、&lt;head&gt、&lt;title&gt; 以及 &lt;body&gt; 也必须存在，并且必须使用 &lt;html&gt; 中的 xmlns 属性为文档规定 xml 命名空间。

下面的例子展示了带有最少的必需标签的 XHTML 文档：

```
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" 
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
    <head>
        <title>Title of document</title>
    </head>
    <body>
        ......
    </body>
</html>
```

---

### 如何从 HTML 转换到 XHTML

1.向每张页面的第一行添加 XHTML &lt;!DOCTYPE&gt;
2.向每张页面的 html 元素添加 xmlns 属性
3.把所有元素命名改为小写
4.关闭所有空元素
5.把所有属性名改为小写
6.为所有属性值加引号


