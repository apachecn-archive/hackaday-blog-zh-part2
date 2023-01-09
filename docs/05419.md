# 自制相位激光测距仪

> 原文：<https://hackaday.com/2014/02/28/homebrew-phase-laser-rangefinder/>

就在你认为 ARM micros 不能再酷了的时候，另一个项目出现了，让你大吃一惊。【伊利亚】[创造了相位激光测距仪](http://habrahabr.ru/post/213749/)(。ru，[Google translate tron](http://translate.google.com/translate?sl=ru&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fhabrahabr.ru%2Fpost%2F213749%2F&act=url))只用了一个激光二极管、一副放大镜、一些元件和一个 STM32F4 发现开发板。

该建筑背后的理论是利用激光的相位来确定物体的距离。通过将激光二极管的输出调制到几百 Mhz，可以比较来自激光的反射，给出目标距离的相当合理的估计。这种方法有一些缺点；一旦反射的相位差超过 360 度，距离就会“绕回”到探测器的正前方。

当然，所用的激光二极管没有任何调制，但通过使用 STM32F4 ARM 芯片，[Ilia]能够在从 74HC04 芯片和几个电阻砍出的驱动板的帮助下调制激光的振幅。不理想，但很管用。

该装置的接收器使用光电二极管向同一微控制器供电。凭借令人印象深刻的 DMA 和 PLL 魔法(你知道，STM32F4 真的很酷)，可以比较传输和反射的相位，从而进行距离测量。

这是一个令人印象深刻的工作量，包括一套拼凑的光学系统、一个廉价的开发板和一些组件。对于机器人或传感器套件中的任何一种应用，这个项目都会失败。作为相位激光测距理论的一个示范，它的顶尖水平。

你可以看看下面[伊利亚]的测距仪的视频。一定要全屏显示，并检查 LCD 上的距离测量值。令人印象深刻。

Thanks [Володимир] for the link.

[https://www.youtube.com/embed/TGT65tKHEMk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TGT65tKHEMk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)