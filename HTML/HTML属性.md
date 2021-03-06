# HTML 属性

---

### 属性为 HTML 元素提供附加信息。

---

### HTML 属性

HTML 标签可以拥有属性。属性提供了有关 HTML 元素的更多信息。

属性总是以 名称/值 对的形式出现，比如：name="value"。

属性总是在 HTML 元素的开始标签中规定。

---

### 属性实例

HTML 链接由 &lt;a&gt; 标签定义。链接的地址在 href 属性中指定：

```
<a href="https://www.baidu.com">百度</a>
```

---

### 更多 HTML 属性实例

属性例子1：

&lt;h1&gt; 定义标题的开始

&lt;h1 align="center"&gt; 拥有关于对齐方式的附加信息。

属性例子2：

&lt;body&gt; 定义 HTML 文档的主体。

&lt;body bgcolor="yellow"&gt; 拥有关于背景颜色的附加信息。

属性例子3：

&lt;table&gt; 定义了 HTML 表格。

&lt;table border="1px"&gt; 拥有关于表格边框的附加信息。

---

### HTML 提示：使用小写属性

属性和属性值对大小写不敏感。

不过，万维网联盟在其 HTML 4 推荐标准中推荐小写的属性/属性值。

而新版本的 (X)HTML 要求使用小写属性。

---

### 始终为属性值加引号

属性值应始终被包括在引号内。双引号是最常见的，不过使用单引号也没有问题。

在某些情况下，比如属性值本身就包含双引号，那么您必须使用单引号。

```
name='Bill "Hello World" Gates'
```


