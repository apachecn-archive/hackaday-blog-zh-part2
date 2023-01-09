# 本周失败:WS2811 像素失败

> 原文：<https://hackaday.com/2014/03/06/fail-of-the-week-ws2811-pixel-failure-on-fled/>

这个失败的项目来自 Hackaday 自己的一个项目。[Ben]承担了[FLED 数据可视化项目](http://hackaday.io/project/3-FLED),作为让供应框架装饰更有趣的一种方式。他得到了相当多的帮助，将 96 个 WS2811 像素焊接到他们定制的 6'x4 '外壳中，结果真的很棒。除了显示服务器负载和玩游戏之外，FLED 还成了一种工作面试。让未来的员工坐在终端前，给他们一个小时来编写他们能想到的最有趣的可视化代码。

但是两周前[本]摇摇晃晃地走进办公室，发现显示器没电了。他有没有试着关掉然后再打开？是的，但是没有用。电源不是问题所在，我们别无选择，只能把显示器从墙上拉下来，打开来看看所有的像素。因为他们每一个人都有 4 个焊点在两边，他认为问题出在断开的连接上。但事实并非如此。他求助于二分搜索法，通过将链切成两半，并测试每一部分。他追踪到下面被涂黑的像素，就像你在上面看到的。

[Ben]认为密封外壳内的一个电容器爆炸了，但不确定。请随意告诉我们您认为该组件中的哪些地方失败了。但我们真正想知道的是，是否有更聪明的方法来嗅出不良像素而不切断连接？带着这个东西(没有护膝)在地板上待了四个小时，[本]发誓不再从随机的中国供应商那里采购像素。下次他可能会用预先组装好的琴弦。我们窃笑；这相当于试图让旧圣诞彩灯发挥作用的高科技手段。

如果你还没看过《逃离》的比赛，休息后看看吧。令人惊讶的是，LED 强度和高质量的漫射材料可以使一个完美的 LED 网格看起来像在波浪和颜色曲线中跳舞。

[https://www.youtube.com/embed/19JfB-rlNQ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/19JfB-rlNQ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**