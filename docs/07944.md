# 用 CNC 闪存芯片

> 原文：<https://hackaday.com/2014/12/30/flashing-chips-with-a-cnc/>

[Eberhard]需要为他正在进行的一个项目展示数百台 ATMegas。这是一个问题，但是这个任务确实有一些使自动化变得容易的东西。Megas 焊接到的电路板还没有去板化，他有一个整洁而奇怪的钉床编程连接器。附近还有一台数控机床。这听起来像是自动化的理想情况，[，事实证明设置非常简单](http://pleasantsoftware.com/developer/3d/2014/07/10/pleasant-flashing/)。

有问题的电路板是用于[FPV/无线电控制遥测适配器](http://pleasantsoftware.com/developer/3d/zaggometry-naza2frsky-taranis-telemetry-adapter/)的，谢天谢地，组装厂在发货前没有将每块电路板上的 40 块印刷电路板拆除。一个非常酷的 [ATMega 闪存工具](http://www.hobbyking.com/hobbyking/store/__27195__Atmel_Atmega_Socket_Firmware_Flashing_Tool.html)处理计算机和微控制器之间的电气连接，但是仍然需要一个真实的活生生的人将这个闪存工具从一个芯片移动到下一个芯片，上传固件，并再次重复这个过程。

解决方案是在数控铣床的底座上放几个金属针，3D 打印闪存工具的适配器，并编写一点代码将闪存工具从一个芯片移动到下一个芯片。一个非常简单的应用程序负责将程序员移动到一个未刷新的芯片，上传固件，然后继续下一个芯片。

仍有一些工作要做，基本上将 Gcode 和 AVRdude 命令结合到一个界面中，但即使是现在，40 个 PCB 的完整面板也可以在 10 分钟多一点的时间内完成编程。你可以看看下面的视频。

[https://www.youtube.com/embed/bmolzgJAB4E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bmolzgJAB4E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)