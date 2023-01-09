# 向 A & B 的 Rasberry Pi 型号添加 I/O

> 原文：<https://hackaday.com/2014/09/09/adding-io-to-the-rasberry-pi-models-a-b/>

树莓派已经成为许多酷项目的基础。即便如此，A 型和 B 型一直被批评只有少数 GPIO 引脚可用。当然，新型号 [B+](http://hackaday.com/2014/07/13/introducing-the-raspberry-pi-b/) 有一个 40 针 GPIO 头，但如果你想使用你的旧 RaspPi 和一堆输入和输出呢？[Steve]就是其中之一，他创造了一个非常简洁的解决方案，他称之为 [PiMagic](http://croztech.wordpress.com/pimagic-interface-board-about/) 。这是一个 Pi 板，板上有一个运行 Arduino 引导程序的 ATMEGA328。RaspPi 和 Arduino 通过 UART 通信，因为[Steve]觉得这比走 SPI 或 I2C 路线要简单一些。

RaspPi GPIO 的运行电压为 3.3v，ATMEGA328 的运行电压为 5v。为了解决这个问题，PiMagic 有一个电平转换器，可以保持两个板的 I/O 正常工作。旧的 Pi 在 5v 电源线上提供太多电流时会烧坏 PCB 走线。[史蒂夫]扔了一个保险丝，它会在 Pi 之前烧断，以确保没有 Pi 在这个项目的制作过程中受到伤害。

现在有了许多可用的 I/O，如何物理地访问它们呢？嗯，PiMagic 在典型的 Arduino 布局中有母头。这样，任何 Arduino 屏蔽都可以直接插入。[Steve]将他所有的[源文件提供给那些想自己制作一个的人。休息后找个组装视频。](https://github.com/croztech/pimagic)

[https://www.youtube.com/embed/Jp27--h3kW4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Jp27--h3kW4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)