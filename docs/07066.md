# 螺旋桨上视觉时钟的持续性

> 原文：<https://hackaday.com/2014/09/14/persistence-of-vision-clock-on-a-propeller/>

如果你有一个备用的 DC 电机，一个 PIC16F84A 微控制器，和足够的耐心，那么[Jon]有一个很好的指南来建造一个[视觉持续时钟](http://www.electronixandmore.com/projects/propclock/index.html)，它一定会照亮任何房间。对于那些不熟悉这种类型的时钟的人来说，原理很简单:一个带 led 的“螺旋桨”旋转，在正确的时刻，led 打开并显示时间。

在 ( [)之前](http://hackaday.com/2014/02/27/persistence-of-vision-would-make-a-great-hud/)[我们已经报道过很多次](http://hackaday.com/2013/12/21/fubarino-contest-persistence-of-vision-clock/)视觉项目的持续性，甚至报道过【乔恩】的[旧时钟](http://hackaday.com/2009/06/13/persistence-of-vision-propeller-clock/)，但是让这个视点时钟与众不同的是项目日志的细节。[Jon]对现有项目的文档并不满意，他煞费苦心地撰写了关于他的时钟的所有内容。该项目日志经历了硬件的四个主要版本，并深入了解了软件，使任何人都可以轻松地重建这个强大的时钟。

至于时钟本身，硬件的最终版本有一个用于所有组件的 PCB，并使用 PC 风扇电机来旋转螺旋桨。电力传输消除了滑环或电刷，有利于无线电力传输，这本身就是一个令人印象深刻的壮举。的确，钟表的质量只有细节的极致才能超越！