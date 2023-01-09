# 1337-sp34k 键盘

> 原文：<https://hackaday.com/2015/04/14/1337-sp34k-keyboard/>

一开始只是一个快速的恶作剧，重新映射同事的键盘，后来变成了对键盘工作原理的深入理解。[ch0f]和他其他工作场所的同事有互相恶作剧的习惯。当[ch00f]的好友，一个狂热的游戏玩家和模仿蒙太奇 1337-sp34k (leet speak)的粉丝，去度假时，[ch00f]开始重新映射他朋友的键盘，让它吐出他朋友经常使用的词——“SWAG”、“YOLO”和“420”。但是软件中的重映射太简单了，他的破解是硬件重映射！

问题中的[键盘](http://www.monoprice.com/Product?p_id=9433)使用安装在键盘大小的 PCB 上的机械键。此外，它是单面的，用跳线连接代替了前侧轨道。这使得黑客攻击变得更加容易。计划是使用不常用的键——滚动锁定、打印屏幕和暂停/中断——让他们打印出单词。这三个键的信号轨迹被切掉，代之以微控制器的输出。原始连接也被路由到微控制器，一个拨动开关用于在重新映射和原始版本之间进行选择。由于缺少安装拨动开关的空间，这最终没有实现。[ch00f]如果他的朋友抱怨黑客攻击，他决定更换键盘。在 ATMega 的印刷电路板和固件上做了一点工作，他能够得到选定的键来打出斯瓦格、YOLO 和 420。

这就是一大堆麻烦出现的地方。[ch00f]深入解释手头的各种问题——键盘扫描/多路复用、开关 FET 中的体二极管如何影响扫描、重影和阻塞二极管的使用。到最后，他只是通过按下暂停/中断键激活了单词 SWAG。但他确实找到了为什么在他接入黑客程序后键盘表现奇怪的原因，这是一些有趣的阅读。休息之后不要错过黑客行动的视频。

[https://www.youtube.com/embed/ojHRFW5b6h8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ojHRFW5b6h8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)