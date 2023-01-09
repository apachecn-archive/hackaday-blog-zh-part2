# 从头开始构建超小型 Linux 计算机

> 原文：<https://hackaday.com/2015/04/10/building-super-small-linux-computers-from-scratch/>

传统观点认为，小而强大的嵌入式 Linux，如 Raspberry Pi、Beaglebone 或 Intel Edison，是天生制造的设备，当然不是家酿修补匠可以在家里生产的。hak8or 正在这么做，在家里生产了不是一台，而是两台完全不同的微型 Linux 电脑。

第一个是基于 Atmel 的 AT91SAM9N12 ARM 处理器，但整个电路板只有大约两英寸见方。板上有 64 MB 的 DDR2 DRAM，一个 USB 主机和 OTG 端口，没有其他东西。不过，这款芯片运行的是从 USB 驱动器上剥离下来的 Linux。

第二块板基于 Freescale i.MX233。这块板的大小和功能相似，但它现在并不完全*工作*。DRAM 的时序有问题，SD 卡下面的电容有点太高了。

[hak8or]项目的真正价值在于他为这些回复在 readme.mds 中投入了大量的资源。如果你曾经想构建一个嵌入式 Linux 设备，这里是关于在这些芯片上引导 Linux 的信息的一站式商店。