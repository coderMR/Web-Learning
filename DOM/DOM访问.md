# HTML DOM 访问

---

访问 HTML DOM - 查找 HTML 元素。

---

### 访问 HTML 元素（节点）

访问 HTML 元素等同于访问节点

您能够以不同的方式来访问 HTML 元素：

* 通过使用 getElementById() 方法
* 通过使用 getElementsByTagName() 方法
* 通过使用 getElementsByClassName() 方法

---

### getElementById() 方法

getElementById() 方法返回带有指定 ID 的元素：

下面的例子获取 id="intro" 的元素：

```
document.getElementById("intro");
```

---

### getElementsByTagName() 方法

getElementsByTagName() 返回带有指定标签名的所有元素。

下面的例子返回包含文档中所有 &lt;p&gt; 元素的列表：

```
document.getElementsByTagName("p");
```

下面的例子返回包含文档中所有 &lt;p&gt; 元素的列表，并且这些 &lt;p&gt; 元素应该是 id="main" 的元素的后代（子、孙等等）：

```
document.getElementById("main").getElementsByTagName("p");
亲自试一试
```

---

### getElementsByClassName() 方法

如果您希望查找带有相同类名的所有 HTML 元素，请使用这个方法：

```
document.getElementsByClassName("intro");
```

上面的例子返回包含 class="intro" 的所有元素的一个列表：

注释：getElementsByClassName() 在 Internet Explorer 5,6,7,8 中无效。

---
