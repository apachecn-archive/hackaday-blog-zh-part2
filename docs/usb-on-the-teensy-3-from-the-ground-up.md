# Teensy 3 上的 USB 接口

> 原文：<https://hackaday.com/2014/12/13/usb-on-the-teensy-3-from-the-ground-up/>

当在微控制器上实现 USB 时，如果使用 AVR，大多数人会使用 V-USB，如果涉及 PIC，会使用 Microchip 的 USB 库，或者针对各种 ARM 处理器的任何数量的 USB 库。[凯文]有不同的想法。作为对自己的挑战，[他为 Teensy 3.1](http://kevincuzner.com/2014/12/12/teensy-3-1-bare-metal-writing-a-usb-driver/) 微控制器板编写了一个 USB 设备驱动程序，尽可能地接近裸机。

编写 USB 设备驱动程序首先需要查阅文献。飞思卡尔 K20 系列微控制器(Teensy 3.1 中的微控制器)有一些特性，决定了对特定存储器布局的需求，使用多个时钟，并处理所有 USB 描述符。[Kevin]从时钟开始，每一个都必须启用。时钟由多用途时钟发生器从 16MHz 晶振产生，PLL 到 USB 模块需要的频率，并通过系统集成模块发送出去。

遵循 Freescale 参考指南中的流程图和序列，告诉[Kevin]启动序列到底需要做什么，并提供了一些关于设置所有中断需要做什么的建议。[Kevin]为了这个教程花了大量的时间来记录、编程和敲打键盘，但是他确实给了每个人一个很好的机会来从他的奋斗中学习。

虽然[Kevin]有一个基本完整的 USB 设备驱动程序，但他的工作还远远没有完成。没关系，因为这个项目并不意味着是一个全功能的驱动程序；它仍然缺少真正的错误处理、配置中的字符串和真正的 VID/PID。没关系，这仍然是从零开始构建东西的一个很好的练习，尤其是很少有人成功构建的东西。

哦，[明目张胆的 Hackaday Store plug](http://store.hackaday.com/products/teensy-3-1) 为了 Teensy 3.1。