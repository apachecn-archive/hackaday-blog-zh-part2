# 机会游戏作为红牛的创作作品

> 原文：<https://hackaday.com/2012/07/03/game-of-chance-built-as-a-red-bull-creation-entry/>

![](img/bd0db6ec7b5f51cd90b0d21d7c61ad93.png "redbull-creation-spinner-game")

[Tom Bourke]写信来炫耀为今年红牛创作大赛打造的[机会游戏](http://www.wausaucollaborationcenter.com/2012/07/03/redbull-game-is-done/)。该项目是在威斯康辛州沃索的黑客空间沃索协作中心的帮助下完成的。

在休息后的剪辑中，他很好地展示了这场比赛。靠近设备底部是一个硬盘驱动器盘片，每个玩家可以旋转它来测试他或她的运气。[Tom]使用 max485 芯片将硬盘电机的导线变成正交编码器。这种输入由 Bullduino 板监控，该板在旋转过程中进行声光表演。显示器周围的 LED 可以单独寻址(可能[与墙壁显示器](http://hackaday.com/2012/06/22/bring-your-led-matrix-project-into-the-living-room/)相同的 LED 串),并根据图案的旋转速度循环显示不同的颜色。七段式大显示屏显示生成的随机数。掷出十点你就赢了！我们猜测您需要自己完成游戏的其余部分，但这可以很容易地用作 16 面骰子(或更少)。

[https://www.youtube.com/embed/yXgegmV3JUI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/yXgegmV3JUI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)