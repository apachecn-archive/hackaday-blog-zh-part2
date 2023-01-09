# MagnID——与平板电脑互动的新方式

> 原文：<https://hackaday.com/2015/01/13/magnid-sneaky-new-way-of-interacting-with-tablets/>

被称为“MagnID”的新磁性技术将于本周末在斯坦福大学的年度 TEI 会议上展示。这是一个聪明的黑客，旨在劫持平板电脑的指南针传感器，迫使它识别多个物体。这里先睹为快，看看平板电脑磁输入的可能性。

许多平板电脑都带有某种三轴磁传感器，但正如[Andrea]和[Ian]的演示所示，它们只能传递所有磁力的聚合矢量。如果一个人有多个磁性物体，传感器不能提供太多有用的信息。

他们的解决方案是软件和硬件的结合。每个物体都有一个以不同速度旋转的磁铁。这就产生了复杂的正弦磁场，可以用带通滤波器进行数学隔离。这也给了它们到每个物体的距离。该团队添加了一个带有磁力计的 Arduino，原因不明，也许内置在平板电脑中的磁力计还不够？

下面的演示视频展示了引擎盖下的东西和一些简单游戏的新输入机制，草图和一个[徽标龟](http://hackaday.com/2012/01/31/turning-the-big-trak-into-a-turtle/)。他们希望这能打开所有有形设备的大门。

请在 2015 年 1 月 15 日至 19 日举行的斯坦福第九届年度“[有形、嵌入式、具体化互动](http://www.tei-conf.org/15/)”上查看他们的演示。

[https://www.youtube.com/embed/fAxQ8lzSsYY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fAxQ8lzSsYY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)