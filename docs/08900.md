# 向不可调节熨斗添加 PID 控制

> 原文：<https://hackaday.com/2015/04/28/adding-pid-control-to-a-non-adjustable-iron/>

还记得你的第一个烙铁吗？我们有。它插在墙上，没有办法调节温度。大多数人把这种熨斗称为“引火物”它们不仅潜在地不安全(主要是因为它们附带的支架不够),而且很难使用，加热缓慢，你永远不知道你在什么温度下焊接。

[Mike Doughty]想知道你是否可以用便宜的熨斗来控制温度。他首先拆开一个熨斗，在玻璃纤维套管的帮助下，在云母加热元件上增加一个 K 型热电偶。在几次尝试安装并找到热电偶的正确位置后，他重新组装了熨斗，并将所有东西连接到现成的工业 PID 控制器上。

没有人相信一切都在工作，[迈克]开始测试铁。他使用 Hakko FG-100 烙铁尖端温度计测量尖端的“真实”温度，并将其与 K 型热电偶报告的值进行比较。结果相当令人印象深刻(如休息后的视频所示)。大约只有 10 度。不算太寒酸。

他的结论是，虽然它确实有效，但它不能取代高质量的焊接站。我们怀疑这种想法的真正问题是云母加热元件对尖端受到的任何热负荷的响应太慢(但未改性的铁也是如此。)如果你对组装自己的焊台感兴趣，你可能会对[开源烙铁驱动](http://dangerousprototypes.com/2012/05/29/soldering-iron-driver-v1-5-assembled-and-enclosed/)感兴趣。

[通过[危险协议类型](http://dangerousprototypes.com/2015/04/27/soldering-iron-pid-temperature-controller/)

[https://www.youtube.com/embed/uPF152qa5rU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uPF152qa5rU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)