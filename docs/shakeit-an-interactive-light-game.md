# ShakeIt——一款互动轻游戏

> 原文：<https://hackaday.com/2015/06/03/shakeit-an-interactive-light-game/>

当你让学习变得有趣、互动和娱乐时，学习就变得有趣了。[Arkadi]制作了[shake it——一款互动游戏](https://hackaday.io/project/6039-shakeit),为耶路撒冷的迷你 MakerFaire 制作，向孩子们和成年人演示如何混合浅色。这是他早期项目的后续——[智能杂耍球](http://hackaday.com/2015/04/28/smart-juggling-balls/),我们之前已经介绍过了。

杂耍球由一个 6 自由度传感器(MPU 6050)、一个微控制器、发射器(NRF24L01+)、一些可寻址的 RGB LED 和一个 LiPo 电池组成。一个外部磁铁激活球内的簧片开关，触发它们动作。ShakeIt 灯具由 Arduino Nano 克隆、带 SMA 天线的 NRF24L01+、降压转换器、74 个可寻址 RGB LED 和蓝牙模块组成。蓝牙模块连接到智能手机应用程序。

[Arkadi]从递三个杂耍球开始，每个球都有预先定义的颜色(红色、绿色、蓝色)。当球被摇动时，球内的光变得更强。ShakeIt 灯具被用作混音器。它与球通信，接收每个智能球内部的光强度值，将它们混合，并生成混合颜色。

当互动游戏模式启用时，乐趣就开始了。这种灯具不只是混合光线，而是根据球被摇动的力度来产生图案。首先，灯具显示所有三种颜色充满了中间的球。然后，三个竞争者奋力争取让他们的颜色完全填满球体，直到只剩下一种颜色，并宣布获胜者。

孩子们可能会在这里学习一些色彩理论，但似乎成年人正在玩一个疯狂的游戏。如果你想开发自己的肩膀脱臼 ShakeIt 游戏，可以去[Arkadi]的 github 仓库找 [ShakeIt](https://github.com/arkadiraf/ShakeIt_Public) 和[杂耍球](https://github.com/arkadiraf/Juggling_Balls_Public)。查看下面的视频，看看成年人玩得开心。

[https://www.youtube.com/embed/ivLrFQcIt5U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ivLrFQcIt5U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)