# 带开关和闪光灯的 Z80 电脑

> 原文：<https://hackaday.com/2014/12/01/a-z80-computer-with-switches-and-blinkenlights/>

虽然大多数用芯片制造自己的计算机的人都希望成品能做些有用的事情，但对于一大堆开关和一束闪光灯还是有一些可说的。它们非常简单——大多数情况下，你甚至不需要 RAM——而且外观经典。

[Jim]想造一台这样的电脑，结果[创造了一个带有开关和闪光灯的最小系统](https://github.com/jmacarthur/zeta256)。它基于 Z80 CPU，只有 256 字节的内存，其他没有多少。除了几个额外的芯片输出数据和地址线到发光二极管，还有几个读取开关，这台电脑里只有两个主要的芯片。

随着电路的完成，[Jim] laser 切割了一个足够大的小外壳，以容纳他的条形板 PCB、开关和 led 以及几个按钮，以写入地址，执行软复位，并循环时钟。这种开关/闪光灯设置的最实用的附加物之一是一个*手动曲柄*。这台电脑内部没有水晶，所有的时钟周期都是手动完成的。而不是按几百次按钮来计算什么。[Jim]增加了一个小手摇柄，每转一周时钟循环一次。疯狂，但奇怪的是实用。

[Jim]制作了一个演示视频，展示了他的计算机如何计算两个数字的最大公约数。你可以看看下面的视频。

[https://www.youtube.com/embed/0GmY_UrbXnA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0GmY_UrbXnA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)