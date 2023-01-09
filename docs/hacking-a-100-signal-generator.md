# 黑进一个 100 美元的信号发生器

> 原文：<https://hackaday.com/2015/07/01/hacking-a-100-signal-generator/>

信号发生器是电子工作台上的一个有用的工具。缺点是它们往往相当昂贵。如果你有 100 美元买一个新玩具，MHS-5200A 是一个低成本、双通道、25 MHz 的发生器，可以在易贝找到。

缺点是软件。这是一个丑陋的 Windows 界面，用起来很痛苦。好消息是[wd5gnr] [对协议](http://www.eevblog.com/forum/testgear/mhs-5200a-serial-protocol-reverse-engineered/)进行了逆向工程，所以您不必这么做。这意味着可以开发其他软件来控制设备。

当连接到计算机时，这个函数发生器显示为一个虚拟的 USB 串行端口。[wd5gnr]汇编的[文档](https://docs.google.com/document/d/1HbLQ4u87RJkD3Ktyw7k9U7Zh5BPNzbrhMlszNGdXiiY/edit)列出了你可以发送的所有串行命令，以及它们的作用。如果您不喜欢从串行终端手动设置波形(谁喜欢？)在 [Github](https://github.com/wd5gnr/mhs5200a) 上有一个工具可以自动做到这一点。这将接收一个描述波形的 CSV 文件，并对发生器进行编程以生成波形。

该软件还与[波形管理器和](http://tti1.co.uk/downloads/waveman-plus.htm)兼容，后者是一个用于定义波形的免费 GUI 工具。把这些放在一起，你就可以用不到 100 美元买到一个非常强大的波形发生器。