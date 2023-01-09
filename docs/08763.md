# 回顾:回复:加载专业版

> 原文：<https://hackaday.com/2015/04/10/review-reload-pro/>

大约一年前，蜘蛛实验室的[Nick Johnson]发了一篇关于 Re:load Pro 的提示，这是他的数字恒流负载设计。[Nick]正在开展一项众筹活动，这总是让我在发帖时三思。然而，在这种情况下，我毫不犹豫地在博客上写了一篇[特写(并用我自己的钱支持这场运动)。回复:load Pro 其实是【尼克】的第三代电流负载。购买并使用了原版 Re:load 后，我知道[Nick]有能力实现竞选中的所有承诺。事实证明我是对的——[ Nick]和蜘蛛实验室团队进行了一次非常成功的众筹活动。所有 kickstarter 的支持者已经享受他们的单位几个月了。当到了](http://hackaday.com/2014/04/16/reload-pro-an-open-source-active-load/)[为 Hackaday 商店](http://store.hackaday.com/products/re-load-pro)进货的时候，Re:load Pro 是一个显而易见的选择。

为什么需要数字恒流负载？大量的工作可以从中受益！从测试电池到验证电源，再到测试许多驱动电路，数字负载都是您的利器。

像许多电子设备一样，我们使用 Re:load Pro 的第一步是升级固件。由于 Re:load Pro 由赛普拉斯半导体 PSOC 4 操作，固件更新由 cyflash python 包处理。现在，这意味着使用命令行并安装 pip 和 cyflash。那些不熟悉命令行提示的人会在[固件更新页面](http://www.arachnidlabs.com/reload-pro/firmware.html)上找到一步一步的指导。

我应该注意到 Re:load Pro 是由 USB 输入供电的。我把它连接到我的实验室电脑上，它可以毫无问题地提供必要的电源。

## 校准

下一步是校准 Re:load Pro。这需要一个能够提供至少 10 伏 2 安培电压的可调电源，一个合适的万用表，当然还有一些测试引线。如果你没有可靠的可调电源，问问周围的人；应该很容易找到这样的人。

校准分三步进行——第一步，不连接 Re:load Pro。然后连接设置为大约 9.99 伏的电源。用旋转编码器调整 Re:load Pro 上显示的电压，以显示与电源相同的值。我的电源有一个相当便宜的内部电压表，所以我用了一个万用表并联设置。电压完成后，Re:load Pro 将从电源汲取 2 安培电流。您需要调整 Re:load Pro 上显示的电流，使其与电源电流表上显示的电压相匹配。同样，由于我的电源没有最精确的仪表，我使用了万用表——这次是与负载和电源串联。

## 进行测量

所有的前期工作完成后，是时候进行一些测量了！回复:load pro 有一个简单的用户界面。所有东西都可以通过前面板上的旋转编码器来访问。将旋钮转到所需的值，然后按选择。在我的例子中，我想检查在各种负载下 LiPo 电池的电压降。我简单地接上电池，在编码器上拨了 350 毫安。Re:load Pro 显示电池保持在 12.1 伏，左下方的显示屏显示我从电池中取出了多少毫安时。

Re:load Pro 的 USB 连接器不仅仅是为了供电。它会以串行设备的形式出现在你的电脑上。只需打开您最喜欢的终端模拟器，将端口设置为 115200 波特 8/N/1，就可以了。Re:load Pro 使用简单的基于文本的命令/响应协议，所有命令都在[蜘蛛实验室页面](http://www.arachnidlabs.com/reload-pro/usb-interface.html)上有概述。

## 结论:

Re:load Pro 是第一批新型开源工具之一。像闭源 Rigol 示波器一样，它取代了成本高出数倍的工具。[Nick]Arachnid Labs 并没有满足于他们的成功，他们刚刚完成了他们最新开源工具的 kickstarter。 [Tsunami](https://www.kickstarter.com/projects/nickjohnson/tsunami) 是基于 Arduino 平台的开源信号发生器。工具支持项目，开源工具是推动整个生态系统向前发展的最佳方式。

* * *

编者按:我们正在 Hackaday 上复兴“评论”的概念。很久以前，Hackaday 的校友伊恩·莱斯内特(Ian Lesnet)在他关于智能镊子(T2)的文章中率先提出了这些方法，但自那以后几乎没有人做什么。我们看到大量的工具、零件、原材料和设备在我们的收件箱中流动。我们计划以新的[黑客专栏](http://hackaday.com/category/hackaday-columns/)的形式发布评论。这些评论不是付费的，它们是由编辑和作者根据我们自己的兴趣选择的。这个特殊的例子在 [Hackaday 商店](http://store.hackaday.com)有售，我们从它开始，因为我们已经有了硬件。然而，我们将审查项目，我们不卖，并已提出了审查单位的要求。如果您知道一些您认为值得审查的内容，请通过[提交给提示热线](http://hackaday.com/submit-a-tip/)让我们知道。谢谢！

*-Mike Szczys，执行主编*