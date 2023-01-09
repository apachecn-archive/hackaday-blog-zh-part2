# 活的静物

> 原文：<https://hackaday.com/2015/06/14/the-live-still-life/>

这个项目将艺术家[Justus Bruns]和工程师[Rishi Bhatnagar]以及[Michel Jansen]聚集在一起，合作创作一件互动艺术作品。 [Live Still Life](https://medium.com/@justusbruns/still-live-project-6177d9530bc3#1ee3) 是一幅经典的静物，从印度向世界任何地方直播。这是创建艺术工厂的第一步，数百件这样的作品将在这里制作、保存和流动。

生活静物是一个物理组成的新鲜水果和蔬菜展示在一张桌子上，餐具，餐具和其他静止的物体。这是在班加罗尔的一个木箱里。每一分钟都有一张照片被拍摄下来，图像被实时流式传输，可以从世界上的任何地方即时访问。Les Oiseaux de Merde 的印度策展人随时待命，在水果开始腐烂的那一刻就更换水果，以保持图像的完整性。这样，虽然图像保持不变，但与腐烂的斗争始终存在。点击此链接可以观看[的直播。](http://livestill.oiseauxdemerde.com/)

硬件非常少。一个联网的 Raspberry Pi model B，Raspberry Pi 相机模块，一个用于照明的台灯和一个木制外壳来容纳所有这些，包括艺术品。让相机工作只是 Python 中的几行代码。现场直播拍摄照片比他们预期的要多花很多时间。该服务器是使用一个名为 [Exprestify](https://github.com/ajithnn/exprestify) 的模块编写的，该模块是在 Express JS 之上编写的，以便于实现更简单的 RESTful 函数。对于一些看起来简单明了的东西，团队必须克服几个编码挑战，所以如果你想深入研究代码，一些代码托管在 [Github](https://github.com/workbenchprojects/Raspberry-Pi-Builds) 上，或者你可以[问【Rishi】](https://medium.com/@rishigb/how-i-built-live-still-life-c993100daef7)，因为他仍然需要清理相当多的代码。