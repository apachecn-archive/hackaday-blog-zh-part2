# 超频微控制器

> 原文：<https://hackaday.com/2012/12/27/overclocking-microcontrollers/>

我们都熟悉超频台式电脑；一个很好的介绍热设计功率和一个好的 CPU 冷却器的必要性。[Marcelo]想看看他能超频一个微控制器到什么程度——在这种情况下是 atmega 328——[最终得到了一个为 20 MHz 设计的运行频率为 30 MHz 的微控制器。](http://garagelab.com/profiles/blogs/atmega328-overclock-30mhz)

为了验证他的 uC 可以以更高的时钟速度运行，[Marcelo]开始了他的实验，上传了一段代码，尽可能快地切换几个引脚。他需要用一个普通的 16 MHz 晶体上传这些代码——当芯片的时钟速度更高时，AVRDude 根本无法工作。

在成功演示了他的微控制器可以以 30 MHz 的频率打开和关闭引脚后，[Marcelo]想看看他是否能做些有用的事情。通过编辑他的 Arduino boards.txt 文件中的单个设置。，[Marcelo]能够让他的超频微控制器读取并回复通过串行连接发送的字符。它成功了，证明了超频微控制器在某些情况下是有用的。

至于[Marcelo]计划用他的更快的微控制器做什么，他正在考虑改进 ATMega 供电的 VGA 彩色发生器。更高的时钟速度意味着他可以将更多的像素推到 VGA 显示器上。