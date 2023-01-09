# 漫游六足动物耗尽了 3D 打印

> 原文：<https://hackaday.com/2013/12/30/geoweaver-rise-of-the-monster-3d-printing-hexapods/>

旧金山加州艺术学院(CCA)的学生[吴佳、玛丽·塞克和杰夫·前原诚司]承担了开发行走 3D 打印机的任务。[结果是 Geoweaver](http://www.instructables.com/id/Geoweaver-Walking-3D-Printing-Hexapod/) ，一个带有胶枪挤压系统的六足机器人。Hackaday 以前见过[行走的数控机器](http://hackaday.com/2008/06/11/hexapod-cnc-bot/)，但不是 3D 打印机。Geoweaver 在它的六条腿上各使用两个伺服系统来穿越陆地。该团队能够将几个步态编程到机器人中，使其能够穿越不平坦的地形。行走本身已经够难了，但 Geoweaver 还使用基于胶枪的挤出机来制作 3D 打印品。挤出机机头使用两个伺服系统在半球形弧内摆动。弧形在软件中被映射到一个平坦的~~平面~~，允许机器人准确地将一团胶水滴到它被编程的地方。Geoweaver 不包括太多的机载处理方式 Arduino Uno 用于驱动 15 个伺服系统。这些伺服系统与胶枪式加热器相结合，产生了相当大的功率，这为 Geoweaver 赢得了诸如伺服黑仔、盾牌的食客、电线的熔化者和监管者的破坏者等绰号。

Geoweaver 的印刷品可能还没什么好看的，但是重要的是要记住，这个机器人的未来愿景之一是在全球范围内印刷。Geoweaver 目前使用[react vision](http://reactivision.sourceforge.net/)通过“天空之眼”提供计算机控制。ReacTIVision 跟踪机器人上的基准标记，并将其应用于地形的地形图。这使得 Geoweaver 可以根据打印地面的平整度来改变其高度和打印参数。在按比例放大的 Geoweaver 上，reacTIVision 将被 GPS 或类似的卫星导航系统取代。Geoweaver 中使用的大部分软件都是开源的，包括团队教授编写的 [Grasshopper](http://www.grasshopper3d.com/) 和 [Firefly、](http://fireflyexperiments.com/)、Jason Kelly Johnson 。例外的是[犀牛 5](http://www.rhino3d.com/) 。我们希望看到一个免费或开源的替代方案，为我们自己的 Geoweaver 提供大约 1000 美元的软件。

[https://www.youtube.com/embed/FHnaLbghZ1o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FHnaLbghZ1o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)