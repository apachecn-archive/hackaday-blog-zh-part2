# GPIB 连接二合一

> 原文：<https://hackaday.com/2012/05/01/gpib-connectivity-twofer/>

掸去旧 GPIB 硬件的灰尘，使用这两种解决方案之一将其连接到您的现代计算平台。如果你不知道我们在谈论什么，你可能没有任何 50 年前的测试设备。但是通用接口总线(也称为 IEEE-488)在 1960 年代的测试设备中相当普遍，比如万用表和逻辑分析仪。

【斯文·泡利】负责[左上角的 RS232 GPIB 接口板](http://www.mikrocontroller.net/articles/GPIB-RS232-Schnittstelle) ( [翻译](http://translate.google.com/translate?sl=auto&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fwww.mikrocontroller.net%2Farticles%2FGPIB-RS232-Schnittstelle))。它使用 ATmega16 和几个经典的总线驱动芯片来完成这项工作。

右下角是[史蒂文·卡萨格兰德]开发的 USB 转 GPIB 转换板。这个是基于 PIC 的，使用 18F4520 和 FTDI 芯片来处理等式的 USB 端。

检查用于此协议的连接器。我们打赌这不是最容易找到的部分。但至少现在你会知道当你在跳蚤市场搜寻商品时你在看什么。