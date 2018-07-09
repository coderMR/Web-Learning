# HTML 5 Video + DOM

---

### HTML 5 &lt;video&gt; - 使用 DOM 进行控制

HTML 5 &lt;video&gt; 元素同样拥有方法，属性，事件。

其中的方法用于播放、暂停、加载等。
其中的属性（比如时长、音量等）可以被读取或设置。
其中的 DOM 事件 能够通知您，比方说，&lt;video&gt; 元素开始播放、已暂停、已停止、等等。

下例中简单的方法，向我们展示了如何使用 &lt;video&gt; 元素，读取并设置属性，以及如何调用方法。

实例

为视频创建简单的播放/暂停以及调整尺寸控件：

```
<!DOCTYPE html>
<html>
<head>
    <title>
        video
    </title>
    <meta charset="utf-8">
    <script type="text/javascript">
        function get_dom(id) {
            return document.getElementById(id);
        }

        function changeState() {
            vi_d = get_dom('video1');
            if (vi_d.paused) { // 暂停状态
                vi_d.play();
            } else {
                vi_d.pause();
            }
        }

        function set_size(rate) {
            vi_d = get_dom('video1');
            vi_d.width = 320 * rate;
        }

        function set_large() {
            set_size(2);
        }

        function set_mid() {
            set_size(1);
        }

        function set_small() {
            set_size(0.5)
        }
    </script>
</head>
<body>
    <button type="button" onclick="changeState()">播放/暂停</button>
    <button type="button" onclick="set_large()">大</button>
    <button type="button" onclick="set_mid()">中</button>
    <button type="button" onclick="set_small()">小</button>
    <br /><br />
    <video controls="controls" id="video1" width="320"> 
        <source src="http://www.w3school.com.cn/example/html5/mov_bbb.ogg" type="video/ogg" />
        <source src="http://www.w3school.com.cn/example/html5/mov_bbb.mp4" type="video/mp4" />
    </video>
</body>
</html>
```

![video](img/video.gif)

---

### HTML5 &lt;video&gt; - 方法、属性、事件

下面列出了大多数浏览器支持的视频方法、属性、事件：

<table class="dataintable">
<tr>
<th style="width:33%;">方法</th>
<th style="width:33%;">属性</th>
<th>事件</th>
</tr>

<tr>
<td>play()</td>
<td>currentSrc</td>
<td>play</td>
</tr>

<tr>
<td>pause()</td>
<td>currentTime</td>
<td>pause</td>
</tr>

<tr>
<td>load()</td>
<td>videoWidth</td>
<td>progress</td>
</tr>

<tr>
<td>canPlayType</td>
<td>videoHeight</td>
<td>error</td>
</tr>

<tr>
<td>&nbsp;</td>
<td>duration</td>
<td>timeupdate</td>
</tr>

<tr>
<td>&nbsp;</td>
<td>ended</td>
<td>ended</td>
</tr>

<tr>
<td>&nbsp;</td>
<td>error</td>
<td>abort</td>
</tr>

<tr>
<td>&nbsp;</td>
<td>paused</td>
<td>empty</td>
</tr>

<tr>
<td>&nbsp;</td>
<td>muted</td>
<td>emptied</td>
</tr>

<tr>
<td>&nbsp;</td>
<td>seeking</td>
<td>waiting</td>
</tr>

<tr>
<td>&nbsp;</td>
<td>volume</td>
<td>loadedmetadata</td>
</tr>

<tr>
<td>&nbsp;</td>
<td>height</td>
<td>&nbsp;</td>
</tr>

<tr>
<td>&nbsp;</td>
<td>width</td>
<td>&nbsp;</td>
</tr>
</table>

注释：在所有属性中，只有 videoWidth 和 videoHeight 属性是立即可用的。在视频的元数据已加载后，其他属性才可用。

---
