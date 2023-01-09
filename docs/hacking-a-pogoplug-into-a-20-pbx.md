# 将 Pogoplug 接入 20 美元的 PBX

> 原文：<https://hackaday.com/2014/09/15/hacking-a-pogoplug-into-a-20-pbx/>

Pogoplug Series 4 是一款小型网络连接设备，可让您远程访问外部驱动器。在这个设备的引擎盖下是一个运行在 800 MHz 的 ARM 处理器，它由 Linux 内核支持。如果你想以低廉的价格构建自己的 PBX，[Ward] [为我们介绍一下这个过程](http://nerdvittles.com/?p=10560)。由于 Pogoplug 4 目前售价约为 20 美元，这是一种玩电话的廉价方式。

第一步是将 [Pogoplug 转换成 Debian](http://blog.qnology.com/2014/07/hacking-pogoplug-v4-series-4-and-mobile.html) ，这通常需要仔细遵循说明。Pogoplug 启动 Debian 后，就可以安装[不可思议的 PBX](http://incrediblepbx.com/) 包了。过去，我们已经看到这个包[在树莓派](http://hackaday.com/2012/08/22/building-a-pbx-setup-around-the-raspberry-pi/)上运行。令人难以置信的 PBX 基于[星号](http://www.asterisk.org/)和 [FreePBX](http://www.freepbx.org/) 的预配置设置提供了大量开箱即用的功能。

随着你的 20 美元的 PBX 运行，有很多事情可以做。谷歌的语音服务允许无限制地免费拨打美国和加拿大的电话。有了互联网连接，你可以收到语音邮件的通知，还可以通过语音查询 WolframAlpha。