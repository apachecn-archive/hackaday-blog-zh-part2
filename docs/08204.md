# 基于无绳电钻电池的应急电源

> 原文：<https://hackaday.com/2015/01/31/emergency-power-based-on-cordless-drill-batteries/>

[唐·爱德华多]在经历了家中长达一天的停电后，自己动手解决了问题。就像我们大多数人至少做过一次一样，在这个过程中，他在一个监管机构上吃了苦头。这是因为[他设计了一种使用电动工具电池作为应急电源的方法](https://www.youtube.com/watch?v=UAl8MGOWlw0)——他的电路基于一个 7812 线性稳压器，它很快就变得滚烫。

他的下一个自学项目将他带入了开关模式降压转换器的领域([如果不熟悉，可以了解一下这些](http://hackaday.com/2015/01/24/a-primer-on-buck-and-boost-converters/))。该器件将约 18V 输出降压至 12V，适用于汽车或船舶设备。我们真的很喜欢看到他提出的与电池接口的不同解决方案，这些电池有一个 U 形插脚，在相对的两侧有触点。

最后一次迭代，如上图所示，在降压转换器上构建一个纸牌搭建的房子。在将电压下调至 12V 后，他将输出输入一个“点烟器”式的逆变器，以升压至 110V 交流电。硬件装在一个废弃的电池充电器里，适当的三脚插座挂在后面。我们认为这是一个很好的接触，包括电池水平的 LED 反馈。

我们想听听你对这项技术的看法。有没有更好的方法像这种方法一样简单和适应性强(你不必改变你正在供电的设备)？

[https://www.youtube.com/embed/UAl8MGOWlw0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UAl8MGOWlw0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)