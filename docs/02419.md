# 用手工切割机制作的 DIY 贴片模板

> 原文：<https://hackaday.com/2012/12/27/diy-smd-stencils-made-with-a-craft-cutter/>

除非你愿意花几个小时拿着牙签和一桶焊锡膏，否则每当你放置 SMD 部件时，模板就是你要去的地方。虽然大多数商业和工业 SMD 模板是由激光切割不锈钢制成的，但[Peter]发现一块塑料和一把价值 300 美元的工艺刀同样适合这项工作。

[Peter]花了一些时间用聚酯薄膜制作透明薄片形式的 SMD 模板。这被证明是一种极好的材料；它尺寸稳定，随处可得，厚度正好适合 SMD 模板。聚酯薄膜在一个[剪影浮雕](http://silhouetteamerica.com/silhouetteCameo.aspx)上被切割，基本上是一个桌面大小的乙烯基切割机，目标是工艺品市场。

股票，剪影客串圆角，而不是一些[彼得]想要的功能只有几分之一毫米。[他想出了一个工具](https://github.com/pmonta/gerber2graphtec)将 Gerber 文件的粘贴层转换成单独绘制的线段，使他能够为 0.3 毫米间距的元件切割 SMD 模板。

制作非常精细的模板是一项伟大的工作，但我们想知道这个工具是否可以用在[便宜得多的 Cricut](http://www.cricut.com/home/) 纸和乙烯基切割机上，不幸的是，它被一些非常限制性的软件锁定了。