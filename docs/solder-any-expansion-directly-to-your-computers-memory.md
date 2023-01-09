# 将任何扩展直接焊接到计算机的内存中

> 原文：<https://hackaday.com/2015/06/12/solder-any-expansion-directly-to-your-computers-memory/>

加热熨斗，你会想试试这个:[Hugatry]正在通过接入内存模块上的 i2c 线给他的笔记本电脑添加硬件。我们喜欢这一点，因为焊接过程中损坏内存的代价比直接焊接到主板上要低得多！

直到休息后我们看了视频，我们才意识到内存模块上通常有一个 i2c EEPROM。这实际上是一个名为[串行存在检测](http://en.wikipedia.org/wiki/Serial_presence_detect)的标准，它允许 BIOS 轮询内存并自动配置。似乎具有讽刺意味的是，我们知道[树莓派帽子标准](https://www.raspberrypi.org/introducing-raspberry-pi-hats/)使用相同的技巧，但不知道它也在计算机内存中。

硬件方面，这提供了一种将自己的设备焊接到总线上的简单方法。从那以后，它就变成了一个软件黑客。当然，Linux 使这变得非常容易，这一点由[Hugatry]用 LM75 温度传感器进行了演示。我们希望听到我们的 Windows 和 OSX 用户读者关于如何在这些操作系统中访问 i2c 总线的意见。

[https://www.youtube.com/embed/H8Rkk8McYCw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/H8Rkk8McYCw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)