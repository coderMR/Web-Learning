# CSS 合法颜色值

---

### CSS 颜色

可以用以下方法来规定 CSS 中的颜色：

* 十六进制色
* RGB 颜色
* RGBA 颜色
* HSL 颜色
* HSLA 颜色
* 预定义/跨浏览器颜色名

---

### 十六进制颜色

所有浏览器都支持十六进制颜色值。

十六进制颜色是这样规定的：#RRGGBB，其中的 RR（红色）、GG（绿色）、BB（蓝色）十六进制整数规定了颜色的成分。所有值必须介于 0 与 FF 之间。

举例说，#0000ff 值显示为蓝色，这是因为蓝色成分被设置为最高值（ff），而其他成分被设置为 0。

```
p {
    background-color: #0000FF;
}
```

---

### RGB 颜色

所有浏览器都支持 RGB 颜色值。

RGB 颜色值是这样规定的：rgb(red, green, blue)。每个参数 (red、green 以及 blue) 定义颜色的强度，可以是介于 0 与 255 之间的整数，或者是百分比值（从 0% 到 100%）。

举例说，rgb(0,0,255) 值显示为蓝色，这是因为 blue 参数被设置为最高值（255），而其他被设置为 0。

同样地，下面的值定义了相同的颜色：rgb(0,0,255) 和 rgb(0%,0%,100%)。

```
p {
    background-color: rgb(255, 0, 0);
}
```

---

### RGBA 颜色

RGBA 颜色值得到以下浏览器的支持：IE9+、Firefox 3+、Chrome、Safari 以及 Opera 10+。

RGBA 颜色值是 RGB 颜色值的扩展，带有一个 alpha 通道 - 它规定了对象的不透明度。

RGBA 颜色值是这样规定的：rgba(red, green, blue, alpha)。alpha 参数是介于 0.0（完全透明）与 1.0（完全不透明）的数字。

```
p {
    background-color: rgba(25, 0, 0, 0.5);
}
```

### HSL 颜色

HSL 颜色值得到以下浏览器的支持：IE9+、Firefox、Chrome、Safari 以及 Opera 10+。

HSL 指的是 hue（色调）、saturation（饱和度）、lightness（亮度） - 表示颜色柱面坐标表示法。

HSL 颜色值是这样规定的：hsl(hue, saturation, lightness)。

Hue 是色盘上的度数（从 0 到 360） - 0 (或 360) 是红色，120 是绿色，240 是蓝色。Saturation 是百分比值；0% 意味着灰色，而 100% 是全彩。Lightness 同样是百分比值；0% 是黑色，100% 是白色。

```
p {
    background-color: hsl(120, 65%, 75%);
}
```

---

### HSLA 颜色

HSLA 颜色值得到以下浏览器的支持：IE9+、Firefox 3+、Chrome、Safari 以及 Opera 10+。

HSLA 颜色值是 HSL 颜色值的扩展，带有一个 alpha 通道 - 它规定了对象的不透明度。

HSLA 颜色值是这样规定的：hsla(hue, saturation, lightness, alpha)，其中的 alpha 参数定义不透明度。alpha 参数是介于 0.0（完全透明）与 1.0（完全不透明）的数字。

```
p {
    background-color: hsla(120, 65%, 75%, 0.3);
}
```

---
