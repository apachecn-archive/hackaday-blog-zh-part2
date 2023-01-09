# 殴打西蒙

> 原文：<https://hackaday.com/2014/06/09/beating-simon/>

事实上，每个人都玩过 Simon，这款 70 年代的电子记忆游戏，但是我们当中有谁真正打败过它呢？这是[Ben]和他 7 岁女儿的目标，经过一年的工作，一个 Arduino，一些伺服系统和一些乐高积木，[他们终于做到了](http://redfrontdoor.org/blog/?p=702)。

代替原来的大 Simon，[Ben]正在使用游戏的钥匙链版本:更小，更容易建立一个设备来感知灯光和按下按钮。这些手臂由乐高积木制成，用橡皮筋支撑，由安装在砧板上的两个伺服系统驱动。

为了检测西蒙的灯光，[本]将四个光电晶体管连接到一个 Arduino 上。Arduino 记录西蒙上的灯光图案，并根据该图案激活乐高手臂。[本]版的西蒙在最后一个序列中最多只有 32 步，但这仍然意味着每场游戏需要按 528 次按钮——和许多烦人的哔哔声——才能完成。

下面的视频。

[https://www.youtube.com/embed/F3LjJITuheM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/F3LjJITuheM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/cc6d5RIc72g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/cc6d5RIc72g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/UT4fRTy327w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UT4fRTy327w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)