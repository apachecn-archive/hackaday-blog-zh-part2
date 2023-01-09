# 唱歌的南瓜

> 原文：<https://hackaday.com/2012/10/15/singing-pumpkins/>

![](img/ab06d9b3da574781bc4df02772029a15.png "animatronic-pumpkins")

这张[万圣节桌子会唱一首甜美的小夜曲来惊吓你的客人](http://www.minioncity.com/2012/10/14/diy-animatronic-pumpkins-or-fondly-know-as-jack-o-and-the-lanterns/)。每个电子南瓜都很容易制作，但你可能会花更多的时间来设计表演。

在每个南瓜灯里面，你会发现一个定制的 Arduino 兼容板，叫做迷你板。这些包括无线连接，让系统与播放音频的计算机同步。南瓜是假的，这意味着可以年复一年地重复使用(不像真正的南瓜里的 LED 矩阵)。嘴巴用一小段弯曲的金属线连接到一个伺服系统上，让它随着歌词摆动。休息之后，您可以在剪辑中看到《捉鬼敢死队》主题的表演。

用 C#编写了一个自定义 GUI 来帮助编排。它处理歌曲的回放，有几个按钮可以用来记录灯光和嘴部效果。这个“录音”然后被用来在表演中驱动南瓜。

[https://www.youtube.com/embed/NoVVE3ty5Y8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NoVVE3ty5Y8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)