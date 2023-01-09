# 使用 BeagleBoard-xM 进行 USB 嗅探

> 原文：<https://hackaday.com/2013/07/02/usb-sniffing-with-the-beagleboard-xm/>

[Matlo]写来分享他使用 BeagleBoard-xM 的 [USB 嗅探项目。它建立在 2010 年谷歌代码之夏项目的基础上，该项目使用非 xM 版本的硬件](http://blog.gimx.fr/?p=604)[构建了一个通过 USB 嗅探器的通道](http://www.elinux.org/BeagleBoard/GSoC/2010_Projects/USBSniffer)。[Matlo]当时无法让它工作，但最近重新访问了该项目。他清理了一些脚本，通常也让其他人更容易完成。

上面看到的基于 ARM 的 BeagleBoard 充当中间人。将目标 USB 设备连接到电路板，并将电路板连接到计算机。该板模拟目标设备，在任一方向上传递数据包，同时记录它们。使用 [WireShark](http://www.wireshark.org/) ，捕获的数据以正确的格式显示，WireShark 是理解捕获的通信数据包的事实标准。

这对于弄清楚如何在非标准系统上使用 USB 设备非常有用，反之亦然。