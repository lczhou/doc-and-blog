Eclipse no console output
----

前段时间在leetcode上刷题，有时候需要调试，于是安装了Eclipse + CDT + MinGW。但是发现在Eclipse中直接执行程序，没有任何标准输出，但是单步调试输出就是正常的。

最后Google了一下，在[Eclipse官方论坛](http://www.eclipse.org/forums/index.php?t=msg&th=197552&start=0&S=2a2b64e1f1404705c0214976bd477428)找到了解决办法。原因是没有配置MinGW的环境变量。
或者也可以在Eclipse中配置。

	1 Goto Project->Properties->Run/Debug Settings, choose the .exe file and press "Edit"

	2 In the "Environment" tag, press "New", set it as: 
	"Name:PATH"
	"Value:C:\MinGW\bin"

	
	