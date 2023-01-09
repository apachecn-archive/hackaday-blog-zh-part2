# 多功能一体电脑的极限维修

> 原文：<https://hackaday.com/2014/11/18/extreme-repair-of-an-all-in-one-pc/>

在浏览当地拍卖网站时，[Viktor]发现自己在竞拍一台破旧的联想 A600 一体机。他出价 50 美元左右，赢了。接下来是困难的部分—[真正让这个东西工作起来](http://www.karosium.com/2014/11/lenovo-ideacentre-a600-restoration-intro.html)。前面的玻璃破裂了，但幸运的是液晶显示器安然无恙。热管看起来像是被活动扳手攻击过。superIO 芯片的引脚被损坏，最糟糕的是， [MXM 显卡](http://en.wikipedia.org/wiki/Mobile_PCI_Express_Module)没电了。

第一项任务是修复 superIO 芯片的引脚和附近几个被撞掉的分立元件。完成后，[维克多]实际上能够让电脑从 USB 闪存驱动器启动到 Linux。下一步是打开显示器。[维克多]只需要一个编码站，所以除了死了，MXM 上的视频加速器对他没什么用处。联想的主板被设计成支持 MXM 卡上的视频或内部视频。切换意味着改变一些驱动程序设置和移动一些组件，包括显示器本身的一个相当大的 LVDS 连接器。这是一项艰巨的任务，更糟糕的是，[维克多的]焊接工具是一对焊枪，更适合用来修理 57 年雪佛兰的车身。他能够制造出各种各样的热线装置，并移动了连接器。当他完成时，只剩下一个小小的焊接桥！

最终结果是[Viktor]有了一个新的编码工作站，一台废铁般的电脑从垃圾填埋场被救了出来。如果你喜欢这个黑客，检查一下[维克多的] [低功率 PSU](http://hackaday.com/2011/03/23/diy-low-power-psu-for-home-server-use/) ，或者他的 [1 线网络](http://hackaday.com/2010/03/23/1-wire-lan-with-an-lcd/)！