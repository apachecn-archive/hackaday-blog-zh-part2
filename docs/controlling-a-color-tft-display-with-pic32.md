# 用 PIC32 控制彩色 TFT 显示器

> 原文：<https://hackaday.com/2015/04/07/controlling-a-color-tft-display-with-pic32/>

有时候感觉外面所有人都在用 Arduino。很容易找到教程和库来使用 Arduino，但是如果你想使用另一个平台，你可能会有更多的麻烦。当【Tahmid】决定尝试使用 [PIC32 控制来自](http://hackaday.io/project/3279-interfacing-a-color-tft-display-with-the-pic32 "PIC32 library for a TFT display") [Adafruit](http://www.adafruit.com/product/1480 "Adafruit TFT display") 的 2.2 英寸彩色 TFT 显示屏时，他遇到了这个问题。

Adafruit 真的很擅长为他们的产品提供教程和 Arduino 库。如果你使用的是 Arduino 的话，它会让你很容易地启动和运行。他们所有的库都是开源的，这意味着社区可以根据需要获取和修改它们。[Tahmid]决定这样做，把 Adafruit 库移植到 c 语言的 PIC32 平台上，这是一次很好的学习经历。你可以看到其他人是如何编码的(好的或坏的),这让你沉浸在两个不同芯片家族之间的差异中。

他在网上发布了这些库供其他人使用。他说他对代码做了大量的注释，试图使代码尽可能不言自明。显示器通过 SPI 与 PIC32 接口。下面的演示视频显示了屏幕启动和运行，并演示了清晰的彩色图形。

[https://www.youtube.com/embed/JUHIxQL1xyQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JUHIxQL1xyQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)