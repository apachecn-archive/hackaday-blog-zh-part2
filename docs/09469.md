# Hackaday 奖参赛作品:DIY 眼球追踪

> 原文：<https://hackaday.com/2015/07/05/hackaday-prize-entry-diy-eye-tracking/>

在互联网广告商和制作工作室的黑暗深处，有一个非常非常奇怪的装置。它适合戴在用户的头上，有一个摄像头指向外，但也有一个摄像头指向用户。那个额外的摄像头正对着眼睛。这是一个视线追踪系统，一个可穿戴的机器人，它看着你的眼睛，可以准确地告诉你你在看什么。如果人们真的在看广告，这正是你需要知道的。

为了他们的 Hackaday 奖参赛作品，Makeroni Labs [正在构建一个开源的眼球追踪系统](https://hackaday.io/project/6638-eye-of-horus-open-source-eye-tracking-assistance)。如果你想测试一个网页有多“粘”,或者——因为我们希望看到人们用他们的 Hackaday 奖励项目做一些有用的事情——对于不能控制自己周围环境的残疾人来说，这正是你想要的。

建造一台眼球追踪相机只需要几样东西——一对相机和一点软件。这些摄像头只是网络摄像头，去掉了红外滤光器，几个红外发光二极管对准眼睛，这样面向眼睛的摄像头就可以看到瞳孔。第二个摄像头直接指向前方，通过一点复杂的数学运算，该软件可以计算出用户在看哪里。

电子设备相当有趣，所有处理都在 Linux 上运行，希望它足够快，可以捕捉两个视频流，计算学生在看哪里，并发送另一个视频流。至于其余的构建，该团队正在 3D 打印一切，并计划让每个人都可以使用该设计。这对于视线追踪实验来说很棒，对于真正需要它的人来说是一项了不起的技术。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)