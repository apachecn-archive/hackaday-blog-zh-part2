# 在图形计算器上运行 Debian

> 原文：<https://hackaday.com/2014/11/18/running-debian-on-a-graphing-calculator/>

虽然普遍存在的 TI-83 仍然使用古老的 Zilog Z80 处理器，但较新的 TI-Nspire 系列图形计算器使用现代 ARM 设备。[Ivoah]设法让 Debian Linux 在 TI-Nspire 计算器上运行，并写了一个指南解释这是如何做到的。

这个过程使用了 [Ndless](http://ndless.me/) ，这是一种越狱，允许代码在设备的底层运行。Ndless 还包括用于开发应用程序的完整 SDK、仿真器和调试器。在这种情况下，使用 Ndless 来加载 Linux 内核。

使用 [debootstrap](https://wiki.debian.org/Debootstrap) 和 [QEMU](http://wiki.qemu.org/Main_Page) ARM 仿真器在 PC 上构建根文件系统。这允许你在转换到计算器本身之前，通过 apt 安装任何需要的包。

有了 USB 闪存驱动器上的根文件系统，Ndless 运行 Linux 加载程序，它启动内核，挂载根文件系统，并在大约两分钟内引导到 Debian 系统。正如休息后的视频所展示的，这给你留下了一个计算器的外壳。我们不确定在图形计算器上用 Linux 做什么，但这是一个简洁的演示。

[https://www.youtube.com/embed/Evzz0wO-t78?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Evzz0wO-t78?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)