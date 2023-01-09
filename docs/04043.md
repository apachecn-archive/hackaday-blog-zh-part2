# 本周失败:制造锯齿边缘的激光切割机

> 原文：<https://hackaday.com/2013/09/12/fail-of-the-week-laser-cutter-that-makes-jagged-edges/>

本周的失败仅仅是一次失败，因为埃拉布对自己的标准。上图中的设备是一台用 DVD 驱动部件制成的激光切割机。它超越了我们在这里看到的大多数光驱 CNC 项目——它实际上进行切割！但是[eLabz]认为这是一个失败，因为[驱动电机的步骤在那些切口](http://elabz.com/diy-cnc-laser-cutting-fail/)中可以看到锯齿状的边缘。我们更多地把这看作是在进行下一次细化之前开发过程中的一个暂停点。

首先，仔细观察左边的组件。这是负责 X 轴和一个非常敏锐的眼睛会注意到有两套 DVD 镜头雪橇堆叠在另一个顶部。这种设计允许激光传播两倍的距离(在这种特殊情况下高达 3 英寸)。这里有一个渲染视频，是为了在构建它之前帮助想象它是如何工作的:

[https://www.youtube.com/embed/1O8mx5rlVZw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1O8mx5rlVZw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

你不得不承认这很可爱！但是渲染什么都不是，它其实也是存在的。双 x 轴和单 y 轴都用于移动激光二极管，这意味着工件是静止的。[eLabz]提到他认为这是一个问题，因为系统中存在一些问题。除此之外，他运行的测试件清楚地显示了电机每一步的运行点。这条线是锯齿状的，但用步进电机应该有可能有更好的分辨率。对吗？

那么你认为他错在哪里？回想起来，他认为他不应该使用 DVD 零件，因为公差不在他需要的地方。但他已经走了这么远，我们想知道你会如何做额外的努力来实现尽可能平滑的切割。请在下面留下评论，加入讨论。

但首先，看看一个串联 x 轴雪橇运行的特写视频:

[https://www.youtube.com/embed/cZHflD_73NU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/cZHflD_73NU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**