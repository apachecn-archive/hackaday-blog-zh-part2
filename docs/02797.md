# 无线烟花控制器包括几个安全功能

> 原文：<https://hackaday.com/2013/02/18/wireless-fireworks-controller-includes-several-safety-features/>

克雷格·特纳写信告诉我们他刚刚完成的无线烟花控制器 T1。它总共有八个频道，并提供我们在处理爆炸物时希望看到的那种安全功能。

上面的图片详细描述了项目的启动方。项目箱内有一个由 9V 电池供电的 Arduino。要启用此基站，必须插入位于投影盒顶部的按键，并将其转到 on 位置。左侧是 12V 电池，用于通过一组八个继电器为点火器供电。在休息后的演示视频中，[克雷格]正在使用镍铬合金线进行演示，但我们甚至看到了实际上烧掉电阻器来点燃烟花的[项目。](http://hackaday.com/2012/07/04/a-resistors-fiery-death-used-to-launch-fireworks/)

系统使用 RF12 无线模块与控制面板通信。它也有一个 Arduino 和一个数字键盘。接通电源后，操作者必须输入 PIN 码，系统才会允许任何烟火发射。

[https://www.youtube.com/embed/LdICz38Yft4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LdICz38Yft4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)