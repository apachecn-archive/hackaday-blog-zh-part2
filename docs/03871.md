# 液氮(最终)让 Arduino 项目变得很酷

> 原文：<https://hackaday.com/2013/08/18/liquid-nitrogen-finally-makes-an-arduino-project-cool/>

在莫斯科 1.5 美元一升的价格下，[米恰伊尔]忍不住为自己买了一些液氮。他认为，因为 Arduinos 在极客中非常受欢迎，所以他会尝试在将温度降至-196°C/-320°f 的同时对一台进行超频。

为了检查 ATmega 是否还能正常工作，[米恰伊尔]设计了几个稳定性测试:SRAM 读/写、闪存读、算术数学和程序流测试(代码带有一些条件)。他使用了标准的 HD44780 LCD 来查看测试结果，还使用了 LED，闪烁测试失败的数字。Arduino 由他设计的基于 TTL 逻辑的方波信号发生器进行外部时钟控制，可以产生 16 到 100MHz 的时钟。原来用液氮冷却就可以运行一个 65.3MHz 的 Arduino！

[米恰伊尔]的文章还解释了使用 LN2 冷却时不同的板上元件会发生什么:电解电容几乎不存在，X7R 电容的阻抗下降了 2/3，硅二极管的压降增加了 50%，led 的颜色发生了变化。看看下面的视频:

[https://www.youtube.com/embed/KVRvWmcxnA0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KVRvWmcxnA0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)