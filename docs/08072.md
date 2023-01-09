# 全面的 SHTTTRRR 控制让您从容不迫…

> 原文：<https://hackaday.com/2015/01/15/full-shtttrrr-control-lets-you-take-your-time/>

[Glitchmaker]热爱摄影，写信告诉我们他的最新项目。他有一台佳能 1000D 相机，但不幸的是，它没有定时功能。因此，[Glitchmaker]决定制造一种外部快门控制设备，可以继续指示相机以预定的时间间隔拍照，而不是花一大笔钱买一台新相机。他称他的项目为: [SHTTTRRR](http://hackaday.io/project/3812-shtttrrr) 。你不会认为那是别的意思吧？

你可以看到上面那个不起眼的盒子，里面装的东西刚好够完成工作，没有多余或花哨的东西。幸运的是，Cannon 相机有一个远程快门输入插孔，只需要将一个引脚连接到另一个引脚就可以拍照。盒子里面是一个 ATTINY45 微控制器。它从安装在单个面板上的按钮读取按钮按压次数，并计算两次按钮按压之间的时间。按下按钮之间的时间决定了拍摄照片的频率。在适当的时候，ATTINY45 向晶体管发出信号，连接相机遥控快门输入插孔上的两个适当的引脚。该设备继续告诉相机拍照，直到它被关闭。结果是一系列延时拍摄的照片，这在以前是不可能的！

这是一个简单的项目，解决了问题，完成了工作。还有比这更好的吗？[Glitchmaker]为他所做的 SHTTTRRR 感到自豪，同时也学到了很多关于编程 ATTINY45 的知识。休息过后，请观看一段视频。

[https://www.youtube.com/embed/F44ADg96gY4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/F44ADg96gY4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)