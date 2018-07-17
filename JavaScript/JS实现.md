# JavaScript 使用

---

### HTML 中的脚本必须位于 &lt;script&gt; 与 &lt;/script&gt; 标签之间。

### 脚本可被放置在 HTML 页面的 &lt;body&gt; 和 &lt;head&gt; 部分中。

---

### &lt;script&gt; 标签

在 HTML 页面中插入 JavaScript，必须使用 &lt;script&gt; 标签。

那些老旧的实例可能会在 &lt;script&gt; 标签中使用 type="text/javascript"。现在已经不必这样做了。JavaScript 是所有现代浏览器以及 HTML5 中的默认脚本语言。

可以在文档中放入不限数量的脚本，脚本可位于 HTML 的 &lt;body&gt; 或 &lt;head&gt; 部分中，或者同时存在于两个部分中，通常的做法是把函数放入 &lt;head&gt; 部分中，或者放在页面底部。这样就可以把它们安置到同一处位置，不会干扰页面的内容。

---

### &lt;body&gt; 中的 JavaScript

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
</head>
<body>
    <script type="text/javascript">
        document.write("<p>this is a paragraph</p>")
    </script>
</body>
</html>
```

---

### &lt;head&gt; 中的 JavaScript

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function my_func() {
            // 获取 p 元素 
            p_dom = document.getElementById("demo");
            // 写入新内容
            p_dom.innerHTML = "this is a paragraph";
        }
    </script>
</head>
<body>
    <p id="demo"></p>
    <button type="button" onclick="my_func()">点击</button>
</body>
</html>
```

---

### 外部的 JavaScript 

也可以把脚本保存到外部文件中。外部文件通常包含被多个网页使用的代码。

外部 JavaScript 文件的文件扩展名是 .js。

如需使用外部文件，请在 &lt;script&gt; 标签的 "src" 属性中设置该 .js 文件：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript" src="/my.js"></script>
</head>
<body>
</body>
</html>
```

---
