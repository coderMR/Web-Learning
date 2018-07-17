# HTML DOM - 元素

---

添加、删除和替换 HTML 元素。

---

### 创建新的 HTML 元素 - appendChild()

如需向 HTML DOM 添加新元素，您首先必须创建该元素，然后把它追加到已有的元素上。

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
</head>
<body>
    <div id="div1">
        <p id="p1">This is a paragraph.</p>
        <p id="p2">This is another paragraph.</p>
    </div>
    <script>
        var para=document.createElement("p");
        var node=document.createTextNode("This is new.");
        para.appendChild(node);
        var element=document.getElementById("div1");
        element.appendChild(para);
    </script>
</body>
</html>
```

### 例子解释

这段代码创建了一个新的 &lt;p&gt; 元素：

```
var para = document.createElement("p");
```

如需向 &lt;p&gt; 元素添加文本，首先必须创建文本节点

```
var node = document.createTextNode("this is a new paragraph");
```

然后必须向 &lt;p&gt; 元素追加文本节点：

```
para.appendChild(node);
```

最后，您必须向已有元素追加这个新元素

```
var element=document.getElementById("div1");
element.appendChild(para);
```

---

### 创建新的 HTML 元素 - insertBefore()

上一个例子中的 appendChild() 方法，将新元素作为父元素的最后一个子元素进行添加。

如果不希望如此，可以使用 insertBefore() 方法：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
</head>
<body>
    <div id="div1">
        <p id="p1">This is a paragraph.</p>
        <p id="p2">This is another paragraph.</p>
    </div>
    <script>
        var para=document.createElement("p");
        var node=document.createTextNode("This is new.");
        para.appendChild(node);
        var element=document.getElementById("div1");
        var child=document.getElementById("p1");
        element.insertBefore(para,child);
    </script>
</body>
</html>
```

---

### 删除已有的 HTML 元素

如需删除 HTML 元素，您必须清楚该元素的父元素：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
</head>
<body>
    <div id="div1">
        <p id="p1">This is a paragraph.</p>
        <p id="p2">This is another paragraph.</p>
    </div>
    <script>
        var parent=document.getElementById("div1");
        var child=document.getElementById("p1");
        parent.removeChild(child);
    </script>
</body>
</html>
```

### 例子解释

这个 HTML 文档包含一个带有两个子节点的 &lt;div&gt; 元素：

```
<div id="div1">
<p id="p1">This is a paragraph.</p>
<p id="p2">This is another paragraph.</p>
</div>
```

查找 id="div1" 的元素：

```
var parent=document.getElementById("div1");
```

查找 id = "p1" 的 &lt;p&gt; 元素：

```
var child=document.getElementById("p1");
```

从父元素中删除子元素：

```
parent.removeChild(child);
```

提示：能否在不引用父元素的情况下删除某个元素？

很抱歉。DOM 需要了解您需要删除的元素，以及它的父元素。

这里提供一个常用的解决方法：找到您需要删除的子元素，然后使用 parentNode 属性来查找其父元素：

```
var child=document.getElementById("p1");
child.parentNode.removeChild(child);
```

---

### 替换 HTML 元素

如需替换 HTML DOM 中的元素，请使用 replaceChild() 方法：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
</head>
<body>
    <div id="div1">
        <p id="p1">This is a paragraph.</p>
        <p id="p2">This is another paragraph.</p>
    </div>
    <script>
        var para=document.createElement("p");
        var node=document.createTextNode("This is new.");
        para.appendChild(node);
        
        var parent=document.getElementById("div1");
        var child=document.getElementById("p1");
        parent.replaceChild(para,child);
    </script>
</body>
</html>
```

---
