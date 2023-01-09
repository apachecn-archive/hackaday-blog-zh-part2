# 光滑的浴室镜子被装饰一新

> 原文：<https://hackaday.com/2015/02/12/slick-bathroom-mirror-is-all-tricked-out/>

在电影明星的化妆间里，你通常会看到一面被一串明亮的灯包围着的镜子。[pickandplace]从电影和黑暗的浴室中获得灵感，设计出一款配有一些铃铛和口哨的浴室镜子。首先，他的计划非常详细，为他的设计勾勒出特征和限制。他选择使用一个带有 12 个 LED 灯泡(比 220 伏灯泡安全)的圆形镜子，这样它就可以像时钟一样工作。用户输入由运动传感器处理，以自动打开/关闭和电容式触摸调光器。引擎盖下有一个 RTC(用于根据一天中的时间调整时钟和亮度)，简单的升压 PWM LED 驱动器，10W LED 的热管理，温度传感器，如果 LED 太热，可以降低电流，甚至还有一个防雾加热条–唷！

他的处决同样出色。从搭建木制框架开始，到编写驱动所有电子设备的代码结束。在此过程中，您会发现关于 led、PWM 驱动器、散热和使用 Atmel at 42qt 2160 q slide 矩阵传感器 IC 的电容式触摸调光器的详细说明。他在运动传感器 PIR 模块上遇到了一些问题，还没有编写实现它的代码。他的第一个版本使用了 PIC18F87J50，下一个版本使用了 atx mega 256 a3 bu——但他要求我们不要卷入微芯片与 Amtel 的辩论。我们必须在这一点上达成一致。敏锐的读者会指出，这两个微处理器都不能提供 12 个 PWM 通道。别担心，他都想好了。他还编写了一个简单的控制界面，当该装置通过 USB 连接到计算机时，这个界面非常方便。最重要的是，他制作了一个微型 LED 环，在编写代码时用作“模拟器”，这样他就不必拖着沉重的镜子进出浴室。怎么样才能把工作做得更好！源文件在他的 Github repo 上，硬件原理图的链接遍布他的博客。

如果你不想建造如此花哨的东西，看看带 HUD 显示时间和天气的[浴室镜子](http://hackaday.com/2011/03/02/bathroom-mirror-hud-displays-time-and-weather/)

[https://www.youtube.com/embed/1UKBAC_c-Fg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1UKBAC_c-Fg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)