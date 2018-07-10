# HTML 参考手册

---

### HTML 5

通过制定如何处理所有 HTML 元素以及如何从错误中恢复的精确规则，HTML 5 改进了互操作性，并减少了开发成本。

HTML 5 中的新特性包括了嵌入音频、视频和图形的功能，客户端数据存储，以及交互式文档。

HTML 5 还包含了新的元素，比如：&lt;nav&gt;, &lt;header&gt;, &lt;footer&gt; 以及 &lt;figure&gt; 等等。

HTML 5 工作组包括：AOL, Apple, Google, IBM, Microsoft, Mozilla, Nokia, Opera, 以及数百个其他的供应商。

注释：HTML 5 还没有成为 W3C 正式的推荐标准。

---

### 按功能类别排列

### 基础

| 标签 | 描述
|------|-----
| [&lt;!DOCTYPE&gt;]() | 定义文档类型
| [&lt;html&gt;]() | 定义 HTML 文档
| [&lt;title&gt;]() | 定义文档的标题
| [&lt;body&gt;]() | 定义文档的主体
| [&lt;h1&gt; to &lt;h6&gt;]() | 定义 HTML 标题
| [&lt;p&gt;]() | 定义段落
| [&lt;br&gt;]() | 定义简单的折行
| [&lt;hr&gt;]() | 定义水平线
| [&lt;!--...--&gt;]() | 定义注释

### 格式

| 标签 | 描述
|------|-----
| [&lt;acronym&gt;]() | 定义只取首字母的缩写
| [&lt;abbr&gt;]() | 定义缩写
| [&lt;address&gt;]() | 定义文档作者或拥有者的联系信息
| [&lt;b&gt;]() | 定义粗体文本
| [&lt;bdi&gt;]() ![h5](img/h5.png) | 定义文本的文本方向，使其脱离其周围文本的方向设置
| [&lt;bdo&gt;]() | 定义文字方向
| [&lt;big&gt;]() | 定义大号文本
| [&lt;blockquote&gt;]() | 定义长的引用
| [&lt;center&gt;]() | 不赞成使用。定义居中文本
| [&lt;cite&gt;]() | 定义引用
| [&lt;code&gt;]() | 定义计算机代码文本
| [&lt;del&gt;]() | 定义被删除文本
| [&lt;dfn&gt;]() | 定义定义项目
| [&lt;em&gt;]() | 定义强调文本
| [&lt;font&gt;]() | 不赞成使用。定义文本的字体、尺寸和颜色
| [&lt;i&gt;]() | 定义斜体文本
| [&lt;ins&gt;]() | 定义被插入文本
| [&lt;kbd&gt;]() | 定义键盘文本
| [&lt;mark&gt;]() ![h5](img/h5.png) | 定义有记号的文本
| [&lt;meter&gt;]() ![h5](img/h5.png) | 定义预定义范围内的度量
| [&lt;pre&gt;]() | 定义预格式文本
| [&lt;progress&gt;]() ![h5](img/h5.png) | 定义任何类型的任务的进度
| [&lt;q&gt;]() | 定义短的引用
| [&lt;rp&gt;]() ![h5](img/h5.png) | 定义若浏览器不支持 ruby 元素显示的内容
| [&lt;rt&gt;]() ![h5](img/h5.png) | 定义 ruby 注释的解释
| [&lt;s&gt;]() | 不赞成使用。定义加删除线的文本
| [&lt;samp&gt;]() | 定义计算机代码样本
| [&lt;small&gt;]() | 定义小号文本
| [&lt;strike&gt;]() | 不赞成使用。定义加删除线文本
| [&lt;strong&gt;]() | 定义语气更为强烈的强调稳步
| [&lt;sup&gt;]() | 定义上标文本
| [&lt;sub&gt;]() | 定义下标文本
| [&lt;time&gt;]() ![h5](img/h5.png) | 定义日期/时间
| [&lt;tt&gt;]() | 定义打字机文本
| [&lt;u&gt;]() | 不赞成使用。定义下标线文本
| [&lt;var&gt;]() | 定义文本的变量部分
| [&lt;wbr&gt;]() ![h5](img/h5.png) | 定义可能的换行符

### 表单

| 标签 | 描述
|------|-----
| [&lt;form&gt;]() | 定义供用户输入的 HTML 表单
| [&lt;input&gt;]() | 定义输入控件
| [&lt;textarea&gt;]() | 定义多行的文本输入控件
| [&lt;button&gt;]() | 定义按钮
| [&lt;select&gt;]() | 定义选择列表（下拉列表）
| [&lt;optgroup&gt;]() | 定义选择列表中相关选项的组合
| [&lt;label&gt;]() | 定义 input 元素的标注
| [&lt;fieldset&gt;]() | 定义围绕表单中元素的边框
| [&lt;legend&gt;]() | 定义 fieldset 元素的标题
| [&lt;isindex&gt;]() | 不赞成使用。定义与文档相关的可搜索索引。
| [&lt;datalist&gt;]() ![h5](img/h5.png) | 定义下拉列表
| [&lt;keygen&gt;]() ![h5](img/h5.png) | 定义生成密钥
| [&lt;output&gt;]() ![h5](img/h5.png)| 定义输出的一些类型
 
### 框架

| 标签 | 描述
|------|-----
| [&lt;frame&gt;]() | 定义框架集的窗口或框架
| [&lt;frameset&gt;]() | 定义框架集
| [&lt;noframes&gt;]() | 定义针对不支持框架的用户的替代内容
| [&lt;iframe&gt;]() | 定义内联框架

### 图像

| 标签 | 描述
|------|-----
| [&lt;img&gt;]() | 定义图像
| [&lt;map&gt;]() | 定义图像映射
| [&lt;area&gt;]() | 定义图像内部的区域
| [&lt;canvas&gt;]() ![h5](img/h5.png) | 定义图形
| [&lt;figcaption&gt;]() ![h5](img/h5.png) | 定义 figure 元素的标题
| [&lt;figure&gt;]() ![h5](img/h5.png) | 定义媒介内容的分组，以及它们的标题

# 音频/视频

| 标签 | 描述
|------|-----
| [&lt;audio&gt;]() ![h5](img/h5.png) | 定义声音内容
| [&lt;source&gt;]() ![h5](img/h5.png) | 定义媒介源
| [&lt;track&gt;]() ![h5](img/h5.png) | 定义用在媒体播放器中的文本轨道
| [&lt;video&gt;]() ![h5](img/h5.png) | 定义视频

### 链接

| 标签 | 描述
|------|-----
| [&lt;a&gt;]() | 定义锚
| [&lt;link&gt;]() | 定义文档与外部资源的关系
| [&lt;nav&gt;]() ![h5](img/h5.png) | 定义导航链接

### 列表

| 标签 | 描述
|------|-----
| [&lt;ul&gt;]() | 定义无序列表
| [&lt;ol&gt;]() | 定义有序列表
| [&lt;li&gt;]() | 定义列表的项目
| [&lt;dir&gt;]() | 不赞成使用。定义目录列表
| [&lt;dl&gt;]() | 定义定义列表
| [&lt;dt&gt;]() | 定义定义列表中的项目
| [&lt;dd&gt;]() | 定义定义列表中项目的描述
| [&lt;menu&gt;]() | 定义命令的菜单/列表
| [&lt;menuitem&gt;]() | 定义用户可以从弹出菜单调用的命令/菜单项目
| [&lt;command&gt;]() ![h5](img/h5.png) | 定义命令按钮

### 表格

| 标签 | 描述
|------|-----
| [&lt;table&gt;]() | 定义表格
| [&lt;caption&gt;]() | 定义表格标题
| [&lt;th&gt;]() | 定义表格中表头单元格
| [&lt;tr&gt;]() | 定义表格中的行
| [&lt;td&gt;]() | 定义表格中的单元
| [&lt;thead&gt;]() | 定义表格中的表头内容
| [&lt;tbody&gt;]() | 定义表格中的主体内容
| [&lt;tfoot&gt;]() | 定义表格中的表注内容（脚注）
| [&lt;col&gt;]() | 定义表格中一个或多个列的属性值
| [&lt;colgroup&gt;]() | 定义表格中供格式化的列组

### 样式/节

| 标签 | 描述
|------|-----
| [&lt;style&gt;]() | 定义文档的样式信息
| [&lt;div&gt;]() | 定义文档中的节
| [&lt;span&gt;]() | 定义文档中的节
| [&lt;header&gt;]() ![h5](img/h5.png) | 定义 section 或 page 的页眉
| [&lt;footer&gt;]() ![h5](img/h5.png) | 定义 section 或 page 的页脚
| [&lt;section&gt;]() ![h5](img/h5.png) | 定义 section
| [&lt;article&gt;]() ![h5](img/h5.png) | 定义文章
| [&lt;aside&gt;]() ![h5](img/h5.png) | 定义页面内容之外的内容
| [&lt;details&gt;]() ![h5](img/h5.png) | 定义元素细节
| [&lt;dialog&gt;]() ![h5](img/h5.png) | 定义对话框或窗口
| [&lt;summary&gt;]() ![h5](img/h5.png) | 为 &lt; details&gt; 元素定义可见的标题

### 元信息

| 标签 | 描述
|------|-----
| [&lt;head&gt;]() | 定义关于文档的信息
| [&lt;meta&gt;]() | 定义关于 HTML 文档的元信息
| [&lt;base&gt;]() | 定义页面中所有链接的默认地址或默认目标
| [&lt;basefont&gt;]() | 不赞成使用。定义页面中文本的默认字体、颜色或尺寸
 
### 编程

| 标签 | 描述
|------|-----
| [&lt;script&gt;]() | 定义客户端脚本
| [&lt;noscript&gt;]() | 定义针对不支持客户端脚本的用户的替代内容
| [&lt;applet&gt;]() | 不赞成使用。定义嵌入的 applet
| [&lt;embed&gt;]() ![h5](img/h5.png) | 为外部应用程序定义容器
| [&lt;object&gt;]() | 定义嵌入的对象
| [&lt;param&gt;]() | 定义对象的参数

---
