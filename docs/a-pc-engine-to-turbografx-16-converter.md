# 涡轮 Grafx-16 飞机的个人计算机发动机

> 原文：<https://hackaday.com/2014/10/10/a-pc-engine-to-turbografx-16-converter/>

个人电脑引擎在日本相当受欢迎，但只有美国最酷的孩子才有美国版的 TurboGrafx16。这两个系统并不完全相同。TurboGrafx-16 的数据总线被翻转，因此游戏不兼容，美国游戏有区域锁定。[Kaz]查看了现有的在美国系统上运行日本游戏的黑客，每一个都需要修改控制台。他认为自己可以做得更好，于是发明了 PC-Henshin T1，这是一个适配器和 CPLD，可以让日本游戏在美国游戏机上运行。

为了防止美国和日本型号的 PC 卡连接器上的线路混淆，我们提供了一些适配卡。这很好，但它们只解决了兼容性问题的一部分。几乎每个美国游戏中都有区域锁定程序，这意味着 PC 引擎控制台不能运行 TurboGrafx-16 游戏。[Kaz]使用了一个小而便宜的 CPLD 来读取数据总线，在读取时修补所有东西，并将日本游戏机变成可以玩美国游戏的东西。

下面视频。

 [https://www.youtube.com/embed/LTJBBTdZmUI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LTJBBTdZmUI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)