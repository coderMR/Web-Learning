# HTML 脚本

---

### JavaScript 使 HTML 具有更强的动态和交互性

---

### HTML script 元素

&lt;script&gt; 标签用于定义客户端脚本，比如 Javascript。

script 元素即可包含脚本语句，也可通过 src 属性指向外部脚本。

必需的 type 属性规定脚本的 MIME 类型。

Javascript 最常用于图片操作、表单验证以及内容动态更新。

下面的脚本向浏览器输出 Hello World。

```
<script>
    document.write('Hello World')
</srcipt>
```

---

### &lt;noscript&gt; 标签

&lt;noscript&gt; 标签提供了无法使用脚本时的替代内容。

noscript 元素可包含普通 HTML 页面的 body 元素中能够找到的所有元素。

只有在浏览器不支持脚本或者禁用脚本时，才会显示 noscript 元素中的内容。

```
<script>
    document.write('Hello World')
</srcipt>
<noscript>
    your browser dose not support Javascript
</noscript>
```

---

### 如何应付老式的浏览器

如果浏览器压根没有办法识别 &lt;script&gt; 标签，那么 &lt;script&gt; 标签所包含的内容将以文本方式显示在页面上，为了避免这种情况方式，应该将脚本隐藏在注释标签当中。那些老式的浏览器，将忽略这些注释，所以不会将脚本内容显示到页面上。而新的浏览器将读懂这些脚本并执行它们，即使代码被嵌套在注释标签内。

```
<script type="text/javascript">
<!--
document.write("Hello World!")
//-->
</script>
```

---
