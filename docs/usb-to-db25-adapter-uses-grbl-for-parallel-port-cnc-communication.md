# USB 转 DB25 适配器使用 GRBL 进行并行端口 CNC 通信

> 原文：<https://hackaday.com/2014/09/16/usb-to-db25-adapter-uses-grbl-for-parallel-port-cnc-communication/>

随着新计算机的不断生产，并行端口有越来越不常见的明显趋势。对于我们年轻的读者来说；并行端口是一种接口标准，用于计算机和各种外围设备之间的双向通信。并行端口的消亡部分是由于 USB 标准的发明。

如果摆弄数控机床是你的爱好之一，那么你应该熟悉并行端口接口在数控控制板连接中相当流行。那么，如果你的新电脑没有并行端口，但你仍然想运行你的数控机床，你该怎么办？嗯，你肯定不会被卡住，因为[Bray]已经提出了一个专门用于 CNC 的 [USB 转并行端口适配器](http://www.coreforge.com/blog/2014/08/grbl-tb6560-interface/)解决方案。

一个便宜的现成的 [USB 转 DB25 适配器](http://cdn-images.sewelldirect.com/products/SW-4518/SW-4518.jpg)乍一看可能是个好主意，但它们不适用于 CNC 应用。[Bray 的]适配器基于 Arduino，运行 [GRBL](http://bengler.no/grbl) 。GRBL 代码负责获取从计算机发送的 g 代码命令，将它们存储在缓冲器中，直到它们准备好被转换为步进和方向信号，并通过并行端口 DB25 连接器发送到 CNC 控制器。对于需要控制数控机床但没有并行端口的人来说，这是一个很好的解决方案。

[Bray]正在使用运行 [GRBLweb](https://github.com/andrewhodel/grblweb) 的 Raspberry Pi 来控制他的适配器板。但是，您可以使用其他程序与 GRBL 通信，例如[通用 g 代码发送器](https://github.com/winder/Universal-G-Code-Sender)和 [GRBL 控制器](http://zapmaker.org/projects/grbl-controller-3-0/)。

该板是在 [Eagle](http://www.cadsoftusa.com/eagle-pcb-design-software/product-overview/?language=en) PCB 软件中创建的，并使用【Bray’s】CNC 路由器铣削而成。这种设计是单面的，非常适合自制的 PCB。他甚至为开始、保持和重置输入按钮制作了一个子板。像所有伟大的 DIY 者一样，[Bray]已经将他的电路板和原理图文件提供给其他人下载。