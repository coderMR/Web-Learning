# HTML DOM - 事件

---

HTML DOM 允许 JavaScript 对 HTML 事件作出反应。。

---

### 对事件作出反应

当事件发生时，可以执行 JavaScript，比如当用户点击一个 HTML 元素时。

如需在用户点击某个元素时执行代码，请把 JS 代码添加到 HTML 事件属性中：

```
onclick = JS
```

HTML 事件的例子：

* 当用户点击鼠标时
* 当网页已加载时
* 当图片已加载时
* 当鼠标移动到元素上时
* 当输入字段被改变时
* 当 HTML 表单被提交时
* 当用户触发按键时

在本例中，当用户点击时，会改变 &lt;h1&gt; 元素的内容：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
</head>
<body>
    <h1 onclick="this.innerHTML='hello!'">请点击这段文本！</h1>
</body>
</html>
```

在本例中，会从事件处理程序中调用函数：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function changetext(id) {
            id.innerHTML="hello!";
        }
    </script>
</head>
<body>
    <h1 onclick="changetext(this)">请点击这段文本！</h1>
</body>
</html>
```

---

### HTML 事件属性

如需向 HTML 元素分配事件，您可以使用事件属性。

实例：

向 button 元素分配一个 onclick 事件：

```
<button onclick="displayDate()">试一试</button>
```

---

### onload 和 onunload 事件

当用户进入或离开页面时，会触发 onload 和 onunload 事件。

onload 事件可用于检查访客的浏览器类型和版本，以便基于这些信息来加载不同版本的网页。

onload 和 onunload 事件可用于处理 cookies。

实例：

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function checkCookies() {
            if (navigator.cookieEnabled==true) {
                alert("Cookies are enabled")
            } else {
                alert("Cookies are not enabled")
            }
        }
    </script>
</head>
<body>
    <p>弹出的提示框会告诉你浏览器是否已启用 cookie。</p>
</body>
</html>
```

---

### onchange 事件

onchange 事件常用于输入字段的验证。

下面的例子展示了如何使用 onchange。当用户改变输入字段的内容时，将调用 upperCase() 函数。

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function myFunction() {
            var x=document.getElementById("fname");
            x.value=x.value.toUpperCase();
        }
    </script>
</head>
<body>
    请输入你的英文名：<input type="text" id="fname" onchange="myFunction()" />
    <p>当你离开输入框时，被触发的函数会把你输入的文本转换为大写字母。</p>
</body>
</html>
```

---

### onmouseover 和 onmouseout 事件

onmouseover 和 onmouseout 事件可用于在鼠标指针移动到或离开元素时触发函数。

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function mOver(obj) {
            obj.innerHTML="谢谢你"
        }

        function mOut(obj) {
            obj.innerHTML="把鼠标指针移动到上面"
        }
    </script>
</head>
<body>
    <div onmouseover="mOver(this)" onmouseout="mOut(this)" style="background-color:#D94A38;width:200px;height:50px;padding-top:25px;text-align:center;"> Mouse Over Me
</div>
</body>
</html>
```

---

### onmousedown、onmouseup 以及 onclick 事件

onmousedown、onmouseup 以及 onclick 事件是鼠标点击的全部过程。首先当某个鼠标按钮被点击时，触发 onmousedown 事件，然后，当鼠标按钮被松开时，会触发 onmouseup 事件，最后，当鼠标点击完成时，触发 onclick 事件。

```
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
    <meta charset="utf-8">
    <script type="text/javascript">
	    function mDown(obj) {
	        obj.style.backgroundColor="#1ec5e5";
	        obj.innerHTML="松开鼠标"
	    }
	
	    function mUp(obj) {
	        obj.style.backgroundColor="#D94A38";
	        obj.innerHTML="谢谢你"
	    }
    </script>
</head>
<body>
    <div onmousedown="mDown(this)" onmouseup="mUp(this)" style="background-color:#D94A38;width:200px;height:50px;padding-top:25px;text-align:center;">点击这里
</div>
</body>
</html>
```

---
