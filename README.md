countStr
=
主要用于字符统计和限制字符长度的jq插件。

使用方法
-

假设你的网页已经引入了jq插件<br>
1.引入countStr.js

2.编写dom结构
从外层div开始寻找表单控件，和字数显示的标签
<div class="xx">
	<input type="text">
	<span></span>
</div>

3.使用countStr函数
<script><br>
>>('xx').countStr({length:'30',input:'input',zishu:'span'})<br>
</script><br>
length:要限制的字数，可以不写<br>
input:div下要检测的input<br>
zishu:用于显示的标签<br>
