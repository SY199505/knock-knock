# knock-knock
iframe 缺点
	1.阻塞onload（在主页面onload之前，iframe页面onload最后）
	2.不利于seo
	3.共享连接池，影响并行加载
	解决方法：动态添加iframe的src属性
浏览器多个标签通信
	websocket、sharedworker、localstorge