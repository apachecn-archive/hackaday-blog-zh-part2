# 如何逆向工程，以 Rigol DS1054Z 为特色

> 原文：<https://hackaday.com/2014/10/22/how-to-reverse-engineer-featuring-the-rigol-ds1054z/>

几年来，Rigol DS1052E 一直是我的第一台非官方示波器。它很便宜，对大多数项目来说已经足够好了，而且已经有很多黑客和 mods 为这个非常受欢迎的 scope 提供了两倍的带宽和其他有趣的工具。1052E 有点老了，Rigol 刚刚发布了期待已久的更新产品 DS1054Z。这是一个四通道示波器，有更大的屏幕，更多的铃铛和哨子，而且*只比六年前的 1052E 贵 50 美元。*基本上，如果你想买一个便宜、可用的示波器，把 52E 从你的单子上划掉，用 54Z 代替。

有了四个输入通道，[达夫·琼斯]想知道 Rigol 的工程师如何设法在满足 400 美元的神奇价位的同时，将两个额外的前端塞进示波器。这意味着[戴夫]是时候对 1054 z 进行逆向工程了，让互联网上的每个人都见识一下一个真正的工程师是如何撕裂其他工程师的价值的。

主板从外壳中取出后,[Dave]做的第一件事就是给主板的两面拍一张漂亮、清晰、对焦的照片。这些图片经过编辑，变成线条画，并打印在透明纸上。这样，可以同时查看电路板的两面，允许使用几个干擦标记来突出显示走线和信号。

除非你在逆向工程的海洋中航行，把你带到绝望之岛，拆下单个元件，否则你只能测量电路中单个元件的价值。为此，您需要在电表上安装一个低压欧姆功能；如果你在一个元件上施加太多的电压，你可能会打开电路中的一些硅，你的测量结果将会是垃圾。幸运的是，[Dave]展示了一种方法来测试您的仪表是否适合这种工作；你需要另一个仪表。

接下来，主要是查看数据手册并绘制电路原理图；输入在左侧，输出在右侧，地在底部，正供电轨在顶部。这比听起来要难——大多数[戴夫]在这方面的专业知识只是模式识别。通过暴力对电路进行逆向工程是一回事，但知道电路工作的原因和方式会让事情变得容易得多。

[https://www.youtube.com/embed/lJVrTV_BeGg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/lJVrTV_BeGg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/kb9P1Am9aFU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kb9P1Am9aFU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)