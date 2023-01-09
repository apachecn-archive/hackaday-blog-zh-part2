# 极客婚礼的电子婚纱

> 原文：<https://hackaday.com/2013/08/16/electronic-wedding-attire-for-a-geeky-wedding/>

[![](img/87da052684235b76eda8906924122e31.png)](http://hackaday.com/wp-content/uploads/2013/08/02_1047_d_s_1147-large-1024x682.jpg)

过去，我们展示了许多在[Bill]和[Mara]婚礼上使用的项目。然而，我们忘记了最重要的事情:他们的电子增强型服装。

从上图可以看出，妻子选择了 led，而丈夫更喜欢电致发光(EL)线/面板。基于 ATtiny 的平台 *LilyTiny* 被挑选来控制所有的 led， [charlieplexing](http://en.wikipedia.org/wiki/Charlieplexing) 被实现，因为只有 4 个 IO 引脚可用。动画是用 [Vixen](http://www.vixenlights.com/) 制作的，并通过 python 脚本导出。

为了给 EL 线供电，[比尔]黑了一个 Sparkfun EL 电池组/逆变器。他移除了外壳，取出了逆变器部分，对设计进行了充分的逆向工程，以找出如何绕过产生开/关/闪烁功能的板载微控制器。最后，他 3D 打印外壳，用一个锂离子电池组包装电子设备。升压调节器用于提供 EL 面板电源所需的 12v 电压。

别忘了看看他们的[核心](http://hackaday.com/2013/03/28/centerpieces-for-a-geeky-wedding/)和[婚礼请柬](http://hackaday.com/2013/01/30/really-really-geeky-wedding-invitations/)，我们之前已经介绍过了。