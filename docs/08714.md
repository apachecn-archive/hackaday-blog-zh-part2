# 卡斯塔拆卸

> 原文：<https://hackaday.com/2015/04/05/castar-teardown/>

一年多前，castAR 这款带有投影仪和反光表面的增强现实眼镜在 Kickstarter 上亮相。从那以后[我们在 Maker Faire](http://hackaday.com/2013/09/24/castar-comes-to-maker-faire-ny-2013/) 上看到了它，看到它被[用于可视化 3D 打印](http://hackaday.com/2014/05/23/castar-and-holographic-print-preview-for-3d-printers/)，以及[与最新版本的硬件](http://hackaday.com/2015/01/12/castar-hands-on-and-off-record-look-at-next-version/)坐在一起。现在，我们信任的两个人中的一个终于得到了他的开发者版本的 castAR。

在[Mike]深入研究硬件之前，快速回顾一下 castAR 的工作原理:眼镜内部有两个 720p 投影仪，将图像投射到一块反光织物上。这个图像直接反射回眼镜，一副偏振眼镜(就像你在 3D 电视上看到的那种)，将图像分成左右两只眼睛。给眼镜添加一些头部跟踪功能，你就有了一个 castAR。

这款眼镜配有一个小腰包，可以为眼镜供电，为附件插座添加两个插孔，并切换来自计算机的 HDMI 信号。眼镜是真正有趣的地方，它有两个摄像头，两个投影仪和几个非常大的芯片。投影仪本身就是一个巨大的创新；[Jeri]公开表示[镜头制造商告诉她光学装置不应该工作](http://hackaday.com/2015/01/12/castar-hands-on-and-off-record-look-at-next-version/)。

至于芯片，有一个 HDMI 接收器和一个 Altera Cyclone FPGA。黑板上还有一张来自小行星的整洁的小图片。下面视频。

[https://www.youtube.com/embed/WipDp7-zSZo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WipDp7-zSZo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)