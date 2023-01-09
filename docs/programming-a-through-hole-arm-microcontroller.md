# 通孔 ARM 微控制器编程

> 原文：<https://hackaday.com/2013/05/29/programming-a-through-hole-arm-microcontroller/>

![NXP](img/3d05ed25ffbcdc4e382e9cc473bd880b.png)

电子爱好者的 ARM 微控制器时代即将到来，幸运的是，DIP 封装中有几款兼容试验板的微控制器。其中一款芯片是恩智浦的 LPC 810m 021 fn 8——一款小型 8 引脚 DIP 芯片，配有 4 kB 闪存和 1kb SRAM，时钟速度足以处理一些非常酷的东西。[Joao]需要一种方法来对这些微控制器中的一个进行编程，并想出了一种仅使用 USB/UART 适配器的[简单方法。](http://vilaca.eu/lpc810/)

这种构建的关键是，LPC810 不需要任何额外的组件来操作；内部振荡器意味着芯片将在 30 MHz 下运行，只需连接电源和接地。为了给芯片编程，[Joao]将芯片的 Tx 和 Rx 线连接到一个 USB/UART 适配器上(当然是 3.3 V)，用 [Flashmagic](http://www.flashmagictool.com/) 上传了一些代码。

在之前，我们已经见过这些 [DIP 大小的 ARM 芯片，但是【Joao】使用现成工具编写闪烁 LED 程序的方法意味着开始使用这些非常酷、非常强大的微控制器是小菜一碟。](http://hackaday.com/2012/09/09/the-easiest-way-to-dive-in-to-arm-programming/)