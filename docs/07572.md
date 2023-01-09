# Z80 微型电视时钟

> 原文：<https://hackaday.com/2014/11/14/a-z80-micro-tv-clock/>

作为计算机历史上的一次冒险，[Len]建造了一个时钟。Z80 微型电视时钟将一台自制电脑和三台微型电视组合成一个相当大的时钟。

驱动时钟的计算机运行 [CP/M](http://en.wikipedia.org/wiki/CP/M) 操作系统。这个操作系统最终作为开源软件发布，并且各种自制计算机项目已经实现了它。这个时钟基于现有的[试验板 CP/M 机器](http://searle.hostei.com/grant/cpm/index.html)，包括原理图和软件。

随着操作系统的运行，[Len]有了一个文本编辑器和 C 编译器。现在可以为设备编写定制软件了。编写软件以与 Maxim [DS12885](http://www.maximintegrated.com/en/products/digital/real-time-clocks/DS12885.html) 实时时钟交互，该时钟记录时间，并将时间输出到显示控制器。

这栋建筑中的微型电视是索尼 Watchman 显示器，配有一个 2 英寸的 CRT。这些设备没有视频输入端口，所以[Len]把它们拆开，开始四处查看。NTSC 信号是通过探测电路板并寻找正确的波形找到的。

为了从 CP/M 驱动电视，构建了一个自定义视频驱动程序。这使用了三个相对现代的 ATmega328P 微控制器和 [arduino-tvout](https://code.google.com/p/arduino-tvout/) 库。所有这些组件都被放在一个由木头和铜管制成的支架上，使它成为一个功能性的台式时钟