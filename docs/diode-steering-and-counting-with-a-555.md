# 用 555 实现二极管控制和计数

> 原文：<https://hackaday.com/2015/02/25/diode-steering-and-counting-with-a-555/>

虽然你不太可能看到这种技术在今天被广泛使用，但用 555、一些逻辑芯片和一些二极管，你可以做很多事情。[Fran]在这里提供了一个很好的例子，使用这些简单的部件来构建一个从零开始计数的电路。

[Fran]的灵感来自于[[Dave]的一个邮袋](https://www.youtube.com/watch?v=4hHPeNIU6ls)和[Colin Mitchell]的[555 电路书](http://www.talkingelectronics.com/projects/50%20-%20555%20Circuits/50%20-%20555%20Circuits.html)中的一个。555 是*在每个零件抽屉里都能找到的*标准组件，但由于我们有微型微控制器，价格与 555 相同，我们现在很少看到简单的定时器芯片和几个逻辑芯片的艺术性。

这个电路从一个 555 连接到一个 4017B 十进制计数器开始。仅仅通过在 4017 的输出端绑上几个 led，[Fran]就让一束 led 按顺序亮了起来。很酷，但没什么意外。真正的技巧是使用几个二极管和六个 led 来构建一个扫描仪——一排 led 将从左到右闪烁，然后从右到左闪烁。令人印象深刻，再多一点电路，这就是拉森扫描仪，正如《太空堡垒卡拉狄加》和《霹雳游侠》中所见。

当[Fran]拿出一块原型板、几十个二极管和七个旧晶体管来实现从 0 到 9 的七段显示计数时，这种技术的真正诀窍就来了。4017 只需在十个引脚上计数，每个引脚都连接到显示器每个部分的一组二极管。加上几个电阻和一个晶体管，[Fran]用分立元件复制了一个七段驱动器。

如果数到零还不足以证明你可以用一些二极管和逻辑芯片做很多事情，[用一个](http://hackaday.com/2014/06/26/homebrew-programming-with-diodes/)给 Atari 2600 编程怎么样？

下面视频。

[https://www.youtube.com/embed/JNbDdnEpAOQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JNbDdnEpAOQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)