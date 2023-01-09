# 船长，乘坐你的 Arduino 控制的自动驾驶帆船

> 原文：<https://hackaday.com/2014/01/08/ride-captain-ride-aboard-your-arduino-controlled-autopiloted-sailboat/>

机械工程师、织布机制造商和狂热的水手杰克想要为他 1983 年的罗伯特·佩里·北欧 40 号帆船配备一个比原来更现代的自动驾驶系统。他知道基于 PC 的解决方案可以工作，但是有点遥不可及。然而，一旦他的儿子向他展示了 Arduino，他就上路了。他为他的单桅帆船 Wile E. Coyote 建造了这个基于 Arduino 的自动驾驶系统。

他用了两个 Arduino Megas。一个只用于 GPS，另一个控制其他一切。[杰克]的自动驾驶仪有三种模式。在他所谓的旋钮转向中，一个电位计驱动现有的液压泵，他用一个 [Polulu Qik 系列 DC 电机控制器](http://www.pololu.com/product/1112)控制该液压泵。在指南针转向模式下，一个 [Pololu IMU](http://www.pololu.com/product/1268) 锁定航向转向(HTS)。GPS 模式使用一个预先确定的航路点，并将航向(CTS)设置为与航路点相同的方位。

[Jack]的系统还在必要时使用交叉跟踪误差(XTE)校正来计算新的 HTS。他在 [Dropbox](https://www.dropbox.com/sh/l1l1432c9vfs4g1/7PJUMgsj0E) 上有很棒的文档和几个 Fritzing 和 Arduino 文件。

自动驾驶帆船装置现在一定很流行。我们刚刚在 11 月份看到了另一部。

[https://www.youtube.com/embed/-nA6wo9PXls?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-nA6wo9PXls?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢杰里米]