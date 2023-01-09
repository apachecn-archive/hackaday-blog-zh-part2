# 武器化四旋翼飞行器升级

> 原文：<https://hackaday.com/2014/02/04/weaponized-quadrotor-upgrades/>

今天我们来看几个有趣的黑客，尽管它们可能有点不明智。你能把什么最疯狂的东西绑在四旋翼飞行器上？[火箭](http://www.youtube.com/watch?v=MdFbia2h0_U)？[激光](https://www.youtube.com/watch?v=Nt39Fd87wys)？原来…它们都已经完成了。

首先是[拉米卡扎的]烟火发射四旋翼飞行器。无人机使用 ArduPilot Mega 2.6 稳定，它携带一对由一对钢元件点燃的“火箭”。ATtiny 分析辅助无线电频道的 PWM 信号，该信号控制为元件供电的继电器。他已经在高空测试过了，所以他实际上是非常安全的。

接下来是【JLaservideo 的】激光四旋翼飞行器。他用一个廉价玩具的遥控控制器给他的 Arduino Uno 增加了无线功能。他将原来的遥控玩具的电机电线重新布线到 Arduino 的输入端，反过来激活 5V 继电器，为 1W 激光器供电。由于明亮的光束，它看起来很棒——我们真的希望他戴上了适当的眼睛保护装置，因为那种功率的激光会对你的视网膜造成严重伤害！

休息后留下来看看两个四旋翼飞行器的运行！

**编辑更新:**我同意很多评论，认为这既危险又不负责任。但是我们不应该审查这些内容(这些内容发布在其他地方，所以我们撤下这篇文章没什么作用),我们应该强调这些危险，并想办法安全负责地完成同样的恶作剧。-迈克·斯奇斯

[https://www.youtube.com/embed/MdFbia2h0_U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MdFbia2h0_U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Nt39Fd87wys?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Nt39Fd87wys?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果你看到了更疯狂的事，请告诉我们！