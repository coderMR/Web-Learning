# HTML Server-Sent 事件

---

### Server-Sent 事件允许网页从服务器获得更新。

---

### Server-Sent 事件 - One Way Messaging

Server-Sent 事件指的是网页自动从服务器获得更新。

以前也可能做到这一点，前提是网页不得不询问是否有可用的更新。通过 Server-Sent 事件，更新能够自动到达。

例如：Facebook/Twitter 更新、股价更新、新的博文、赛事结果等等。

---

### 接收 Server-Sent 事件通知

EventSource 对象用于接收服务器发送事件通知：

```
var soruce = new EventSource("demo_sse.php");
source.onmessage = function(event) {
    document.getElementById("result").innerHTML = event.data + "<br />";
};
```

### 例子解释：

* 创建一个新的 EventSource 对象，然后规定发送更新的页面的 URL （本例中是 "demo_sse.php"）
* 每当接收一个更新，就会发生 onmessage 事件
* 当 onmessage 事件发生时，把已接收的数据推入 id 为 result 的元素中

---

### 检测 Server-Sent 事件支持

我们编写了一段额外的代码来检测服务器发送事件的浏览器支持：

```
if (typeof(EventSource) !== "undefined") {
    // 支持服务器发送事件
    // 代码
} else {
    // 抱歉！不支持服务器发送事件！
}
```

---

### EventSource 对象

在上例中，我们使用 onmessage 事件来获取消息。不过还可以使用其他事件：

| 事件 | 描述
|------|-----
| onopen | 当通往服务器的链接被打开
| onmessage | 当接收到消息
| onerror | 当发生错误

---
