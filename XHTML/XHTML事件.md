# HTML 事件属性

---

### 全局事件属性

HTML 4 增加了使事件在浏览器中触发动作的能力，比如当用户点击元素时启动 JavaScript。

下面列出了添加到 HTML 元素以定义事件动作的全局事件属性。

---

### Windows 事件属性

针对 window 对象触发的事件（应用到 &lt;body&gt; 标签）：

| 属性 | 值 | 描述
|------|----|-----
| [&lt;onafterprint&gt;]() ![h5](img/h5.png) | script | 文档打印之后运行的脚本
| [&lt;onbeforeprint&gt;]() ![h5](img/h5.png) | script | 文档打印之前运行的脚本
| [&lt;onbeforeunload&gt;]() ![h5](img/h5.png) | script | 文档卸载之前运行的脚本
| [&lt;onerror&gt;]() ![h5](img/h5.png) | script | 在错误发生时运行的脚本
| [&lt;onhaschange&gt;]() ![h5](img/h5.png) | script | 当文档已改变时运行的脚本
| [&lt;onload&gt;]() | script | 页面结束加载之后触发
| [&lt;onmessage&gt;]() ![h5](img/h5.png) | script | 在消息被触发时运行的脚本
| [&lt;onoffline&gt;]() ![h5](img/h5.png) | script | 当文档离线时运行的脚本
| [&lt;ononline&gt;]() ![h5](img/h5.png) | script | 当文档上线时运行的脚本
| [&lt;onpagehide&gt;]() ![h5](img/h5.png) | script | 当窗口隐藏时运行的脚本
| [&lt;onpageshow&gt;]() ![h5](img/h5.png) | script | 当窗口成为可见时运行的脚本
| [&lt;onpopstate&gt;]() ![h5](img/h5.png) | script | 当窗口历史记录改变时运行的脚本
| [&lt;onredo&gt;]() ![h5](img/h5.png) | script | 当文档执行撤销（redo）时运行的脚本
| [&lt;onresize&gt;]() ![h5](img/h5.png) | script | 当浏览器窗口被调整大小时触发
| [&lt;onstorage&gt;]() ![h5](img/h5.png) | script | 在 Web Storage 区域更新后运行脚本
| [&lt;onundo&gt;]() ![h5](img/h5.png) | script | 在文档执行 undo 时运行的脚本
| [&lt;onunload&gt;]() | script | 一旦页面已下载时触发（或者浏览器窗口已被关闭）

### Form 事件

由 HTML 表单内的动作触发的事件（应用到几乎所有 HTML 元素，但最常用在 form 元素中）：

| 属性 | 值 | 描述
|------|----|-----
| [&lt;onblur&gt;]() | script | 元素时区焦点时运行的脚本
| [&lt;onchange&gt;]() | script | 在元素值被改变时运行的脚本
| [&lt;oncontextmenu&gt;]() ![h5](img/h5.png) | script | 当上下文菜单被触发时运行的脚本
| [&lt;onfocus&gt;]() | script | 当元素获得焦点时运行的脚本
| [&lt;onforminput&gt;]() ![h5](img/h5.png) | script | 在表单改变时运行的脚本
| [&lt;onforminput&gt;]() ![h5](img/h5.png) | script | 当表单获得用户输入时运行的脚本
| [&lt;oninput&gt;]() ![h5](img/h5.png) | script | 当元素获得用户输入时运行的脚本
| [&lt;oninvalid&gt;]() ![h5](img/h5.png) | script | 当元素无效时运行的脚本
| [&lt;onreset&gt;]() | script | 当表单中的重置按钮被点击时触发。 HTML5 中不支持
| [&lt;onselect&gt;]() | script | 在元素中文本被选中后触发
| [&lt;onsubmit&gt;]() | script | 在元素中文本被选中后触发

# Keyboard 事件

| 属性 | 值 | 描述
|------|----|-----
| [&lt;onkeydown&gt;]() | script | 在用户按下按键时触发
| [&lt;onkeypress&gt;]() | script | 在用户敲击按钮时触发
| [&lt;onkeyup&gt;]() | script | 当用户释放按键时触发

### Mouse 事件

| 属性 | 值 | 描述
|------|----|-----
| [&lt;onclick&gt;]() | script | 元素上发生鼠标点击时触发
| [&lt;ondblclick&gt;]() | script | 元素上发生鼠标双击时触发
| [&lt;ondrag&gt;]() ![h5](img/h5.png) | script | 元素被拖动时运行的脚本
| [&lt;ondragend&gt;]() ![h5](img/h5.png) | script | 在拖动操作末端运行的脚本
| [&lt;ondragenter&gt;]() ![h5](img/h5.png) | script | 当元素已被拖动到有效拖放区时运行的脚本
| [&lt;ondragleave&gt;]() ![h5](img/h5.png) | script | 当元素离开有效拖放目标时运行的脚本
| [&lt;ondragover&gt;]() ![h5](img/h5.png) | script | 当元素在有效拖放目标上正在被拖放时运行的脚本
| [&lt;ondragstart&gt;]() ![h5](img/h5.png) | script | 在拖动操作开端运行的脚本
| [&lt;onmousedown&gt;]() | script | 当元素上按下鼠标按钮时触发
| [&lt;onmousemove&gt;]() | script | 当鼠标指针移动到元素上时触发
| [&lt;onmouseout&gt;]() | script | 当鼠标指针移出元素时触发
| [&lt;onmouseover&gt;]() | script | 当鼠标指针移动到元素上时触发
| [&lt;onmouseup&gt;]() | script | 当在元素上释放鼠标按钮时触发
| [&lt;onmousewheel&gt;]() ![h5](img/h5.png) | script | 当鼠标滚轮正在被滚动时运行的脚本
| [&lt;onscroll&gt;]() ![h5](img/h5.png) | script | 当元素滚动条被滚动时运行的脚本

### Media 事件

由媒介（比如视频、图像和音频）触发的事件（适用于所有 HTML 元素，但常见于媒介元素中，比如 &lt;audio&gt;、&lt;embed&gt;、&lt;img&gt;、&lt;object&gt; 以及 &lt;video&gt;）：

| 属性 | 值 | 描述
|------|----|-----
| [&lt;onabort&gt;]() | script | 在退出时运行的脚本
| [&lt;oncanplay&gt;]() ![h5](img/h5.png) | script | 当问及就绪可以开始播放时运行的脚本（缓冲已足够开始）
| [&lt;oncanplaythrough&gt;]() ![h5](img/h5.png) | script | 当媒介用过无需因缓冲而停止即可播放至结尾时运行的脚本
| [&lt;ondurationchange&gt;]() ![h5](img/h5.png) | script | 当媒介长度改变时运行的脚本
| [&lt;onemptied&gt;]() ![h5](img/h5.png) | script | 当发生故障并且文件突然不可用时运行的脚本（比如连接意外断开时）
| [&lt;onended&gt;]() ![h5](img/h5.png) | script | 当媒介已叨叨结尾时运行的脚本（可发送类似"感谢观看"之类的信息）
| [&lt;onerror&gt;]() ![h5](img/h5.png) | script | 当在文件加载期间发生错误时运行的脚本
| [&lt;onloadeddata&gt;]() ![h5](img/h5.png) | script | 当媒介数据已加载时运行的脚本
| [&lt;onloadedmetadata&gt;]() ![h5](img/h5.png) | script | 当元数据（比如分辨率和时长）被加载时运行的脚本
| [&lt;onloadstart&gt;]() ![h5](img/h5.png) | script | 在文件开始加载且未实际加载任何前运行的脚本
| [&lt;onpause&gt;]() ![h5](img/h5.png) | script | 当媒介被用户或程序暂停时运行的脚本
| [&lt;onplay&gt;]() ![h5](img/h5.png) | script | 当媒介已就绪可以开始播放时运行的脚本
| [&lt;onplaying&gt;]() ![h5](img/h5.png) | script | 当浏览器正在获取媒介数据时运行的脚本
| [&lt;onprogress&gt;]() ![h5](img/h5.png) | script | 当浏览器正在获取媒介数据时运行的脚本
| [&lt;onratechange&gt;]() ![h5](img/h5.png) | script | 每当回放速率改变时运行的脚本（比如当用户切换到慢动作或快进模式）
| [&lt;onreadystatechange&gt;]() ![h5](img/h5.png) | script | 每当就绪状态时运行的脚本（就绪状态监测媒介数据的状态）
| [&lt;onseeked&gt;]() ![h5](img/h5.png) | script | 每当 seeking 属性设置为 false （指示定位已结束）时运行的脚本
| [&lt;onseeking&gt;]() ![h5](img/h5.png) | script | 每当 seeking 属性设置为 true （指示定位是活动的）时运行的脚本
| [&lt;onstalled&gt;]() ![h5](img/h5.png) | script | 在浏览器不论何种原因未能取回媒介数据时运行的脚本
| [&lt;onsuspend&gt;]() ![h5](img/h5.png) | script | 在媒介数据完全加载之前不论何种原因终止取回媒介数据时运行的脚本
| [&lt;ontimeupdate&gt;]() ![h5](img/h5.png) | script | 当播放器位置改变时（比如当用户快进到媒介中一个不同的位置时）运行的脚本
| [&lt;onvolumechange&gt;]() ![h5](img/h5.png) | script | 每当音量改变时（包括将音量设置为静音）时运行的脚本
| [&lt;onwaiting&gt;]() | script | 当媒介已停止播放但打算继续播放时（比如当媒介暂停已缓冲更多数据）运行的脚本

---


