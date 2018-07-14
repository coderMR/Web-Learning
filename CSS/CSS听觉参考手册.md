# CSS 听觉参考手册

---

### 听觉样式表

听觉样式表可把语音合成与音响效果相组合，使用户可以听到信息，而无需进行阅读。

听觉呈现可用于：

* 视觉能力低弱的人士
* 帮助用户学习阅读
* 帮助有阅读障碍的用户
* 家庭娱乐
* 在汽车中使用

听觉呈现通常会把文档转化为纯文本，然后传给屏幕阅读器（可读出屏幕上所有字符的一种程序）。

听觉样式表的一个例子：

```
h1, h2, h3, h4
{
    voice-family: male;
    richness: 80;
    cue-before: url("beep.au")
}
```

上面的例子可以让语音合成器演奏一段声音，然后用男性的声音读出标题。

### CSS2 听觉参考

W3C : "W3C" 列的数字显示出属性由哪个 CSS 标准定义（CSS1 还是 CSS2）。

<table class="dataintable">
<colgroup span="4">
<col class="no_wrap"  />
<col  />
<col class="no_wrap"  />
<col  />
</colgroup>
  <tr>
    <th>属性</th>
    <th>描述</th>
    <th>值</th>
    <th>W3C</th>
  </tr>
  <tr>
    <td>azimuth</td>
    <td>Sets where the sound/voices should come from (horizontally)</td>
    <td>
		<ul>
			<li class="table_value">angle</li>
			<li>left-side</li>
			<li>far-left</li>
			<li>left</li>
			<li>center-left</li>
			<li>center</li>
			<li>center-right</li>
			<li>right</li>
			<li>far-right</li>
			<li>right-side</li>
			<li>behind</li>
			<li>leftwards</li>
			<li>rightwards</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>cue</td>
    <td>A shorthand property for setting the cue-before and cue-after properties in one declaration</td>
    <td>
		<ul>
			<li class="table_value">cue-before</li>
			<li class="table_value">cue-after</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>cue-after</td>
    <td>Specifies a sound to be played after speaking an element's content to delimit it from other</td>
    <td>
		<ul>
			<li>none</li>
			<li class="table_value">url</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>cue-before</td>
    <td>Specifies a sound to be played before speaking an element's content to delimit it from other</td>
    <td>
		<ul>
			<li>none</li>
			<li class="table_value">url</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>elevation</td>
    <td>Sets where the sound/voices should come from (vertically)</td>
    <td>
		<ul>
			<li>angle</li>
			<li>below</li>
			<li>level</li>
			<li>above</li>
			<li>higher</li>
			<li>lower&nbsp;</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>pause</td>
    <td>A shorthand property for setting the pause-before and pause-after properties in one declaration</td>
    <td>
		<ul>
			<li class="table_value">pause-before</li>
			<li>pause-after</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>pause-after</td>
    <td>Specifies a pause after speaking an element's content</td>
    <td>
		<ul>
			<li class="table_value">time</li>
			<li>%</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>pause-before</td>
    <td>Specifies a pause before speaking an element's content</td>
    <td>
		<ul>
			<li class="table_value">time</li>
			<li>%</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>pitch</td>
    <td>Specifies the speaking voice</td>
    <td>
		<ul>
			<li class="table_value">frequency</li>
			<li>x-low</li>
			<li>low</li>
			<li>medium</li>
			<li>high</li>
			<li>x-high&nbsp;</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>pitch-range</td>
    <td>Specifies the variation in the speaking voice. (Monotone voice or animated voice?)</td>
    <td><ul><li class="table_value">number</li></ul></td>
    <td>2</td>
  </tr>
  <tr>
    <td>play-during</td>
    <td>Specifies a sound to be played while speaking an element's content</td>
    <td>
		<ul>
			<li>auto</li>
			<li>none</li>
			<li class="table_value">url</li>
			<li>mix</li>
			<li>repeat</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>richness</td>
    <td>Specifies the richness in the speaking voice. (Rich voice or thin voice?)</td>
    <td><ul><li class="table_value">number</li></ul></td>
    <td>2</td>
  </tr>
  <tr>
    <td>speak</td>
    <td>Specifies whether content will render aurally</td>
    <td>
	<ul>
	<li>normal</li>
    <li>none</li>
    <li>spell-out</li>
	</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>speak-header</td>
    <td>Specifies how to handle table headers. Should the headers be spoken before every cell, or only before a cell with a different header than the previous cell</td>
    <td>
		<ul>
			<li>always</li>
			<li>once</li>
		</ul>
    </td>
    <td>2</td>
  </tr>
  <tr>
    <td>speak-numeral</td>
    <td>Specifies how to speak numbers</td>
    <td>
	<ul>
	<li>digits</li>
    <li>continuous</li>
	</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>speak-punctuation</td>
    <td>Specifies how to speak punctuation characters</td>
    <td>
		<ul>
			<li>none</li>
			<li>code</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>speech-rate</td>
    <td>Specifies the speed of the speaking</td>
    <td>
		<ul>
			<li class="table_value">number</li>
			<li>x-slow</li>
			<li>slow</li>
			<li>medium</li>
			<li>fast</li>
			<li>x-fast</li>
			<li>faster</li>
			<li>slower&nbsp;</li>
		</ul>
	</td>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>stress</td>
    <td>Specifies the &quot;stress&quot; in the speaking voice</td>
    <td><ul><li class="table_value">number</li></ul></td>
    <td>2</td>
  </tr>
  <tr>
    <td>voice-family</td>
    <td>A prioritized list of voice family names that contain specific voices</td>
    <td>
		<ul>
			<li class="table_value">specific-voice</li>
			<li>generic-voice</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
  <tr>
    <td>volume</td>
    <td>Specifies the volume of the speaking</td>
    <td>
		<ul>
			<li class="table_value">number</li>
			<li class="table_value">%</li>
			<li>silent</li>
			<li>x-soft</li>
			<li>soft</li>
			<li>medium</li>
			<li>loud</li>
			<li>x-loud&nbsp;</li>
		</ul>
	</td>
    <td>2</td>
  </tr>
</table>

---
