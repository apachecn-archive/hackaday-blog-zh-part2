# 亮闪闪的头饰

> 原文：<https://hackaday.com/2012/06/25/blinky-headgear-2/>

![](img/cfa5e83f4f46eb8b035c3d87fa8ca5fc.png "blinky-headgear")

由于我们的老朋友 555 定时器，这款[帽子有一个追逐 LED 功能](http://www.instructables.com/id/Rotating-LED-Marquee-Hat/)。[BananaSlug]甚至内置了一个按钮就能改变速度的选项。

他的设计从一顶戏服帽开始。25 个发光二极管中的每一个都焊接到一个 2×4 孔的原生电路板上。LED 封装通过帽子上的一个狭缝推出，但原型板仍然留在里面，可以缝合到位。从那里[BananaSlug]将一条负极总线焊接在周围，并将每个模块的一条单独的正极引线焊接回控制板。它们由一组 CD4017 十进制计数器寻址，这些计数器由 555 定时器电路计时。

这是一个很棒的小模拟/逻辑项目，如果你有合适的外套，这种风格是完美的。