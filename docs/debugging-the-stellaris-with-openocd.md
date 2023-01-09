# 用 OpenOCD 调试 Stellaris

> 原文：<https://hackaday.com/2012/10/21/debugging-the-stellaris-with-openocd/>

![](img/9423d21d21db259e91b8bd3d48f71b4a.png "StellarisLaunchPad")

看起来好像德州仪器真的通过他们新的 ARM 驱动的 Stellaris 开发板接触到了黑客社区。在 Stellarisiti 论坛上，一名成员[询问 Stellaris 板的调试选项](http://forum.stellarisiti.com/topic/197-can-i-debug-the-stellaris-launchpad-via-gccgdb/)。Stellaris 已经有了一个[在线调试接口](http://www.ti.com/tool/stellaris_icdi_drivers#&lid=en_US_folder_ts_top_anchor_support_community) (ICDI)，但不幸的是在 Linux-ey 环境下工作有点困难。

[开放式片上调试器](http://openocd.sourceforge.net/)的其中一个开发人员已经在与 TI 沟通，以获得 Stellaris 板的 ICDI 规范。TI 发布了信息，经过相当多的工作，[的一切都向所有人开放。](http://forum.stellarisiti.com/topic/197-can-i-debug-the-stellaris-launchpad-via-gccgdb/#entry1098)

目前，对 Stellaris 的 OpenOCD 支持仍然不完整，但 Gits 上有一个项目[允许为 ti 的新板进行多平台开发。](https://github.com/utzig/lm4tools)

不用说，让一切正常运行仍然是一件苦差事。不过，这并不是真正的问题；Stellaris 才出现了几个月，开发人员需要时间将所有需要的工具放入漂亮整洁的包中。我们很高兴 TI 在相关文档方面如此积极，以免开发变得困难一百万倍。