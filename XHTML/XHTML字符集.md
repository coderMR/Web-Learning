# HTML 字符集

---

### HTML 字符集

如需正确的显示 HTML 页面，浏览器必须知道使用何种字符集。

万维网早期使用的字符集是 ASCII。ASCII 支持 0-9 的数字，大写和小写英文字母表，以及一些特殊字符。

由于很多国家的字符并不属于 ASCII，现代浏览器的默认字符集是 ISO-8859-1。

如果网页使用不同于 ISO-8859-1 的字符集，就应该在 &lt;meta&gt; 标签进行制定。

---

### ISO 字符集

ISO 字符集是国标标准组织（ISO）针对不同的字母表/语言定义的标准字符集。

下面列出了世界各地的使用的不同字符集。

<table class="dataintable">
<tr>
<th style="width:20%;">字符集</th>
<th style="width:30%;">描述</th>
<th>使用范围</th>
</tr>

<tr>
<td>ISO-8859-1</td>
<td>Latin alphabet part 1</td>
<td>北美、西欧、拉丁美洲、加勒比海、加拿大、非洲</td>
</tr>

<tr>
<td>ISO-8859-2</td>
<td>Latin alphabet part 2</td>
<td>东欧</td>
</tr>

<tr>
<td>ISO-8859-3</td>
<td>Latin alphabet part 3</td>
<td>SE Europe、世界语、其他杂项</td>
</tr>

<tr>
<td>ISO-8859-4</td>
<td>Latin alphabet part 4</td>
<td>斯堪的纳维亚/波罗的海（以及其他没有包括在 ISO-8859-1 中的部分）</td>
</tr>

<tr>
<td>ISO-8859-5</td>
<td>Latin/Cyrillic part 5</td>
<td>使用古代斯拉夫语字母表的语言，比如保加利亚语、白俄罗斯文、俄罗斯语、马其顿语</td>
</tr>

<tr>
<td>ISO-8859-6</td>
<td>Latin/Arabic part 6</td>
<td>使用阿拉伯字母的语言</td>
</tr>

<tr>
<td>ISO-8859-7</td>
<td>Latin/Greek part 7</td>
<td>现代希腊语，以及有希腊语衍生的数学符号</td>
</tr>

<tr>
<td>ISO-8859-8</td>
<td>Latin/Hebrew part 8</td>
<td>使用希伯来语的语言</td>
</tr>

<tr>
<td>ISO-8859-9</td>
<td>Latin 5 part 9</td>
<td>土耳其语</td>
</tr>

<tr>
<td>ISO-8859-10</td>
<td>Latin 6</td>
<td>拉普兰语、日耳曼语、爱斯基摩北欧语</td>
</tr>

<tr>
<td>ISO-8859-15</td>
<td>Latin 9 (aka Latin 0)</td>
<td>与 ISO 8859-1 类似，欧元符号和其他一些字符取代了一些较少使用的符号</td>
</tr>

<tr>
<td>ISO-2022-JP</td>
<td>Latin/Japanese part 1</td>
<td>日本语</td>
</tr>

<tr>
<td>ISO-2022-JP-2</td>
<td>Latin/Japanese part 2</td>
<td>日本语</td>
</tr>

<tr>
<td>ISO-2022-KR</td>
<td>Latin/Korean part 1</td>
<td>韩语</td>
</tr>
</table>

---

### Unicode 标准

由于上面列出的字符集都有容量限制，而且不兼容多语言环境，Unicode 联盟开发了 Unicode 标准。

Unicode 标准涵盖了世界上所有的字符、标点和符号。

不论是何种平台、程序或语言，Unicode 都能够进行文本数据的处理、存储和交互。

---

### Unicode 联盟

Unicode 联盟开发了 Unicode。他们的目标是用标准的 Unicode 转换格式（UTF）来取代现有的字符集。

Unicode 标准已经获得了成功，在 XML、Java、ECMAScript（JavaScript）、LDAP、CORBA 3.0、WML 中，Unicode 已经得到了实现。在许多操作系统以及所有的现代浏览器中，Unicode 同样得到了支持。

Unicode 联盟与领导性的标准发展组织进行合作，比如 ISO、W3C 以及 ECMA。

Unicode 可以被不同的字符集兼容。最常用的编码方式是 UTF-8 和 UTF-16：

### UTF-8

UTF-8 中的字符可以是 1-4 个字节长。UTF-8 可以表示 Unicode 标准中的任意字符。UTF-8 向后兼容 ASCII。UTF-8 是网页和电子邮件的首选编码。

### UTF-16

16 比特的 Unicode 转换格式是一种 Unicode 可变字符编码，能够对全部 Unicode 指令表进行编码。UTF-16 主要被用于操作系统和环境中，比如微软的 Windows 2000/XP/2003/Vista/CE 以及 Java 和 .NET 字节代码环境。

注释：最前面的 256 个 Unicode 字符集字符对应于 256 个 ISO-8859-1 字符。

注释：所有 HTML 4 处理器均已支持 UTF-8，而所有 XHTML 和 XML 处理器支持 UTF-8 和 UTF-16。

---
