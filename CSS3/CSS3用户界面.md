# CSS3 用户界面

---

### CSS3 用户界面

在 CSS3 中，新的用户界面特性包括重设元素尺寸、盒尺以及轮廓等。

在本节中，将介绍以下用户界面属性：

* resize
* box-sizing
* outline-offset

---

Firefox、Chrome 以及 Safari 支持 resize 属性。

Internet Explorer、Chrome、Safari 以及 Opera 支持 box-sizing 属性。Firefox 需要前缀 -moz-。

所有主流浏览器都支持 outline-offset 属性，除了 Internet Explorer。

---

### CSS3 Resizing

在 CSS3，resize 属性规定是否可由用户调整元素尺寸。

```
<!DOCTYPE html>
<html>
<head>
<style> 
div
{
border:2px solid;
padding:10px 40px; 
width:300px;
resize:both;
overflow:auto;
}
</style>
</head>
<body>

<div>resize 属性规定是否可由用户调整元素尺寸。</div>

<p><b>注释：</b> Firefox 4+、Safari 以及 Chrome 支持 resize 属性。</p>

</body>
</html>
```

### CSS3 Box Sizing

box-sizing 属性允许您以确切的方式定义适应某个区域的具体内容。

```
<!DOCTYPE html>
<html>
<head>
<style> 
div.container
{
width:30em;
border:1em solid;
}
div.box
{
box-sizing:border-box;
-moz-box-sizing:border-box; /* Firefox */
-webkit-box-sizing:border-box; /* Safari */
width:50%;
border:1em solid red;
float:left;
}
</style>
</head>
<body>

<div class="container">
<div class="box">这个 div 占据左半部分。</div>
<div class="box">这个 div 占据右半部分。</div>
</div>

</body>
</html>
```

---

### CSS3 Outline Offset

outline-offset 属性对轮廓进行偏移，并在超出边框边缘的位置绘制轮廓。

轮廓与边框有两点不同：

* 轮廓不占用空间
* 轮廓可能是非矩形

```
<!DOCTYPE html>
<html>
<head>
<style>
div
{
margin:20px;
width:150px;
padding:10px;
height:70px;
border:2px solid black;
outline:2px solid red;
outline-offset:15px;
}
</style>
</head>
<body>

<p><b>注释：</b>Internet Explorer 和 Opera 不支持 support outline-offset 属性。</p>

<div>这个 div 在边框边缘之外 15 像素处有一个轮廓。</div>

</body>
</html>
```

---
