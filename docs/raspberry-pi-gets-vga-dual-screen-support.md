# 树莓 Pi 获得 VGA，双屏支持

> 原文：<https://hackaday.com/2014/09/10/raspberry-pi-gets-vga-dual-screen-support/>

事实证明，Raspberry Pi 中的 Broadcom SOC 实际上非常强大。它实际上能够使用少量电阻通过 GPIO 引脚驱动 VGA 显示器。

[Gert van Loo]，Raspberry Pi 芯片架构师、向导和许多有趣扩展板的创造者，本周在剑桥举行的 Raspberry Pi Jam 上展示了新 B+型号的 VGA 适配器。显然，SoC 上有一个并行接口，可用于利用电阻梯形 DAC 驱动 VGA。这是 1080p、60 fps 的原生 VGA*以及用于树莓 Pi 的 HDMI* 。只有[的新型号 B+](http://hackaday.com/2014/07/14/the-raspberry-pi-model-b-is-here-again/) 有足够的引脚来做到这一点，但这是一个有趣的小板。

一个树莓派有两个显示器的前景非常有趣，剩下的四个可用的 GPIOs 意味着一个触摸屏可以添加到一个显示器上，有效地制作一个巨大的任天堂 DS。当然，双显示器 Raspi 解决了更多实际问题，如为当前的 DSP/树脂 3D 打印机驱动投影仪，同时在打印过程中仍然允许可用的界面。

VGA 扩展板“可能与 EMC 有问题”，这意味着它可能不会成为产品。不过，制作 PCB 和焊接 SMD 电阻并没有那么难，我们会在电路板文件发布时发布更新。

感谢[Uhrheber]发送这封邮件。