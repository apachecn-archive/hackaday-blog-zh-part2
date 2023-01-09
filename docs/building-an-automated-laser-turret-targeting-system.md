# 建造自动激光炮塔瞄准系统

> 原文：<https://hackaday.com/2015/08/25/building-an-automated-laser-turret-targeting-system/>

去年，[阿尔瓦罗]为 DEFCONBOTs 比赛制造了一个激光炮塔机器人。效果很好，但今年，他决定更上一层楼。现在，他不再移动整个机器人激光阵列，而是使用检流计只移动激光——他实际上是[建造了一个迷你激光投影仪。](http://alvarop.com/2015/08/laser-turret-v2-part-1-overview/)

检流计基本上是一个非常灵敏的移动安培计，它也可以用作非常精确的机电致动器，例如移动一个微小的镜子。你可以想象，你实际上可以建造自制的检流计——但这真的不那么容易。相反，[阿尔瓦罗]选择在易贝订购几个激光表演控制器，并以自己的方式解决问题——我们同意。

给检流计接线并为它们制作一些电路是容易的部分。棘手的部分是自动化系统。

你看，以前当激光器连在摄像机上时，这很简单。激光在摄像机拍摄的地方拍摄。任何简单的图像识别软件都可以。但是现在两者独立了，就没那么简单了。如果你可以精确地安装所有东西，你可以使用 trig 来计算激光角度和最终位置，但问题是…精确地安装所有东西:

> 如果我是一名机械加工/CAD 向导，我可以足够精确地安装激光器、检流计和相机，以便我可以使用一些数学计算角度/深度，并计算出激光的方向。
> 
> 正如我之前提到的，我不是 CAD 专家，而且我的机械技能也…欠缺。由于没有解决这个问题的机械方法，我不得不开始用软件来创造。

他的软件解决方案很酷。它需要通过创建预定义点的网格来进行校准，但从那里开始，可能性是无穷无尽的。看一看。

[https://www.youtube.com/embed/7acicM_vzDA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7acicM_vzDA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

现在一些乒乓球作为目标。

[https://www.youtube.com/embed/NY5AHltA9wE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NY5AHltA9wE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

最后——一辆行驶的火车。

[https://www.youtube.com/embed/55kElXY1A9U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/55kElXY1A9U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

有人记得激光瞄准蚊子系统吗？那些怎么还没投产！上来[阿尔瓦罗]！