# 将 Stellaris Launchpad 转变为逻辑分析仪

> 原文：<https://hackaday.com/2013/01/27/turning-the-stellaris-launchpad-into-a-logic-analyzer/>

![acquisition](img/4762a1f7ae11ed2cf94775c98e61d9a4.png)

如果你有一个 Stellaris Launchpad，试着把它用作逻辑分析仪

Stellaris 逻辑分析仪基于[这个早期版本](http://jjmz.free.fr/?p=148),它从一个可与 Arduino 逻辑分析仪相媲美的水坑中提取代码，并将其移植到一个速度更快、功能更强的 Stellaris Launchpad，该平台采用 ARM Cortex 4F 处理器。

这种构建将 Launchpad 变成了一个 10 MHz、8 通道逻辑分析仪，具有 16 kB 的缓冲区，由于采用了 SUMP 协议，几乎可以与所有软件相媲美。尽管 Launchpad 中的 ARM 芯片不支持 5 伏，但只有端口 B 上的引脚 0 和 1 被限制为 3.6 伏。端口 B 上的所有其他引脚都可以承受 5 伏电压。

把一直放在你工作台上的 Launchpad 变成一个有用的工具是一件不错的工作。