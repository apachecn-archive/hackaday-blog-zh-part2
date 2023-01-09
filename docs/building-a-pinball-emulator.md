# 构建弹球模拟器

> 原文：<https://hackaday.com/2015/04/11/building-a-pinball-emulator/>

建造一台 MAME 机器——一个可以玩从 *Galaga* 到 *Street Fighter II* 的游戏的街机柜——肯定在全球成千上万 Hackaday 读者的“要建造”清单上。这是一个相对简单的建设，提供你可以把一张中密度纤维板在你的车；这只是一个模拟器，如果你能找到一个 CRT，并有一台旧电脑，你已经成功了一半。

还有一类街机游戏可以效仿。这当然是弹球机。[Jan]在过去几个月里建造了一个虚拟弹球柜[，他的建造日志令人难以置信](http://www.klomp.de/index.php/virtueller-flipper-vpin-selber-bauen/homemade-virtual-pinball-cabinet-vpin)。如果你曾经想建立一个弹球模拟器，这是参考指南。

弹球模拟器最重要的部分是显示器。为此，[简]在操场上使用了一台 40 英寸的电视，[一台 28 英寸的显示器来展示玻璃艺术](http://www.klomp.de/index.php/virtueller-flipper-vpin-selber-bauen/66-virtueller-flipper-installation-monitor-dmd-und-lautsprecher-in-backbox-backglass)，还有一台传统的[128×32 DMD](http://www.klomp.de/index.php/virtueller-flipper-vpin-selber-bauen/66-virtueller-flipper-installation-monitor-dmd-und-lautsprecher-in-backbox-backglass)。他没有制造自己的橱柜，而是重新利用了一台旧的机电机器 [Bally 的*小乔*](http://www.ipdb.org/machine.cgi?id=1460) 。

软件是这场表演的真正明星，PinballX 作为前端，[未来弹球](http://www.futurepinball.com/)和[视觉弹球](http://sourceforge.net/projects/vpinball/)作为模拟器。这些模拟器驱动显示器，更换后玻璃，并模拟球的物理特性。运行所有这一切的计算机有几个整洁的机电位，包括一个摇动器电机，一个原始的 Williams replay 敲门器，[和一些继电器或螺线管](http://www.klomp.de/index.php/virtueller-flipper-vpin-selber-bauen/58-virtueller-flipper-echtes-pinball-feeling-mit-den-siemens-schuetzen-als-force-feedback)给数字表一个巨大的力反馈。这是做这件事的方法，如果你没有把这些机电零件安全地固定在机器上，你就真的失去了沉浸感。

你可以在下面看看这张桌子的视频。

[https://www.youtube.com/embed/wgAAYnFD-dk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wgAAYnFD-dk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)