# Arduino 操作系统

> 原文：<https://hackaday.com/2014/04/26/the-arduino-operating-system/>

虽然 Arduino 和它的库是与传感器接口和闪烁 LED 的最快方式，但有时你不应该编写和编译代码来做一些特别简单的事情。[Oliver]意识到微控制器的大多数过于简单的功能都可以通过运行在该微控制器上的命令行来完成，于是[开发出了迷你海盗](http://www.instructables.com/id/Arduino-comand-line-tool-MiniPirate/?ALLSTEPS)，Arduino 命令行工具。

MiniPirate 只是在 Arduino 上编译的草图，它允许引脚设置为高电平或低电平，设置 PWM 值，或者读写 I2C 字节。它基本上是总线盗版的一个极其精简的版本，意味着对电路和外围设备的极其简单的修改。

[Oliver]演示了他的迷你海盗，他拿了一个 DS1307 实时时钟，连接了 I2C 总线，并写入了设置时间的值。这是一个非常简单的实现，意味着他需要用十六进制写所有的东西，但它仍然很容易在许多其他项目中找到用途。