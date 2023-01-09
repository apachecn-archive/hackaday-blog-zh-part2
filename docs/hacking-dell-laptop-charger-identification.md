# 黑客攻击戴尔笔记本电脑充电器识别

> 原文：<https://hackaday.com/2014/03/03/hacking-dell-laptop-charger-identification/>

如果你曾经有过笔记本充电器坏了，你知道更换它们会很贵。许多笔记本电脑要求你使用“正品”充电器，并拒绝在使用山寨型号时开机。真正的充电器与笔记本电脑通信，并提供设备的功率、电流和额定电压等信息。虽然这是一个很好的安全措施，确保使用兼容的充电器，但它也允许制造商提高充电器的价格。

[Xuan]为戴尔充电器制造了一种伪造识别信息的设备。在这个由四部分组成的系列( [1](http://hclxing.wordpress.com/2014/02/06/hacking-the-dell-laptop-power-adapter/) 、 [2](http://hclxing.wordpress.com/2014/02/09/hacking-the-dell-laptop-power-adapter-part-ii-2/) 、 [3](http://hclxing.wordpress.com/2014/02/09/hacking-a-dell-power-adapter-part-iii/) 、 [4](http://hclxing.wordpress.com/2014/02/26/hacking-a-dell-power-adapter-final-not-really/) )中，涵盖了逆向工程通信和构建欺骗器的细节。

戴尔使用[单线](http://en.wikipedia.org/wiki/1-Wire)协议与充电器通信，而【Xuan】使用 MSP430 监听通信。在读取数据并验证 CRC 之后，可以对其进行检查，以找到指定功率、电压和电流的字段。

接下来，使用两个戴尔 DC 插孔和一个 MSP430 制作了一个定制 PCB。这通过电路板传递电力，但使用 MSP430 向计算机发送虚假数据。该演示展示了一个假装以 65 W 运行的 90 W 适配器。通过这种工作方式，您可以从任何满足电流和电压要求的电源为笔记本电脑供电。