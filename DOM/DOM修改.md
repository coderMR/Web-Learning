# HTML DOM - 修改

---

修改 HTML = 改变元素、属性、样式和事件。

---

### 修改 HTML 元素

修改 HTML DOM 意味着许多不同的方面：

* 改变 HTML 内容
* 改变 CSS 样式
* 改变 HTML 属性
* 创建新的 HTML 元素
* 删除已有的 HTML 元素
* 改变事件

---

### 创建 HTML 内容

改变元素内容的最简单的方法是使用 innerHTML 属性。

改变元素内容的最简单的方法是使用 innerHTML属性。

下面的例子改变一个 &lt;p&gt; 元素的 HTML 内容：

```
<html>
<body>

<p id="p1">Hello World!</p>

<script>
document.getElementById("p1").innerHTML="New text!";
</script>

</body>
</html>
```

---

### 改变 HTML 样式

通过 HTML DOM，您能够访问 HTML 元素的样式对象。

下面的例子改变一个段落的 HTML 样式：

```
<html>

<body>
<p id="p2">Hello world!</p>

<script>
document.getElementById("p2").style.color="blue";
</script>

</body>
</html>
```

---

### 创建新的 HTML 元素

如需向 HTML DOM 添加新元素，您首先必须创建该元素（元素节点），然后把它追加到已有的元素上。

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

---
