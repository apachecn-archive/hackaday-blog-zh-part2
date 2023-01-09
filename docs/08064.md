# [Tesla500]制造高速摄像机

> 原文：<https://hackaday.com/2015/01/15/tesla500-builds-a-high-speed-video-camera/>

[Tesla500]热衷于高速摄影。不幸的是，像 Phantom Flex 这样的高速摄像机的成本高达数万甚至数十万美元。当工具太贵时，你唯一能做的就是——自己动手制作！【Tesla 500 的】HSC768 因其图像传感器的数据传输速率而得名。由于安森美半导体 [Lupa1300-2](http://www.onsemi.com/PowerSolutions/product.do?id=LUPA1300-2) 图像传感器使用 10 位像素格式，每秒 768 百万像素相当于大约 960 兆字节/秒。

这实际上是[Tesla 500]的第二个高速摄像机，第一个是 HSC80，基于慢得多的 Lupa300 传感器。HSC80 确实可以工作，但它与 FPGA devboard 相连，由 PC 控制。[Tesla 500]的经验在第二次努力中得到了真正的体现，因为 HSC768 是一个完整的便携式系统，运行 Linux，具有基于 QT 的 GUI 和触摸屏。3D 打印的外壳让相机拥有了我们熟悉的 DSLR/ [MILC](http://en.wikipedia.org/wiki/Mirrorless_interchangeable-lens_camera) 的外形。

处理器是德州仪器公司的 TMS 320dm 8148 da Vinci，运行 TI 定制的 Linux。达芬奇控制了大多数普通的东西，比如 GUI、触发器 I/O、SD 卡和 SATA 接口。真正神奇的是高速图像采集，全部由 FPGA 处理。高速图像采集需要高速内存，而且是大量的高速内存！谢天谢地，台式电脑给了我们大容量、高速的 DDR3 ram 模块。然而，当设计相机时，[Tesla500]发现 Xilinx 和 Altera 都没有支持 DDR3 模块的 1000 美元以下的 FPGA。当然，它们将支持单个 DDR3 芯片，但处理芯片时成本要高得多。Lattice 确实有一个低成本的 FPGA，具有[Tesla500]所需的功能，所以 Lattice ECP3 系列芯片进入了相机。

最终结果看起来非常值得[Tesla500]在这个项目上投入的所有努力。HSC768 能够以每秒 500 帧的速度拍摄 SXGA (1280×1024)视频，或以每秒 1200 帧的速度拍摄 800×600 灰度图像。较低的分辨率允许更高的帧速率。[Tesla500]甚至用相机分析了他在[气动干手器中遇到的一种奇怪的空气振荡。](http://hackaday.com/2014/11/04/ultra-powerful-pneumatic-hand-dryer/)点击休息时间，观看摄像机的概览视频和干手器视频。两者都包含一些惊人的高速序列！

[https://www.youtube.com/embed/yhUO673YgJg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/yhUO673YgJg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/6QWcTnYXZ48?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6QWcTnYXZ48?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)