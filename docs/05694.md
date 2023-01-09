# 用 3D 打印机分配焊膏

> 原文：<https://hackaday.com/2014/04/02/dispensing-solder-paste-with-a-3d-printer/>

在制造几块电路板时，PCB 生产中有一个奇怪的中间地带。用注射器或牙签将焊锡膏涂在一块电路板上很容易，但是当粘贴一把电路板时，这种方法会令人厌烦。当你制作几十或几百块电路板时，焊膏模板可以加快制作过程，但是只为几块电路板制作一个模板是一种浪费。当然，这个奇怪的中间地带的解决方案是[改装一台 3D 打印机来分发焊膏](https://www.youtube.com/watch?v=tgXtRDVvhdU)。

这个项目是[Jake]和[hzeller]之间的合作，将 KiCAD 文件转换成 g 代码，以便将焊膏直接分配到电路板上。他们使用的机器是一台[A 型机器打印机](http://www.typeamachines.com/)，用锡膏分配器代替了挤压机。分配器连接到控制板的风扇输出端，从视频来看，他们得到了非常好的结果，这仍然是非常实验性的。

所有将 KiCAD 文件转换成 g 代码的代码都在[【hzeller】的 github](https://github.com/hzeller/rpt2paste) 上。如果你想知道，他们正在粘贴的板是[一个名为 Bumps 的 BeagleBone](https://github.com/hzeller/bumps) 的步进驱动板。

下面的视频。

[https://www.youtube.com/embed/tgXtRDVvhdU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tgXtRDVvhdU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/9D8YfNfAQOE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9D8YfNfAQOE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)