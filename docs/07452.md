# FPGA 中视差推进器的改进

> 原文：<https://hackaday.com/2014/10/30/improving-the-parallax-propeller-in-an-fpga/>

Parallax Propeller 是一款有趣的芯片，并没有得到太多的喜爱，但由于整个芯片都是开源的，这种情况可能会发生变化:人们将这种芯片放在 FPGA 中，并修改二进制文件[，以赋予芯片在最初的](http://syso.name/s/parallax-propeller-p8x32a-v-with-64-i-o/)中从未存在的功能。

去年 8 月，Parallax [发布了 P8X32A](http://hackaday.com/2014/08/07/parallax-propeller-1-goes-open-source/) 的源代码，让任何拥有 FPGA 板的人都能够[为自己的设计尝试道具](http://hackaday.com/2014/08/24/fpga-with-open-source-propeller-1-running-spin/)。从那时起，一些人投入了一些时间，清理文件，解读 ROM 映像，修复错误，以及一个开源微控制器内核所需的所有常规维护。

[Sylwester]抓取了视差论坛上[发现的一些实验变化，并把它们作为 Propeller 源的一个分支包含进来。它支持第二个 32 位端口，为新芯片提供 64 个 I/O 引脚、乘法指令、视频生成器、硬编码 SD 卡库，以及一种称为微程序的变体，该变体具有四个核心而不是八个核心。](http://forums.parallax.com/forumdisplay.php/101-Propeller-1-Verilog-Code-Development)

您可以在这里获取所有更新的源[，并将其加载到 DE0 Nano FPGA 板上。如果你非常幸运，拥有 Altera DE2-115 开发板，你也可以运行即将到来的 Propeller 2。](https://git.no-route.org/syso/p8x32a_emulation/tree/v0.4b-PORTB-MUL)