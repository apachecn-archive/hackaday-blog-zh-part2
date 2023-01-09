# 试验板上的 Unix

> 原文：<https://hackaday.com/2015/05/21/unix-on-your-breadboard/>

随着智能手机变得越来越大，运行 Unix(或 Linux，视情况而定)的最小芯片的竞赛仍在继续。这个领域的一个新竞争者是[Serge],他在 Fubarino 微控制器上安装了一个功能强大的试验板友好型设备。

该器件使用 PIC32MX795 处理器来运行用于微控制器的 2.11BSD Unix 版本。它只使用 128 千字节的内存，这对于有限的可用空间来说是非常好的，但它并不吝啬软件。它有一个 C 编译器、汇编器和一大堆其他的实用工具，你可以在一些更强大的工具中找到它们。所有这些都包含在一个具有试验板兼容引脚的包中，因此您可以将您的 Unix 与现实世界进行交互。

下面有一个视频展示了该设备的运行情况，如果你有可用的硬件，还有一整套说明可以让你立即启动并运行。[Serge]提到这可以在其他架构上运行，但正在寻找其他人加入该项目，将其移植到这些处理器上。这不是我们第一次看到在微控制器上安装 [*nix，但它是更有用的一个！](http://hackaday.com/2012/03/28/building-the-worst-linux-pc-ever/comment-page-2/)

[https://www.youtube.com/embed/eddEQn_Bm3k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/eddEQn_Bm3k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)