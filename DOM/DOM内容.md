# HTML DOM - 修改 HTML 内容

---

通过 HTML DOM，JavaScript 能够访问 HTML 文档中的每个元素。

---

### 改变 HTML 内容

改变元素内容的最简单的方法是使用 innerHTML 属性。

下面的例子更改 &lt;p&gt; 元素的 HTML 内容：

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

通过 HTML DOM，您能够访问 HTML 对象的样式对象。

下面的例子更改段落的 HTML 样式：

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

### 使用事件 

HTML DOM 允许您在事件发生时执行代码。

当 HTML 元素”有事情发生“时，浏览器就会生成事件：

* 在元素上点击
* 加载页面
* 改变输入字段

下面例子在按钮被点击时改变 &lt;body&gt; 元素的背景色：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
</head>
<body>
    <input type="button" value="改变背景色" onclick="document.body.style.backgroundColor='lavender';" />
</body>
</html>
```

下面的例子在按钮被点击时改变 &lt;p&gt; 元素的文本：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function ChangeText() {
            document.getElementById("p1").innerHTML = "Nex text";
        }
    </script>
</head>
<body>
    <p id="p1">Hello world!</p>
    <input type="button" onclick="ChangeText()" value="Change text" />
</body>
</html>
```

---
