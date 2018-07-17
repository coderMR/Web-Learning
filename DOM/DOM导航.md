# HTML DOM - 导航

---

通过 HTML DOM，您能够使用节点关系在节点树中导航。

---

### HTML DOM 节点列表

getElementsByTagName() 方法返回节点列表。节点列表是一个节点数组。

下面的代码选取文档中的所有 &lt;p&gt; 节点：

```
var x=document.getElementsByTagName("p");
```

可以通过下标号访问这些节点。如需访问第二个 <p>，您可以这么写：

```
y=x[1];
```

---

### HTML DOM 节点列表长度

length 属性定义节点列表中节点的数量。

您可以使用 length 属性来循环节点列表：

```
x=document.getElementsByTagName("p");

for (i=0;i<x.length;i++)
{
document.write(x[i].innerHTML);
document.write("<br />");
}
```

---

### 导航节点关系

您能够使用三个节点属性：parentNode、firstChild 以及 lastChild ，在文档结构中进行导航。

```
<html>
<body>

<p>Hello World!</p>
<div>
  <p>DOM 很有用!</p>
  <p>本例演示节点关系。</p>
</div>

</body>
</html>
```

* 首个 &lt;p&gt; 元素是 &lt;body&gt; 元素的首个子元素（firstChild）
* &lt;div&gt; 元素是 &lt;body&gt; 元素的最后一个子元素（lastChild）
* &lt;body&gt; 元素是首个 &lt;p&gt; 元素和 &lt;div&gt; 元素的父节点（parentNode）

firstChild 属性可用于访问元素的文本：

```
<html>
<body>

<p id="intro">Hello World!</p>

<script>
x=document.getElementById("intro");
document.write(x.firstChild.nodeValue);
</script>

</body>
</html>
```

---

### DOM 根节点

这里有两个特殊的属性，可以访问全部文档：

* document.documentElement - 全部文档
* document.body - 文档的主体

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        alert(document.body.innerHTML);
    </script>
</head>
<body>
    <p>Hello World!</p>
    <div>
        <p>DOM 很有用！</p>
        <p>本例演示 <b>document.body</b> 属性。</p>
    </div>
</body>
</html>
```

---

### childNodes 和 nodeValue

除了 innerHTML 属性，您也可以使用 childNodes 和 nodeValue 属性来获取元素的内容。

下面的代码获取 id="intro" 的 <p> 元素的值：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        var txt=document.getElementById("intro").childNodes[0].nodeValue;
        document.write(txt);
    </script>
</head>
<body>
    <p id="intro">Hello World!</p>
</body>
</html>
```

---
