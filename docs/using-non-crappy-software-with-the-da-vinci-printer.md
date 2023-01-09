# 在达芬奇打印机上使用非垃圾软件

> 原文：<https://hackaday.com/2014/04/17/using-non-crappy-software-with-the-da-vinci-printer/>

XYZprinting 的达芬奇打印机被证明是世界上最便宜的消费打印机之一。当然，它使用芯片灯丝，但对于任何知道. hex 文件是什么的人来说，这是一个简单的修复方法。是的，达芬奇主机软件是一堆功能有限的专有垃圾，但是[马克]已经找到了一个绕过的方法。

当[马克]收到他的达芬奇时，他立即开始窥探打印机的内部，就像任何一个好的修理工应该做的那样。他找到了一个 SD 卡，里面保存了打印机附带的所有样本，都是方便的 Gcode 格式。在这些样本里。STL 文件是你所期望的所有调用——设置温度，改变图层高度，以及你在任何其他 RepRap 中找到的所有其他好东西。

稍微修改一下。由任何切片程序生成的 STL 文件，[Mark]不再受达芬奇附带的可怕的主机软件的限制。再加上[重置灯丝盒内芯片的能力](http://hackaday.com/2014/04/10/resetting-drm-on-3d-printer-filament/)，【Mark】拥有了至少和任何开放硬件型号一样功能的打印机。

[https://www.youtube.com/embed/V1UhqT5iOXk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/V1UhqT5iOXk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)