# Hackaday 获奖作品:更好的 KVM 交换机

> 原文：<https://hackaday.com/2015/05/05/hackaday-prize-entry-a-better-kvm-switch/>

现在，在一个战斗岗位上拥有一台台式机和一台笔记本电脑，而平板电脑则在一旁待命，这并不罕见。再加上一些锉刀、控制台和各种便宜的电脑，很容易在一张桌子上摆放大量的机器和显示器。传统上，KVM 交换机是解决这一问题的方法，它与许多不同的设备共享键盘、鼠标和显示器，但这是一个丑陋的解决方案。[frankstripod] [有一个设备可以用一些有趣的软件和一些 USB 接口来修复这个问题。](https://hackaday.io/project/2872-driverless-mouse-and-keyboard-sharing)

[frankstripod]爱上了一个名为 [Synergy](http://www.synergy-project.org/) 的程序，这个程序通过网络将几台计算机的键盘、鼠标和显示器结合在一起，因此你将只需要使用一个键盘和鼠标；就像把你的鼠标从一台电脑拖到另一台电脑一样简单。不过也有一些限制:在操作系统加载之前，键盘无法工作(没有 BIOS 访问)，如果网络中断，键盘也无法工作，设置可能会很复杂。这个项目旨在用一个小型的，可联网的 KVM 取代 Synergy 设置中的“服务器”部分。

目前的计划是使用一个运行 Linux 的小型嵌入式板来读取 USB 键盘，并在几台计算机之间切换输出。一些脚本检测鼠标从一个屏幕移动到另一个屏幕，一个微控制器在每台计算机之间切换 USB 输出。如果这听起来很奇怪，你是对的，但它确实有效:[frank]的 2014 年 Hackaday 奖项目[是一个可以同时与两台计算机一起工作的鼠标](https://hackaday.io/project/1125-mouse-controller-project)。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)