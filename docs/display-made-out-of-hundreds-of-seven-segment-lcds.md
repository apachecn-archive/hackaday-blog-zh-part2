# 由数百个七段发光二极管组成的显示器

> 原文：<https://hackaday.com/2012/03/30/display-made-out-of-hundreds-of-seven-segment-lcds/>

![](img/b696c2b3dfd5bb4102092bc7cec400fb.png "digit")

虽然巨大的 LED 面板对于想要展示其工程肌肉的人来说是一个相对常见的项目，但我们对[Skot9000]由七段显示器组成的[巨大 LED 显示器的纯粹之美感到惊讶。他称这个建筑为数字网格，这是一个我们从未见过的奇妙展示。](http://www.skot9000.com/digitgrid/)

为了构建基于七段 led 的显示器，[Skot]在设计 DigitGrid 时采用了模块化方法。为了给所有这些七段显示器供电和控制，[Skot]使用德州仪器 TLC5920 作为一个模块运行四个 4 位显示器。这些模块中的四个连接在一起形成一行 32×2 的数字，八行数字组合在一起形成 512 位的显示器。每个数字有七个 led，整个面板有 ~~3，584~~ 4，096 个 led。

为了给这个巨大的 LED 显示器阵列供电和控制，每一行都使用 PIC16F 微控制器，该微控制器又由 FPGA 控制。写了几个小时的 Verilog 后，[Skot]有了一个相当不错的软件，可以从他的电脑上发送帧到显示器上。结果，很简单，是惊人的。[Skot]设法制作了一个短片，展示他的新显示器的动画功能，这是一个奇迹。休息之后你可以看看那个视频。

[https://www.youtube.com/embed/FP6xWrKVqo4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FP6xWrKVqo4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)