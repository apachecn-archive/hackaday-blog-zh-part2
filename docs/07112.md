# [Sprite_TM]将 Linux 放入时钟收音机中

> 原文：<https://hackaday.com/2014/09/18/sprite_tm-puts-linux-in-a-clock-radio/>

【雪碧】需要一个闹钟才能在早上醒来，虽然他的手机有一个无限可编程的闹钟，但他的老飞利浦 AJ-3040 从未让他失望过。这 15 年来他一直受益匪浅，没有理由抛弃它。升级它是唯一的方法，在这个便宜的消费电子产品盒子里有有机发光二极管显示器和 Linux 系统。

打开收音机后，[雪碧]找到了两块板。第一个是无线电 PCB，现有的电路板可以稍加修改，用开关输入另一个音频源。时钟 PCB 是围绕一个使用电源频率作为时基的旧芯片构建的。这是与旧的多路复用液晶屏一起从机箱中撕下来的。

时钟需要一个新的显示器和大脑，于是[Sprite]从他的零件抽屉里拿出一个旧的 288×48 像素的有机发光二极管显示器。当通过一点半透明的红色塑料发光时，它可以是旧 led 的合理复制品。时钟的大脑是一个杨桃 Linux 模块。在为有机发光二极管编写了一个内核模块后，[Sprite]拥有了一台功能齐全的 Linux 计算机，可以放入一个时钟收音机中。

在有了一块装配了电源、I2C 扩展器、USB 立体声 DAC 和有机发光二极管 SPI 端口的电路板之后，[Sprite]有了一个可以在有机发光二极管屏幕上启动 Linux 的时钟收音机。在下面的视频中，[Sprite]演示了时钟的功能，包括设置众多闹钟中的一个，从互联网上流式传输音频，以及更改显示器的字体。该时钟还有一个网络用户界面，可以远程设置闹钟——甚至可以从手机上设置，如果[Sprite]愿意的话。

[https://www.youtube.com/embed/Ktyp-08oinM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Ktyp-08oinM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

现在你知道为什么[Sprite] [是 Hackaday 奖](http://hackaday.com/2014/06/17/judge-spotlight-sprite_tm/)的评委了。