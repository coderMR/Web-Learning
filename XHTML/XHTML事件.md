# XHTML 事件属性

---

HTML 4.0 的新特性之一是使 HTML 事件触发浏览器中的行为，比方说当用户点击一个 HTML 元素时启动一段 JavaScript 。以下就是可被插入 HTML 标签以定义事件行为的一系列属性。

---

### 窗口事件

仅在 body 和 frameset 元素中有效。

| 属性 | 值 | 描述
|------|----|-----
| onload | 脚本 | 当文档被载入时执行脚本
| onunload | 脚本 | 当文档被卸下时执行脚本

---

### 表单元素事件（Form Element Events）

仅在表单元素中有效

| 属性 | 值 | 描述
|------|----|-----
| onchange | 脚本 | 当元素改变时执行脚本
| onsubmit | 脚本 | 当表单被提交时执行脚本
| onreset | 脚本 | 当表单被重置时执行脚本
| onselect | 脚本 | 当元素被选取时执行脚本
| onblur | 脚本 | 当元素失去焦点时执行脚本
| onfocus | 脚本 | 当元素获得焦点时执行脚本

---

### 键盘事件（Keyboard Events）

在下列元素中无效：base、bdo、br、frame、frameset、head、html、iframe、meta、param、script、style、title。

| 属性 | 值 | 描述
|------|----|-----
| onkeydown | 脚本 | 当键盘被按下时执行脚本
| onkeypress | 脚本 | 当键盘被按下后又松开时执行脚本
| onkeyup | 脚本 | 当键盘被松开时执行脚本

---

### 鼠标事件（Mouse Events）

在下列元素中无效：base、bdo、br、frame、frameset、head、html、iframe、meta、param、script、style、title。

| 属性 | 值 | 描述
|------|----|-----
| onclick | 脚本 | 当鼠标被单击时执行脚本
| ondblclick | 脚本 | 当鼠标被双击时执行脚本
| onmousedown | 脚本 | 当鼠标按钮被按下时执行脚本
| onmousemove | 脚本 | 当鼠标指针移动时执行脚本
| onmouseout | 脚本 | 当鼠标指针移出某元素时执行脚本
| onmouseover | 脚本 | 当鼠标指针悬停与某元素之上时执行脚本
| onmouseup | 脚本 | 当鼠标按钮被松开时执行脚本

---
