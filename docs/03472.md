# 用 ATMegas 制造的 16 核计算机

> 原文：<https://hackaday.com/2013/06/24/16-core-computer-made-of-atmegas/>

您的台式机有两个、四个甚至八个内核，但您上次看到多核自制计算机是什么时候？[Jack] [就是这么做的](http://www.youtube.com/watch?v=S_zfjmukIGM)，用少量 ATMega 微控制器构建了 DUO Mega，一台 16 核计算机。

根据[【Jack】的描述](http://www.ostracodfiles.com/mega/menu.html)，有 15 个“工作”内核，每个内核都有自己的 16MHz 晶振，并连接到 8 位数据总线。当机器启动时，单个“管理器”内核(也是一个 ATMega328)轮询所有工作器，并将一个用自定义字节码编写的程序加载到每个内核上。内核本身可以访问共享的 RAM 池(32k)、一点闪存、一个 VGA 输出端口和一个连接到主内核的以太网控制器。

由于[杰克]的 DUO Mega 计算机有多个核心，它擅长多任务处理。在下面的视频中，你可以看到电脑在计算器应用程序、怪异的俄罗斯方块游戏和记事本应用程序之间移动。DUO Mega 中的 16 个内核也使复杂的计算速度大大加快；他生成 Mandelbrot 模式的速度比任何 8 位微控制器单独生成的速度都要快，还能在点击鼠标时生成素数。

[https://www.youtube.com/embed/S_zfjmukIGM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/S_zfjmukIGM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)