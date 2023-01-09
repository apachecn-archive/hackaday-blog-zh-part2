# Arduino 也可以编程 PIC！

> 原文：<https://hackaday.com/2012/05/02/arduino-can-program-pic-too/>

这是[Soranne]在开发使用 Arduino 板对 PIC 微控制器进行[编程的方法时整理的接线图。您可以看到，他通过将主 Clear (MCLR)引脚连接到外部电源来解决 12V 问题。这伴随着一个警告，Arduino 应该总是在连接之前被重置。](http://arduino.cc/forum/index.php/topic,92929.0.html)

他用 16F628 对此进行了测试，并高兴地报告说，他可以成功地刷新程序存储器，但尚未实现写入 EEPROM 的方法。这应该适用于任何 16F 系列芯片，但我们敢打赌，如果一些有知识的人决定伸出援手，这将得到扩展。

在个人电脑方面,[Soraane]一直在开发一个程序，通过 USB 连接将代码推送到 Arduino。他正在用 C#开发它，甚至为这个项目开发了一个 GUI。你可以在上面链接的第二篇帖子中找到这个软件，但是你必须登录 Arduino 论坛才能看到下载链接。

我们认为 12V 问题是为什么我们没有看到更多的 PIC 自主程序员。但是有一些解决方案，比如这个 ATmega8 版本。