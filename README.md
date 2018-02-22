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
