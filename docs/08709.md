# DIY 七段显示器

> 原文：<https://hackaday.com/2015/04/04/diy-seven-segment-displays/>

[Esai]想从零开始造一个电子钟。这是一个崇高的追求，但普通的七段显示器就是如此——极其普通。不同于那些可以从普通零售商那里以一美元一个的价格买到的显示器，[Esai] [在一些 perfboard](http://blog.esai.pw/2015/04/an-smd-4-digit-7-segment-diy-display.html) 上制作了他自己的四位数、七段显示器。

在将 58 个 SMD LEDs 焊接到 perfboard 的一个小矩形之前，[Esai]用一个标记描绘出每一段。每个部分由两个 led 组成，它们都用 30 号线连接到适合试验板的引脚接头。

每个段连接成 LED 矩阵中的一列，每个数字为一行。这是一个简单的设计，但板上没有任何电阻。希望[Esai]将在这个显示器上使用合适的 LED 驱动程序；你真的不希望 led 在 1:11 一天烧坏两次。