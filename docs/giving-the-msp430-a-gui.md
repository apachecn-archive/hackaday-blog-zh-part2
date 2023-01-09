# 为 MSP430 提供一个图形用户界面

> 原文：<https://hackaday.com/2012/10/07/giving-the-msp430-a-gui/>

有时你需要切换或读取一个项目的微控制器上的几个引脚，这个项目如此简单(或如此临时)，以至于编写一些固件需要相当大的时间投入。[Jaspreet]也有同样的问题——想在不写任何代码的情况下读取值和切换引脚——所以他想出了一个相当聪明的解决方案,通过串行连接控制 MSP430。

[Jaspreet]称他的项目 ControlEasy，它确实像广告宣传的那样:它提供了一个软件接口，通过台式计算机控制 ADC 输入、PWM 输出和输出引脚的状态。ControlEasy 通过运行在任何带有硬件 UART(如 TI Launchpad)的 MSP430 上的匹配代码向计算机发送和接收数据来实现这一点。

现在，ControlEasy 可以读取模拟值，生成 PWM 输出，并将各个引脚设置为高电平和低电平。[Jaspreet]计划扩展他的软件，允许控制液晶显示器、I2C 和 SPI 设备。

在休息后的视频中，你可以看到[Jaspreet]通过 GUI 摆弄着他的 LaunchPad 上的一些大头针。如果您想试用，也可以下载该软件，但不幸的是，目前它仅适用于 Windows。

[https://www.youtube.com/embed/rMAQzwj42QI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rMAQzwj42QI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)