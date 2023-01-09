# 简单的超外差短波接收机可追溯到近 100 年前

> 原文：<https://hackaday.com/2015/03/08/simple-superheterodyne-sw-receiver-harks-back-almost-100-years/>

早期的无线电接收器的工作原理被称为调谐无线电频率(TRF)，于 1916 年获得专利。它们不太容易使用，要求每一级都调到相同的频率(直到联动电容器使这变得有点容易)。1918 年设计的超外差式设计更优越，但在当时更贵。出于成本考虑，超级热设计的采用落后于 TRF，直到 1930 年。从那时起，直到最近，超外差设计一直是大多数商业无线电接收机的核心。直接变频接收机是在 1930 年左右设计的，但需要复杂的锁相环，这限制了它们在商业接收机中的应用。所有这些背景的要点是，超外差设计已经很好地服务了 90 多年，但一旦软件定义无线电(SDR)变得无处不在，它很快就会变得多余。这就是为什么这项关于简单超外差短波接收机的研究值得进一步研究。

[Dilshan]制造了这种基于两个晶体管和两个 IF 变压器的超外差无线电，设计用于接收 13m 至 41m 波段。整个构建是在试验板上组装的，因此很容易教其他人进行实验。[Dilshan]对[天线、棒形线圈和 IF 变压器参数](http://elect.wikispaces.com/Two+transistor+superheterodyne+shortwave+receiver)提供了非常有用的见解。要深入研究无线电架构，请查看[业余无线电](http://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/)上的这篇文章。如果你想近距离看看古董收音机，可以看看这个关于[修复古董收音机](http://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/)的帖子。