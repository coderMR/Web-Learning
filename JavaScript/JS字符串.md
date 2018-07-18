# JavaScript 字符串(String)对象

---

### String 对象用于处理已有的字符块。

---

### 创建 String 对象的语法：

```
new String(s);
String(s);
```

参数：参数 s 是要存储在 String 对象中或转换成原始字符串的值。

当 String() 和运算符 new 一起作为构造函数使用时，它返回一个新创建的 String 对象，存放的是字符串 s 或 s 的字符串表示。

当不用 new 运算符调用 String() 时，它只把 s 转换成原始的字符串，并返回转换后的值。

---

### String 对象属性

| 属性 | 描述
| constructor | 对创建该对象的函数的引用
| length | 字符串的长度
| prototype | 允许您向对象添加属性和方法

---

### String 对象方法

<table class="dataintable">
  <tr>
    <th style="width:30%">方法</th>
    <th>描述</th>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_anchor.asp">anchor()</a></td>
    <td>创建 HTML 锚。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_big.asp">big()</a></td>
    <td>用大号字体显示字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_blink.asp">blink()</a></td>
    <td>显示闪动字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_bold.asp">bold()</a></td>
    <td>使用粗体显示字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_charAt.asp">charAt()</a></td>
    <td>返回在指定位置的字符。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_charCodeAt.asp">charCodeAt()</a></td>
    <td>返回在指定的位置的字符的 Unicode 编码。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_concat_string.asp">concat()</a></td>
    <td>连接字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_fixed.asp">fixed()</a></td>
    <td>以打字机文本显示字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_fontcolor.asp">fontcolor()</a></td>
    <td>使用指定的颜色来显示字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_fontsize.asp">fontsize()</a></td>
    <td>使用指定的尺寸来显示字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_fromCharCode.asp">fromCharCode()</a></td>
    <td>从字符编码创建一个字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_indexOf.asp">indexOf()</a></td>
    <td>检索字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_italics.asp">italics()</a></td>
    <td>使用斜体显示字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_lastIndexOf.asp">lastIndexOf()</a></td>
    <td>从后向前搜索字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_link.asp">link()</a></td>
    <td>将字符串显示为链接。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_localeCompare.asp">localeCompare()</a></td>
    <td>用本地特定的顺序来比较两个字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_match.asp">match()</a></td>
    <td>找到一个或多个正则表达式的匹配。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_replace.asp">replace()</a></td>
    <td>替换与正则表达式匹配的子串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_search.asp">search()</a></td>
    <td>检索与正则表达式相匹配的值。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_slice_string.asp">slice()</a></td>
    <td>提取字符串的片断，并在新的字符串中返回被提取的部分。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_small.asp">small()</a></td>
    <td>使用小字号来显示字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_split.asp">split()</a></td>
    <td>把字符串分割为字符串数组。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_strike.asp">strike()</a></td>
    <td>使用删除线来显示字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_sub.asp">sub()</a></td>
    <td>把字符串显示为下标。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_substr.asp">substr()</a></td>
    <td>从起始索引号提取字符串中指定数目的字符。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_substring.asp">substring()</a></td>
    <td>提取字符串中两个指定的索引号之间的字符。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_sup.asp">sup()</a></td>
    <td>把字符串显示为上标。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_toLocaleLowerCase.asp">toLocaleLowerCase()</a></td>
    <td>把字符串转换为小写。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_toLocaleUpperCase.asp">toLocaleUpperCase()</a></td>
    <td>把字符串转换为大写。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_toLowerCase.asp">toLowerCase()</a></td>
    <td>把字符串转换为小写。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_toUpperCase.asp">toUpperCase()</a></td>
    <td>把字符串转换为大写。</td>
  </tr>
  <tr>
    <td>toSource()</td>
    <td>代表对象的源代码。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_toString_string.asp">toString()</a></td>
    <td>返回字符串。</td>
  </tr>
  <tr>
    <td><a href="/jsref/jsref_valueOf_string.asp">valueOf()</a></td>
    <td>返回某个字符串对象的原始值。</td>
  </tr>
  </table>
```

---
