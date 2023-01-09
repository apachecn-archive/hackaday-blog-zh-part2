# 逆向工程然后用 FPGA 驱动 LCD

> 原文：<https://hackaday.com/2015/01/29/reverse-engineer-then-drive-lcd-with-fpga/>

[Ben Heck]的粉丝知道他对弹球机情有独钟，他围绕这个主题的项目往往相当史诗。这是一个很好的例子。在一次贸易展上，他看到了一个超宽格式的液晶显示屏，他认为这将是一个完美的弹球建筑。他发现这是一种特殊的模块，可以安装在你汽车的遮阳板上。问题是它只需要合成输入，他想要比这更高质量的视频。解决方案:[逆向工程 LCD 协议，在 FPGA 中实现](https://www.youtube.com/watch?v=DIIjVSmbtFc)。

这个项目是一个替换电子驱动程序的完整演示；技能当然不局限于 LCD 模块。他从拆卸硬件开始，寻找看起来像差分信号线路的东西。考虑到这一点，他上网寻找通用视频协议，这将有助于他弄清楚他在寻找什么。一个四通道示波器嗅探信号，因为该装置显示一个蓝色屏幕，上面有红色字样“无信号”。这种模式很容易被发现，因为除了需要显示红色字母时，像素大部分都是重复的。事实证明，该协议很像带有前沿、消隐等的 VGA。

带着大量关于时间的笔记，[Ben]切换到使用 Cyclone III FPGA 来替换屏幕的股票控制器。该产品声称分辨率为 800×234，但当使用这些参数驱动它时，它不会填满整个屏幕。稍微调整一下，他发现显示器实际上有 1024×310 像素。奖金！

我们需要更多的研究来弄清楚他是如何将嗅出的数据归结到他的单一颜色编码的协议单上的。但这只是一半的乐趣！如果你需要更多的资源来理解这些信号是如何工作的，看看[我们另一个最喜欢的 FPGA-LCD 黑客](http://hackaday.com/2011/09/09/putting-laptop-lcds-to-use-with-an-fpga/)。

[https://www.youtube.com/embed/DIIjVSmbtFc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DIIjVSmbtFc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢塞巴斯蒂安]