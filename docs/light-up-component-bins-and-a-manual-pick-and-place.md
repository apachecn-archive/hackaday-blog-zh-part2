# 点亮元件箱和手动取放

> 原文：<https://hackaday.com/2014/11/05/light-up-component-bins-and-a-manual-pick-and-place/>

[迈克]制造一些非常小众的乐器，他正在考虑的生产量意味着没有必要将他的组装外包出去。这意味着一切都要手工完成，包括从箱子里挑选电阻和其他元件的烦人任务。在寻找一种加速组装过程的方法后，[他发明了自动填充器](http://mikebeauchamp.com/2014/11/stuffomatic-manual-pick-and-place/)，一种按下按钮就能定位正确部件的装置。

组装时抓取零件的正常方式是读取板上的参考，交叉参考 BOM 上的值，并从箱子中找出正确的零件。为了加快速度，[Mike]将 led 灯放在每个零件箱中，连接到一个将 BOM 存储在内存中的 Teensy 2.0。单击脚踏开关查找下一个组件，并点亮相关零件箱中的 LED。

[Mike]说这项发明将他的组装时间加快了大约 30%,如果你想花几个小时来组装一个单元，这是一个很大的进步。

如果你想知道[迈克]到底在组装什么，[看看这个](http://therevox.com/)。它深受 Ondes Martenot 的启发，这是一种与特雷门琴一样古老的电子乐器，但却比它酷一百万倍。下面的视频样本。

[https://www.youtube.com/embed/P4RU5Q2nx4Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/P4RU5Q2nx4Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)