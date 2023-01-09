# 用微控制器控制电视

> 原文：<https://hackaday.com/2012/05/16/controlling-a-tv-with-a-microcontroller/>

![](img/a447cb33d98807edbdf870e2ce9c9b9c.png "twofer")

这里有两个构件，它们只用两个针脚就可以将文本打印到电视上:

#### 带着 Arduino 还活着

在看到所有播放*还活着*的构建后，【鲍勃】决定拿一个 1972 年的琥珀监视器和[在](http://www.youtube.com/watch?v=NGnu4YTLhco) *[传送门](http://www.youtube.com/watch?v=NGnu4YTLhco)结尾重现过场。*构建使用 Arduino 的 [TVout 库](http://code.google.com/p/arduino-tvout/)。同时运行 Unix 和 Alive 动画有一些问题，所以[Bob]在命令行动画的末尾翻转了一下 EEPROM，重新启动进入 GLaDOS 的报告。你可以在这里查看老式彩色显示器

#### ATMega 视频文本生成器

[Stian]认为他的身材不够好，但他的朋友[Mikael]不这么认为。【Stian】写了一个库来[实时生成 NTSC 视频信号](http://jmp.no/blog/amvtg/)。这是一个基于文本的版本，分辨率为 37×17 字符，只需要大约 3kB 的内存。作为奖励，它只占用[Stian]的 ATMega128 上的两个引脚。

休息之后，您可以查看这两个版本的视频。

[https://www.youtube.com/embed/NGnu4YTLhco?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NGnu4YTLhco?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)
[https://www.youtube.com/embed/FbCXDgIpuw8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FbCXDgIpuw8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)
[https://www.youtube.com/embed/8PU8UWDMPlY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8PU8UWDMPlY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)