# 用于廉价蓝牙模块的固件

> 原文：<https://hackaday.com/2014/05/18/firmware-for-cheap-bluetooth-modules/>

如果你曾经用微控制器、某种传感器以及与外界的连接制作过任何东西，你可能会想，中国的那些地方怎么能生产出廉价的电子产品，而价格只是你自己动手制作的成本的一个百分比。这不仅仅是体积，这是工程；如果某个东西有蓝牙，你可以找到一个内置微控制器的蓝牙模块，这样[你就可以给它写固件](http://pfalcon-oe.blogspot.com/2012/04/opensource-sensor-node-firmware-for.html?m=1)。

BC417 是非常受欢迎的 BlueCore4-Ext 蓝牙模块中的片上系统，具有 8mb 闪存(其中 75%用于蓝牙相关的内容)，大约 12 kB 的 RAM，一切都在虚拟机中运行。[pfalcon] [为这个设备](https://github.com/pfalcon/blutunode)写了一个极具实验性的固件，允许任何人用很少的钱创建一个无线传感器节点。这些设备几乎和一个裸露的 ATMega 一样便宜，所以至少可以说，可能性是有趣的。

此时，在这些设备上安装定制固件最困难的部分是对它们进行编程。为此，[Elastic Sheep]用 SPI 接口的并行端口来拯救[。还有一个](http://elasticsheep.com/2012/06/bluetooth-module-parallel-spi-interface/)[固件转储器](http://elasticsheep.com/2012/06/bluetooth-module-firmware-dump/)和一些[分线板可用](http://elasticsheep.com/2011/09/bluetooth-module-breakout-boards-are-back-in-stock/)。这些模块非常便宜，而且间距也不是太差，所以如果你想尝试一下，你可以自己蚀刻电路板。

感谢[Peter]发送此邮件。