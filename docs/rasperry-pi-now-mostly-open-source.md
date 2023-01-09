# Rasperry Pi:现在大部分都是开源的

> 原文：<https://hackaday.com/2012/10/24/rasperry-pi-now-mostly-open-source/>

![](img/0f7b1507b9cff9526ea22f3c978fbf7c.png "Raspi")

如果你一直在关注为 Raspberry Pi 构建 Android、Chromium 和其他操作系统的进展，你会发现一个共同的主题。Raspi 芯片的驱动程序是闭源的，由 Broadcom 用 NDA 保护。这限制了开发人员承担涉及 CPU 内部混乱的项目的能力。

今天，[不再是这种情况](http://www.raspberrypi.org/archives/2221)。Raspberry Pi 上的 CPU 现在是第一个基于 ARM 的系统，具有功能齐全的供应商提供的驱动程序。

以前，OpenGL ES、OpenMax 和 ARM 芯片中其他好东西的驱动程序一直是封闭源代码的，只对 Raspberry Pi 基金会和那些愿意与 Broadcom 签署保密协议的人开放。在这个版本中，驱动程序是开源的，允许 Android、Chromium、Haiku、*BSD 和 RISC OS 背后的开发人员深入研究 Broadcom 驱动程序，并使他们的项目正常工作。

新文件可以在 [Raspberry Pi git](https://github.com/raspberrypi/userland) 中获得，只等开发人员查看。