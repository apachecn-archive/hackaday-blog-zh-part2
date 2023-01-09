# 用科学和统计测量声速

> 原文：<https://hackaday.com/2012/08/27/measuring-the-speed-of-sound-with-science-and-statistics/>

尽管你可能在其他地方听说过，但科学不仅仅是阅读[尼尔·德格拉斯·泰森]的推特账户或基于上帝不存在的认识论。不，科学需要更多的工作来观察*宇宙、*，正如【Ast】在分析数据以[用微控制器](http://flavourmixing.wordpress.com/2012/08/22/measuring-the-speed-of-sound/)测量声速的冒险所证明的。

在[Ast] [建造了一个时间数字转换器](http://flavourmixing.wordpress.com/2012/08/07/timing-is-crucial/)——基本上是一个具有微秒分辨率的超大秒表——之后，他需要一个项目来展示他的 TDC 可以做什么。声速似乎是一个合理的测量方法，所以[Ast]在他巨大的秒表上连接了一对麦克风和放大器。在将麦克风分开测量的距离之后；[Ast]拍手，记录声音在两个麦克风之间的飞行时间，并重复测试。

[测试结束后，](http://flavourmixing.wordpress.com/2012/08/22/measuring-the-speed-of-sound/2/)【Ast】有一组数据记录了拍手声在每个麦克风之间传播的时间。一个简单的线性回归(有一些单位转换)显示声速为每秒 345 +/- 25 米，误差为 7%。

7%的误差幅度并不大，所以[Ast]决定拿出 [Numpy](http://numpy.scipy.org/) 来分析数据。在第一次分析中，每个数据点都被同等对待，这意味着数据中的异常值会产生巨大的误差。通过计算每次距离测量的标准偏差，误差减小，并且[声速变为 331 +/- 14 米/秒](http://flavourmixing.wordpress.com/2012/08/22/measuring-the-speed-of-sound/3/)。

这个结果更好，但是仍然有一些无关的数据点。将这些归因于回声和房间振动，并在仔细考虑后，将这些数据点丢弃。最后的结果？每秒 343 +/- 9 米，误差为 2.6%。

你只需要在维基百科上查一下就能做很多工作？是啊，但那不是科学，不是吗？