# 外部动机:蓝牙的基础

> 原文：<https://hackaday.com/2014/09/03/extrinsic-motivation-basic-for-bluetooth/>

你在 Arduino 项目中使用的那些花哨的无线电模块远比你看到的要多。其中许多都是片上系统，配有自己的微控制器和存储器，可以控制整个闪烁 led 项目。为这些无线电模块开发是一个挑战，因为 ide 和编译器要花费几千美元。[Tim]的 Hackaday 奖参赛作品着眼于这些蓝牙 LE 模块中的一个——德州仪器的 CC2540 和 cc 2541——并将嵌入式 BASIC 解释器放在芯片上。

[Tim]这个项目的灵感来自于对一些使用 CC254X 芯片的流行设备的观察。其中许多包括微控制器和额外芯片带来的额外成本、复杂性和功耗要求。这种无线电模块可以轻松运行 ATMega 可以运行的任何代码，在产品中添加另一个芯片似乎是一种可怕的浪费，当然也不符合开放硬件和软件的精神。

另一种方法是为 CC254X 芯片编写解释程序。他选择了 BASIC，但是添加了一点 Arduino 语言语法，使得开发起来更加容易。经过几次成功的测试，包括 SPI、I2C 和 1 线设备，[Tim]已经有了一个工作的基本系统，但[Tim]承认它确实需要一点修改，以使它更容易使用。

这是一个伟大的项目，个人感到惊讶的是，它没有进入 Hackaday 奖的四分之一决赛。[Tim]仍然在做他的项目，这是外在激励的一个很好的例子；他不需要去太空旅行来说服他建造一些很酷的东西。

你可以看看下面[Tim]的两分钟概念视频。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png)这个项目是[正式进入](http://hackaday.io/submissions/prize/list)hack aday 奖，遗憾的是[没有进入四分之一决赛选择](http://hackaday.io/list/2864-The-Hackaday-Prize%3A-Semifinalists)。这仍然是一个伟大的项目，它本身就值得在 Hackaday 上发表。

[https://www.youtube.com/embed/gd_tHgKUJbI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gd_tHgKUJbI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)