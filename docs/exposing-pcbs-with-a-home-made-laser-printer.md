# 用自制激光打印机曝光多氯联苯

> 原文：<https://hackaday.com/2012/08/09/exposing-pcbs-with-a-home-made-laser-printer/>

制作自己的印刷电路板虽然有用，但却是一件痛苦的事情。使用非常流行的墨粉转移方法需要十几个步骤，必须在第一次就完美地完成，并且在 CNC 机器上铣削电路板会造成很多混乱。最勤奋的黑客能够从一台旧的喷墨打印机上组装出一台直接印刷的打印机，但是这些组装通常有点儿不完整。[Tixiv]的 [LaserExposer 电路板打印机](http://www.das-labor.org/wiki/LaserExposer)是我们看到的首批产品之一，它消除了 PCB 制造其他技术的所有负面影响，将制作自己的电路板变成了一个非常非常简单的过程。

激光曝光机使用光敏铜板，就像我们见过的许多其他 PCB 打印机一样。[Tixiv]使用 1 瓦 445 纳米蓝色激光和六角镜，直接将图稿逐行曝光到板上，而不是将图稿打印到透明胶片或蒙版上。

整个设备是围绕一个旧的平板扫描仪构建的，该扫描仪缓慢地在 PCB 上爬行，露出要蚀刻掉的铜痕迹。这需要对 90 年代激光打印机的镜面电机控制板进行逆向工程，并建立一个电路来精确控制激光的定时。[Tixiv]最终一切正常，经过蚀刻，我们拥有了一些我们见过的最专业的自制电路板。

[Tixiv]放一个他建造的演示视频(休息后，德国音频，YouTube 有字幕…)。有人有旧的平板扫描仪吗？

[https://www.youtube.com/embed/fi4P-Bwc6g8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fi4P-Bwc6g8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)