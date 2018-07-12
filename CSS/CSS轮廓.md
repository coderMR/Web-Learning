# CSS 轮廓

---

### 轮廓（outline）是绘制于元素周围的一条线，位于边框边缘的外围，可起到突出元素的作用。

### CSS outline 属性规定元素轮廓的样式、颜色和宽度。

---

本例演示使用 outline 属性在元素周围画一条线：

```
p {
    border:red solid thin;
    outline:#00ff00 dotted thick;
}
```

设置轮廓的颜色

```
p {
    border:red solid thin;
    outline-style:dotted;
    outline-color:#00ff00;
}
```

设置轮廓的样式

```
p.dotted {outline-style: dotted}
p.dashed {outline-style: dashed}
p.solid {outline-style: solid}
p.double {outline-style: double}
p.groove {outline-style: groove}
p.ridge {outline-style: ridge}
p.inset {outline-style: inset}
p.outset {outline-style: outset}
```

设置轮廓宽度

```
p.one {
    border:red solid thin;
    outline-style:solid;
    outline-width:thin;
}

p.two {
    border:red solid thin;
    outline-style:dotted;
    outline-width:3px;
}
```

---

### CSS 边框属性

CSS 列中的数字指示哪个 CSS 版本定义了该属性

| 属性 | 描述 | CSS
|------|------|-----
| outline | 在一个声明中设置所有的轮廓属性 | 2
| outline-color | 设置轮廓的颜色 | 2
| outline-style | 设置轮廓的样式 | 2
| outline-width | 设置轮廓的宽度 | 2

---
