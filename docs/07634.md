# 从互联网上的图片克隆一块板子

> 原文：<https://hackaday.com/2014/11/22/cloning-a-board-from-pictures-on-the-internet/>

[Andrew]在 90 年代早期是一个非常酷的家伙，他有一个很棒的键盘合成器，可以做波表合成、采样、音序器和效果处理器。这是一个奇怪的存储时代；合理数量的闪存是闻所未闻的，软盘统治了土地。[Andrew]的 synth 可以选择连接 SCSI 驱动器。像所有高端设备的可选附件一样，Ensoniq SCSI 卡的当前价格是天文数字，[【Andrew】认为他可以自己制作一个这样的卡](http://rosinsmoke.wordpress.com/2014/11/15/recreating-an-obsolete-scsi-1-interface-board-for-an-equally-obsolete-synthesizer/?preview_id=190)。

在易贝闲逛时，[Andrew]发现了问题中的卡——只有几个无源器件、一些连接器、一个电压调节器和一个来自 AMD 的奇怪芯片。这个芯片是一个 33C93A，一个 SCSI 控制器，他花了 7 美元从中国供应商那里买到了一个。没有比这更好的了。

手里拿着芯片的数据表和一些关于电路工作原理的合理假设，[Andrew]试着画出原理图。之后，他找到了另一个几年前尝试过相同项目的爱好者。所有的网都是一样的，剩下要做的就是把一块板送到工厂。

快速浏览一下[前面板 Express](http://www.frontpanelexpress.com/) 给【Andrew】弄了一个卡的安装支架，把它插入 synth 后，显示了一个新的选项——SCSI。[成功了](http://rosinsmoke.wordpress.com/2014/11/21/achievement-unlocked-my-ensoniq-sp-4-scsi-clone-works/)，有了一个古老的 SCSI 光盘驱动器，他有了大量的离线存储空间来存放他的 synth。伟大的工作，我们希望看到更多的东西。