# 在 Windows RT 设备上运行 X86 应用

> 原文：<https://hackaday.com/2013/02/18/running-x86-apps-on-windows-rt-devices/>

Windows RT 是安装在 ARM 驱动的平板电脑和上网本(如新的微软 Surface)上的 Windows 版本，它有一个缺点:有数万个为 x86 硬件编写的应用程序根本无法在这种新的 ARM 驱动的架构上运行。虽然这可能会给医院、银行和其他需要适当 Wintel 平台的机构带来问题，但我们想知道如何让 Civ III 和帝国时代等经典游戏在这些新平板电脑上运行。

XDA 开发者论坛上的【mamai ch】[似乎用了很多魔法，为我们提供了一个解决方案。他创建了一个在 Windows RT 上运行 x86 Win32 应用的工具。基本上，他为 ARM 设备创建了一个 x86 模拟器，该模拟器还将 Windows API 调用传递给 Windows RT。](http://forum.xda-developers.com/showthread.php?t=2095934)

到目前为止，[mamaich]已经在他的 Windows RT box 上玩了一些经典的 Windows 游戏，包括来自 Windows 95 的*英雄无敌 3* 和*太空学员弹球*。一些实用程序如 7Zip 和 WinRAR 也可以使用。

[mamaich]的构建计划是使 x86 仿真更加自动化，而不需要单独的启动工具。最后，我们将拥有一个完美的 RTS 游戏便携平台。