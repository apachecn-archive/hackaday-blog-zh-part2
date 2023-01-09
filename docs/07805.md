# 通过汽车转速表倾斜你的 cpu

> 原文：<https://hackaday.com/2014/12/14/redlining-your-cpu-via-automotive-tachometer/>

许多 CPU 使用小工具在风格上借鉴了汽车，显示类似于仪表盘上的转速表的东西。[Pat]更进一步，尝试重新借用这种风格。他想，为什么不用一个实际的物理转速表来显示他的树莓派的 CPU 转速有多高呢？

我们的目标是将 0-100% CPU 使用率调整到转速为 0-8000 RPM，第一步是诊断 PWM 输入频率的范围，使指针在转速的整个圆弧上移动。使用他的 Tektronix 3252C 函数发生器，他很快确定需要 0-440 Hz，并绘制了一些中间点。响应曲线不是线性的，所以他起草了一些捏造的指导方针来使所有的数据点匹配。

接下来，他编写了几行 Python 代码(他分享了)来让 Pi 轮询它的 CPU 使用情况，并将其转换为适当的频率。Pi 使输出变得容易，GPIO 引脚 11 将信号传送到 7404 进行缓冲，然后输出到转速表。汽车转速表本身运行在 12V，但它的输入信号只需要 5V，所以他从他的零件箱拿出一个 7805。

一旦全部组装起来，只需使用一个额外的组件，它就能完美地工作。有些人可能认为这比依赖 USB 的或基于转速表的 [Arduino ~~臃肿的~~更聪明。](http://hackaday.com/2012/07/02/junkyard-scavenging-nets-a-tachometer-to-play-with/)

看到视频后，打破了 tach 抽搐，甚至当鼠标移动，并盯住红色时，打开浏览器。如果您想一目了然地看到您的 Pi 何时投入工作，就不再需要用尽宝贵的屏幕空间(或者根本不使用屏幕)。

[https://www.youtube.com/embed/iQvMupVMfOY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/iQvMupVMfOY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果你希望一个设备增加一个转速表来显示实际的转速，我们已经在之前[报道过了！](http://hackaday.com/2012/08/30/arduino-tachometer-tutorial/)