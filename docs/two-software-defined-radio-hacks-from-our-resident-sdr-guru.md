# 来自我们的常驻 SDR 专家的两个软件定义无线电黑客

> 原文：<https://hackaday.com/2012/06/16/two-software-defined-radio-hacks-from-our-resident-sdr-guru/>

![](img/40ffd5cdce732f03b93c51327a85c66a.png "radio")

看来[巴林特]在这些领域正成为某种程度上特别提款权大师；在过去的几个月里，他得到了一个与 GNU Radio 一起工作的 USB 电视调谐器接收器，开始了一个软件定义的广播教程 YouTube 频道，甚至使用这个项目来监听飞机和空中交通管制之间的对话。这一次，【巴林特】回来了~~使用这个廉价的 USB 电视调谐器进行~~ [无线电测向](http://wiki.spench.net/wiki/SDRDF)，并在 [Linux](http://www.youtube.com/watch?v=46VbuViPKt4) 和 [OS X](http://www.youtube.com/watch?v=492Ub66IsRA) 中运行 HDSDR。

【巴林特】的[无线电测向演示](http://www.youtube.com/watch?v=NSC4Y8yA-jY)回顾了使用多普勒效应和机械旋转天线的传统测向方法。因为[巴林特]处理的是 150MHz 左右的频率(约 2 米波长)，建立一个物理测向设置需要以每分钟 40000 转的速度旋转天线；对于任何硬件构建来说都太快了。[巴林特]的解决方案是在一个圆周上连接 4 个天线，每秒钟在它们之间进行数千次电子切换。[巴林特]给[建了一个 wiki 页面](http://wiki.spench.net/wiki/SDRDF)，详细介绍了他构建的所有理论和实现细节。

[巴林特]还写了一个简洁的应用程序,通过网络控制软件无线电，包括 Realtek 电视加密狗。在足够广阔的地理区域内，任何人扮演空中交通管制员都将变得极其容易[。BorIP 服务器还可以用来在 Wine 下运行 Linux 和 OS X 的](http://hackaday.com/2012/04/16/playing-air-traffic-controller-with-software-defined-radio/)[HDSDR](http://www.hdsdr.de/)；只需将 HDSDR 连接到同一台机器上的网络回环，就可以避开 Wine 对本地访问硬件的厌恶。

令人敬畏的工作，我们迫不及待地想看到[巴林特]的实验室下一步会出什么。

编辑:代替加密狗，[Balnt]正在使用一个“真正的”软件无线电板。很多人给他发信息，问他是否可以用同样的方法用电子狗来寻找方向。以下是[巴林特]要说的话:

> 在我看来，诀窍是创建一些(或多或少简单的)额外硬件，直接从加密狗的板载振荡器中取出时钟信号，并将其分频以供天线开关使用，即 28 MHz 几十 kHz(这是在 FPGA 上的“软件”中完成的)。然而，仍然存在一个问题:计数器需要根据天线当时指向的已知方向进行校准，否则来自加密狗的数据流的停止/开始将意味着每次停止/开始时方向将失去同步 90/180/270 度。也许有人会为这个小小的障碍想出一个优雅的解决方案！

所以你走吧。准备好接受挑战了吗？