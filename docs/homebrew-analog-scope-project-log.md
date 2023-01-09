# 自制模拟范围项目日志

> 原文：<https://hackaday.com/2015/09/01/homebrew-analog-scope-project-log/>

[GK]有一些旧的阴极射线管，所以很自然地他决定用其中的一个做一个老式的模拟示波器。幸运的是，[他一直在记录他的进步](http://www.eevblog.com/forum/projects/designed-a-cro-in-spice/)。由于这是一个需要解决的大项目，他开始用 Spice 建模来计算所有正确的值。

原型电源需要一些定制的变压器绕组，但完成后，电源完成了工作。虽然他仍然在 Z(强度)轴上布线，但示波器已经能够显示信号，甚至使用他之前建造的字符生成器显示文本字符(见下面的视频)。

[GK]花了大部分时间谈论高压电源设计。对于他手头上的特殊电子管，他需要+200 伏、-400 伏、-550 伏和 6.3 伏交流电用于 CRT 加热器。这肯定不是典型的基于 Arduino 的数字示波器，每个人都至少构建一次。

我们喜欢用于[艺术项目](http://hackaday.com/2014/12/13/tripping-on-oscilloshrooms-with-an-analog-scope/)、[逻辑分析仪转换](http://hackaday.com/2014/04/09/turning-an-analog-scope-into-a-logic-analyzer/)和[游戏](http://hackaday.com/2014/12/29/ultimate-oscilloscope-hack-quake-in-realtime/)的模拟示波器。当然，如果你的零件箱里没有旧的 CRT，你可以考虑试试激光。

[https://www.youtube.com/embed/4xtjVeDzo54?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4xtjVeDzo54?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)