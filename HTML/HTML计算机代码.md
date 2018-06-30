# HTML 计算机代码元素

---

### 计算机代码

```
var person = {
    firstName:'Bill',
    lastName:'Gates',
    age:50,
    eyeColor:'Blue'    
}
```

---

### HTML 计算机代码格式

通常，HTML 使用可变的字母尺寸，以及可变的字母间距。

在显示计算机代码时，并不需要如此。

&lt;kbd&gt;、&lt;samp&gt; 以及 &lt;code&gt; 元素全都支持固定的字母尺寸和间距。

---

### HTML 键盘格式

HTML &lt;kbd&gt; 元素定义键盘输入格式：

实例：

```
<p>to open a file, select:</p>
<p><kbd>file | open...</kbd><p>
```

---

### HTML 样本格式

HTML &lt;samp&gt; 元素定义计算机输出格式：

实例：

```
<samp>
demo.example.com login: Apr 12 09:10:17
Linux 2.6.10-grsec+gg3+e+fhs6b+nfs+gr0501+++p3+c4a+gr2b-reslog-v6.189
</samp>
```

---

### HTML 代码格式

HTML &lt;code&gt; 元素定义编程代码格式：

实例：

```
<code>
def main():
    print('program')
</code>
```

注释：&lt;code&gt; 元素不保留多余的空格和折行。

如需解决这一问题，必须在 &lt;pre&gt; 元素中包围代码。

实例：

```
<p>Example coding</p>
<code>
<pre>
# -*- coding=utf-8 -*-

def main():
    print('program')

if __name__ == '__main__':
    main()
</pre>
</code>
```

---

### HTML 变量格式化

HTML &lt;var&gt; 元素定义变量

实例：

```
<p><var>E = mc<sup>2</sup><var></p>
```

---

### HTML 计算机代码元素

| 标签 | 描述 
|------|------
| &lt;kbd&gt; | 定义输入文本
| &lt;samp&gt; | 定义输出文本
| &lt;var&gt; | 定义变量
| &lt;code&gt; | 定义代码
| &lt;pre&gt; | 定义预格式化代码

