# 构建 PWM 调光器的简单或困难方法

> 原文：<https://hackaday.com/2013/09/15/the-easy-or-hard-way-to-build-a-pwm-dimmer/>

根据您从 Hackaday 多年来庞大的构建和项目库中收集的信息，实现 PWM 的唯一方法是使用微控制器、一些代码、成熟的 IDE，甚至是实时操作系统。我们确信，对于一些读者来说，这是自然而然的事情，有了一个令人敬畏的工具链，就像拧上一个灯泡一样简单。当然，有一种更简单的方法。

[Jestin]需要改变 12 伏小负载上的电流。他没有挖掘出一个 in 系统程序员，而是转向了经典的 555 芯片。使用单个电位计，很容易改变 555 的占空比，并将其连接到 MOSFET。在那里放一个负载，你就有了一个非常简单的电路，这是一个全功能的 PWM 调光器。

如果你的抽屉里只有一些碎片，这是一个非常非常简单的调光开关的设置方法。我们也很喜欢[Jestin]的即兴铝管围栏，如下面的视频所示。

[https://www.youtube.com/embed/JJ-Kus7d57A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JJ-Kus7d57A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)