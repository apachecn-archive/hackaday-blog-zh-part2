# 像 MS Paint 一样使用俄罗斯方块

> 原文：<https://hackaday.com/2014/11/08/using-tetris-like-ms-paint/>

在这张像素化的图片中，看看萨姆斯看起来像个老板。谁会想到用俄罗斯方块作为这类图形的画布呢？想出战略性地清除并留下俄罗斯方块碎片的原始想法，以上面显示的内容结束，已经足够困难了。但是你究竟如何[实现以编程方式](http://meatfighter.com/tetrisprinteralgorithm/)生成这个的算法呢？

首先，有两件事并不令人惊讶。它不是在正常游戏中手动生成的。那将超出专家的水平。另一件要注意的事情是，棋子出现的顺序不是随机的，而是由算法有策略地计算出来的。挑战不仅在于占据和清除正确的像素，还在于确保保留正确着色的部分。

您需要在休息后观看嵌入的快动作视频，以充分欣赏工作中的编码杰作。我们不会试图解释算法是如何工作的，但会对上面的链接感到舒服，这个链接贯穿了所有的理论(除了提供代码以便您可以自己尝试)。

[https://www.youtube.com/embed/PJkHwulsac4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PJkHwulsac4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](https://www.reddit.com/r/geek/comments/2lkxn1/algorithm_that_can_make_8bit_characters_in_tetris/)