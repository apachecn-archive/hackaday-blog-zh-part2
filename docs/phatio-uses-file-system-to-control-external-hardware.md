# PhatIO 使用文件系统来控制外部硬件

> 原文：<https://hackaday.com/2012/11/29/phatio-uses-file-system-to-control-external-hardware/>

[Andrew Smallbone]写了一个他最新开源项目的链接。这是 phatIO，[一个 USB I/O 设备，使用大容量存储文件系统进行控制](http://www.phatio.com/)。这个想法是任何操作系统都可以操作 USB 存储设备上的文件。这将枚举为大容量存储，您对其文件系统的任何更改都将导致 I/O 头上的 pin 操作。

我们长期以来一直是 Linux 的拥护者，并且很高兴看到*nix 系统上的所有东西都是一个文件。这只是将这个想法扩展到多个平台。[Andrew 的]硬件指南概述了系统的结构。顶层“io”目录包含名为 mode、pins、status 和其他几个子目录。目录中有每个 pin 的文件。写入这些文件与写入数据方向寄存器、端口寄存器或读取微控制器上的引脚寄存器具有相同的效果。

该板尚未投入生产，github 链接到他的硬件文件给了我们一个 404 错误。但是有几个软件演示的代码可用。休息之后，我们加入了费蒂奥驾驶拉森扫描仪的视频。

[https://www.youtube.com/embed/EZmZIUKY9oc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EZmZIUKY9oc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)