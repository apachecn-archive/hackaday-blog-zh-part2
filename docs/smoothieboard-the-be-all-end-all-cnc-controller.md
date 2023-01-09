# Smoothieboard 是最重要的 CNC 控制器

> 原文：<https://hackaday.com/2013/09/30/smoothieboard-the-be-all-end-all-cnc-controller/>

不久前[我们看了一下 3D 打印机的电子板](http://hackaday.com/2013/09/06/3d-printering-electronics-boards/)，讨论了打印机、激光切割机和研磨机最常见的电子板的成本和优势。最令人印象深刻的电路板之一是 Smoothieboard，但当时找到供应商有点困难。现在， [Smoothieboard 在 Kickstarter](http://www.kickstarter.com/projects/logxen/smoothieboard-the-future-of-cnc-motion-control) 上发布，让每个人都有机会接触这款非常酷的 CNC 控制板。

虽然大多数 RepRap 和 3D 打印机控制器板使用 ATMega 或其他 8 位微控制器，但 Smoothie 使用恩智浦 LPC Cortex-M3 芯片形式的 32 位 ARM 芯片。这不仅允许 Smoothie 在你的机器上做一些非常酷的事情——例如，原生弧和圆，而且这种更好的硬件还允许以太网，拖放固件，以及将 USB 端口作为串行端口或大容量存储设备。

思慕雪有三种口味，有 3、4 或 5 个步进电机驱动器。这些 Allegro A4982 驱动器对于任何 3D 打印机、激光切割机或小型工厂来说都足够好，但断开的引脚允许步进驱动器提供超过 2A 的电流。

smoothie 板上的一切都是模块化的，这意味着该板同样能够为 RepRap、mill、激光切割机或绘图仪供电。甚至有一个[计划控制面板](http://smoothieware.org/smoothiepanel)称为 Smoothiepanel，使它成为你下一个 CNC 构建的绝佳选择。