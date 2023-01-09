# 树莓 Pi 型号 B+来了(又来了！)

> 原文：<https://hackaday.com/2014/07/14/the-raspberry-pi-model-b-is-here-again/>

取决于你相信谁，昨天有人要么打破了一个 NDA，要么是一个元素 14 运输错误的幸运接收者。尽管如此，我们还是很幸运地得以一睹新款树莓派 B+ 的风采。今天，一切都是实时的， [Adafruit 有一个很好的拆解](https://learn.adafruit.com/introducing-the-raspberry-pi-model-b-plus-plus-differences-vs-model-b?view=all)什么是新的，什么是改变，什么是这个新的板完全不同。

关于这个新 Pi 的最大问题是 CPU:型号 A 和 B 中的 Broadcom SoC 现在看起来有点老了，升级的 CPU 将是一个非常非常受欢迎的补充。没有变化。这是同样的 700 MHz Broadcom 芯片，内存为 512MB。也不会有“神奇的，因为你很棒”的 RAM 升级，最初的 Model B 在生产早期就看到了 SoC 中根本没有足够的地址引脚。

尽管没有升级 CPU，但有一些简洁的功能解决了最初 Pi 的抱怨:标准大小的 SD 卡插槽被一个不会伸出主板边缘的 microSD 卡插槽取代。端口被重新安排，模拟视频和音频一起通过 TRRS 插头输出。由于这个芯片，现在有四个 USB 端口和一个以太网端口[，还有大量的安装孔:它们是 58 毫米宽、49 毫米高的正方形中的 2.5 个孔。B+还包括一个完全重新设计的电源——巨型线性稳压器不见了，取而代之的是一个全面更好的电源。](http://www.microchip.com/wwwproducts/Devices.aspx?product=LAN9514)

对于任何想用 Pi 做项目的人来说，最大的变化是扩展的 GPIO 头。这是一个 40 针接头，其“顶部”引脚与原来的 26 针接头相同。是的，你现有的所有 Pi 板/护盾/无论什么都还能工作。这个接头上的新引脚包括九个 GPIO 引脚，用于 [Wolfson 声卡](http://www.element14.com/community/community/raspberry-pi/raspberry-pi-accessories/wolfson_pi)的 I2S 引脚，以及一对用于 ID EEPROM 的引脚。到 ID EEPROM 的连接已经成为 BeagleBone 的一个特性有一段时间了，这将允许 Pi 在启动时配置适当的 I/o 和内核模块，这取决于连接的 Pi 板。

最好的部分是价格——它和 OG Model B 一样。使用与你的旧 Model A 或 B 相同的外壳是不可能的，但这完全是 Kickstarter 的目的，对吗？你可能想抓一个，因为这可能会成为升级版 Raspberry Pi 2.0 的外形，它可能会在一两年内发布。