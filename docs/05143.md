# 微控制器上的小型计算机

> 原文：<https://hackaday.com/2014/01/24/minicomputers-on-microcontrollers/>

PDP-11 系列小型机开发于 60 年代末至 70 年代，很可能是有史以来最重要的一台计算机。第一个广泛发行的 Unix 和 C 版本是在 PDP-11 上开发的，从摩托罗拉 68000 到 MSP430，它的硬件影响无处不在。

当[戴夫·切尼]看到最近用 4kB C 代码编写的 8086 模拟器时，他意识到模拟整个计算机系统实际上并不需要一大块内存之外的大量资源。带着一个 Arduino 巨型克隆体，他开始了我们最近见过的最酷的项目之一:[在 AVR 上模拟 PDP-11。](http://dave.cheney.net/2014/01/23/avr11-simulating-minicomputers-on-microcontrollers)

[Dave]使用 ATMega2560 驱动的 Arduino Mega clone 和以太网模块作为该版本的硬件。连接到它的是一个充满一对 RAM 芯片的屏蔽，它扩展了“Mega”上相对有限的 RAM。

到目前为止，[Dave]已经让他的模拟系统从 SD 卡启动 Unix V6。对于 PDP-11 存储，他还模拟了 RK05 磁盘驱动器，这是一个包含 2.5 兆数据的 14 英寸大磁盘。与最初的 PDP-11/40 相比，[Dave]估计他的机器大约慢 10 倍。尽管如此，原始的 11/40 系统占据了多个服务器机架，并且最常见的安装消耗几千瓦的电力。Arduino Mega 可以放在口袋里，可以通过 USB 供电。

该系统的未来发展包括提高模拟器的精度，运行更先进的操作系统和 DEC 诊断程序，并可能加快模拟速度。我们建议在额外的防护罩上增加一些开关和闪光灯，但这只是我们的想法。

所有代码都可以在[【Dave】的 git](https://github.com/davecheney/avr11) 上找到，关于他的 SPI RAM shield 的描述很快就会出现。