# JavaScript 简介

---

### JavaScript 是世界上最流行的编程语言。

### 这门语言可用于 HTML 和 web，更可广泛用于服务器、PC、笔记本电脑、平板电脑和智能手机等设备。

---

### JavaScript 是脚本语言

* JavaScript 是一种轻量级的编程语言。
* JavaScript 是可插入 HTML 页面的编程代码。
* JavaScript 插入 HTML 页面后，可由所有的现代浏览器执行。

---

### JavaScript：写入 HTML 输出

```
<!DOCTYPE html>
<html>
<head>
  <title>JavaScript</title>
  <meta charset="utf-8">
</head>
<body>
    <script type="text/javascript">
        document.write("<h1>this is a heading</h1>");
        document.write("<p>this is a paragraph</p>")
    </script>
</body>
</html>
```

使用 document.write(""); 可向文档中插入 HTML 代码。

---

### JavaScript：对事件作出反应

```
<!DOCTYPE html>
<html>
<head>
  <title>JavaScript</title>
  <meta charset="utf-8">
</head>
<body>
    <button type="button" onclick="alert('弹出提示框')">按钮</button>
</body>
</html>
```

alert() 函数在 JavaScript 中并不常用，但它对于代码测试非常方便。

---

### JavaScript：改变 HTML 内容

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function modify_paragraph() {
            // 获取 id 为 paragraph 的文档元素
            dom_p = document.getElementById("paragraph");
            // 修改元素内容
            dom_p.innerHTML = "<h1>这是使用 JS 修改过后的文本</h1>";
        }
    </script>
</head>
<body>
    <p id="paragraph">这是一段文本原始的样子</p>
    <button type="button" onclick="modify_paragraph()">改变段落文本</button>
</body>
</html>
```

document.getElementById() 用于获取文档中的元素。

innerHTML 属性用于改变元素中的内容。

---

### JavaScript：改变 HTML 图像

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function switch_light() {
            // 获取 img 文档元素
            img_dom = document.getElementById("light");
            // 切换 img 元素的 src 属性
            if (img_dom.src == "http://www.w3school.com.cn/i/eg_bulboff.gif") {
                img_dom.src = "http://www.w3school.com.cn/i/eg_bulbon.gif";
            } else {
                img_dom.src = "http://www.w3school.com.cn/i/eg_bulboff.gif";
            }
        }
    </script>
</head>
<body>
    <img src="http://www.w3school.com.cn/i/eg_bulboff.gif" onclick="switch_light()" id="light" />
    <p>点击灯泡来点亮或熄灭灯泡</p>
</body>
</html>
```

在 JS 中，我们可以将 HTML 元素及其属性利用面向对象的方式随意修改！

---

### JavaScript：改变 HTML 样式

改变 HTML 元素的样式，属于改变 HTML 属性的变种。

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function modify_style() {
            // 获取 h1 元素
            h1_dom = document.getElementById("heading");
            // 修改 h1 元素的样式 通过 style 属性
            // h1_dom.style = "color: red";
            h1_dom.style.color = "red";
        }
    </script>
</head>
<body>
    <h1 id="heading">这是一个标题，可以利用 JS 修改元素的样式</h1>
    <button type="button" onclick="modify_style()">修改标题样式</button>
</body>
</html>
```

因为 HTML5 中行内样式属性 style 的存在，所有我们可以通过修改元素的 style 属性来修改元素的样式。可以使用 style = "red: color" 来重写整个样式属性，也可以使用 style.color = "red" 来修改单个样式。

---

### JavaScript：验证输入

JavaScript 常用于验证用户的输入。

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function validate() {
            // 获取 input 元素
            input_dom = document.getElementById("text_input");
            // 获取 input 元素中的文本
            text = input_dom.value;
            // 利用除法简单判断文本的类型
            if (text == "" || isNaN(text)) {
                alert("输入非数字");
            }
        }
    </script>
</head>
<body>
    <input type="text" id="text_input" />
    <button type="button" onclick="validate()">验证</button>
</body>
</html>
```

isNaN() 函数用来快速检测是否为数值型字符串。

可以使用 JS + 正则 实现表单验证。

---
