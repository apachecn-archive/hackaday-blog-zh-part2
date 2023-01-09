# 我们看到 Arduino 的谢妮模块只是时间问题

> 原文：<https://hackaday.com/2012/09/09/it-was-only-a-matter-of-time-before-we-saw-nixie-modules-for-the-arduino/>

![](img/387a39691e9ae8cb92a983de07d41207.png "nixie")

数码管是一种充满氖的管子，有一系列 10 个形状像数字的阴极，是任何想要独特、复古或蒸汽朋克美学的建筑的经典展示。我们不应该对中国的一家工厂正在生产与 Arduino 兼容的谢妮模块感到惊讶，但事实就是如此。

这些模块基于能够显示数字 0 到 9 的 QS30-1 数码管，并在管子后面包括一个 RGB LED，用于一些漂亮的额外照明。根据[手册](http://www.dfrobot.com/image/data/DFR0206/NIXIE_Module_QS30-1_User_Manual_v1.0.0_EN.pdf)，模块本身基于一对 74HC595 移位寄存器，并且是“可堆叠的”通过向一对引脚施加 12 伏电压，并将另外 5 根线连接到 Arduino，就可以驱动您想要的任意多个谢妮模块。

[保罗·克雷文]得到了这些模块的四重奏，并计划作为个人项目建造一个蒸汽朋克风格的闹钟。[Paul]能够相当快地启动并运行模块，正如休息后看到的那样。

虽然它们肯定不是最便宜的选择，但如果你计划用 Nixies 构建，这可能是获得 vintagey、steampunkey 数字显示的最简单的方式。

[https://www.youtube.com/embed/uNjAUwL48hw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uNjAUwL48hw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)