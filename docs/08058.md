# 在 TCP 上使用 Librtlsdr

> 原文：<https://hackaday.com/2015/01/13/using-librtlsdr-over-tcp/>

[Texane]建造了一个低成本的软件定义无线电设备，可以远程控制。这使得硬件可以放置在室外以获得更好的接收效果，同时可以从任何可以通过 TCP 连接的 PC 进行控制。为了做到这一点，他[创建了 librtlsdr 的分支](https://github.com/texane/librtlsdr/tree/rpc)，该库用于将[廉价电视调谐器转变为软件定义的收音机](http://hackaday.com/tag/rtl-sdr/)。

官方发布的 [rtl-sdr](http://sdr.osmocom.org/trac/wiki/rtl-sdr) 包含了 [rtl_tcp](http://sdr.osmocom.org/trac/wiki/rtl-sdr#rtl_tcp) 实用程序，就是为了这个目的。不幸的是，并不是所有用于 Linux 的 SDR 工具都支持这一点。通过修改库本身，远程设备以与本地设备相同的方式与软件交互。这意味着任何支持 librtlsdr 的软件都应该可以工作。

户外装备包含一个 BeagleBone Black 和 SDR 硬件，密封在一个防风雨的盒子里。这通过以太网连接到[Texane]的家庭网络，并允许 SDR 实用程序在其他地方运行。

这个特性是实验性的，但是 fork 的源代码是为那些想要构建代码并尝试它的人提供的。