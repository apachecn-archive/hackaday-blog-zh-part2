# 旋转视点显示器上的全彩视频

> 原文：<https://hackaday.com/2012/09/11/full-color-video-on-a-spinning-pov-display/>

[在旋转的视点显示器上观看大巴克兔子](http://roseace.telecom-paristech.fr/)令人印象深刻。当然，圆形的显示区域切掉了一部分画面，但除此之外，它看起来棒极了。此 POV 显示基于 Gumstix 板。它运行嵌入式 Linux，这使得视频播放相当容易。但是将每一帧转换成圆形显示器就是另一回事了。

该设备是巴黎电信的一个课程项目的成果。[Félix]、[Sylvain]和[Jérémy]使用 FPGA 进行像素映射。这使用一个编码器轮(而不是传统的霍尔效应传感器)来确定叶片的位置。监控光盘的传感器发送正交编码脉冲，产生 10 位位置数据。FPGA 使用该数据来计算每个 LED 落在其弧中的位置，然后查找该位置的像素颜色。它不是我们见过的最大的 POV 显示器，但它肯定拥有迄今为止最好的 RGB 分辨率。

[https://www.youtube.com/embed/wcM7Y_jDjSY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wcM7Y_jDjSY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢亚历克斯]