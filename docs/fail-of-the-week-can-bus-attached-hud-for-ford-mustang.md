# 本周故障:福特野马的 CAN 总线连接平视显示器

> 原文：<https://hackaday.com/2013/11/07/fail-of-the-week-can-bus-attached-hud-for-ford-mustang/>

这一期的《一周失败》非常出色，你的帮助真的可以让失败的项目重回正轨。[Snipor Bob]想要替换他的野马上所有的仪表盘读数，并有了将被黑的硬件做成平视显示器的想法。你在上面看到的只是接入车辆数据系统的早期硬件概念验证。但也有一个有趣的测试装置，让挡风玻璃作为读数的反射器。

仪表板侧面贴着的看起来很棒的装备导管实际上是我们最喜欢看的东西。但这个想法是使用字符显示器(安装在其他地方)作为光源，在挡风玻璃上投影一个仪表组。[Bobby]正在使用 STN1110 多协议 CAN 芯片接入总线，使用 Arduino Mega 提取数据并驱动显示器。你可能会想，这就是他失败的地方，因为我们从 CAN Hacking 系列中知道,[逆向工程数据库以理解数据](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/)是一件痛苦的事情。幸运的是，他从互联网的某个黑暗角落找到了一张包含所有代码的图表。当真正实现平视显示器时，失败出现了。

下面的剪辑显示了他的平视显示器反射测试使用菲涅尔透镜和一块玻璃来代替挡风玻璃。问题是，为了给合适的焦距腾出空间，他需要将仪表组从仪表板上完全移除。从物理上来说，这不是问题，但事实证明[被动防盗系统](http://www.explorerforum.com/forums/showthread.php?t=234975) (PATS)监控着仪表组，如果它被移除，就会被触发——防止汽车启动。由于显而易见的原因，禁用 PATS 是不可行的，但我们敢打赌，这样做会使您的保险单无效(取决于您的保险商和您的居住地)。

所以，给一个黑客一些这方面的建议吧。[Bobby]如何欺骗组合仪表，以便在不触发 PATS 锁定的情况下将其移除？

[https://www.youtube.com/embed/ZWUESxbtlH8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZWUESxbtlH8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**