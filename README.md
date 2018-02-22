# knock-knock
iframe 缺点
	1.阻塞onload（在主页面onload之前，iframe页面onload最后）
	2.不利于seo
	3.共享连接池，影响并行加载
	解决方法：动态添加iframe的src属性
浏览器多个标签通信
	websocket、sharedworker、localstorge
页面可见性（page visibility API）
	document.visibilityState 的检测值 visible hidden prerender unload
	监控visibilitychange
	`document.addEventListener("visibilitychange", function() {
		console.log(document.visibilityState);
	})`

可继承属性 font-size font-family color
css3新特性
	选择器 :not 
	border-radius
	text-shadow
	text-decoration
	transform
	flexbox:采用flex布局的元素，称为flex容器（flex container），所有子元素自动成为容器成员，称为flex项目
兼容
	获取属性getAttribute()
	chrome 中文界面将小于12px文本以12px显示，-webkit-text-size-adjust: none;
	L-V-H-A : a:link{} a:visited{} a:hover{} a:active{}
	初始化css样式，保证浏览器显示一致
BFC 
	独立的布局环境，BFC中的元素的布局不受外界的影响
	浮动和绝对定位的元素以及overflow不为visible的块级盒子	