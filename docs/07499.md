# 电池保护罩安装在 Arduino 下方

> 原文：<https://hackaday.com/2014/11/06/battery-shield-mounts-underneath-the-arduino/>

那么，当你的 Arduino 项目需要在偏远地区运行或者作为便携设备运行时，你会怎么做呢？有脂电池屏蔽可用，尽管它们可能工作良好，但充电需要使用 USB 端口。你也可以走 9v 电池路线，插入 Arduino 的板载调节器，但 9v 的低毫安时额定值不会让你的项目保持运行很长时间。[AI]为他的 Arduino 项目需要一个快速更换电池的选项，并提出了他所谓的 [AA Undershield](//www.instructables.com/id/The-Arduino-AA-Undershield/?ALLSTEPS) 。

顾名思义，该项目使用 AA 号电池，实际上是两节。是的，两节 1.5 伏的 AA 电池串联起来只相当于 3 伏。Arduino 需要 5v 电压，因此[AI]决定使用 MAX756 DC 到 DC 升压稳压器来保持 5v 的稳定电流。[这篇文章](http://cds.linear.com/docs/en/design-note/dn63f.pdf)有一些漂亮的图表，显示了 9v 电池降压至 5v 与两个 AA 电池升压至 5v 之间的性能差异。

Undershield 中的“under”来自这个安装在 Arduino 下面的护盾，不像地球上的其他护盾。这样做允许使用标准的 0.100 英寸间距的原型 PCB，并且是 Arduino 的数字 7 和 8 引脚之间的奇数尺寸空间的简单 DIY 解决方案。Arduino 借助一些铝制支架，通过其正常的安装孔安装到下护罩上。

[AI]做了很好的工作，用图表和大量照片记录了他的构建，这样任何有兴趣为自己制作一个的人都可以非常容易地做到。