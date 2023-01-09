# 嵌入式印刷电路板使任天堂四得分 USB 操纵杆

> 原文：<https://hackaday.com/2013/04/21/drop-in-pcb-makes-nintendo-four-score-a-usb-joystick/>

任天堂 Four Score 是最初的任天堂娱乐系统的控制器附件，它允许你同时使用四个控制器。[Simon Inns]想在他的电脑上使用一些原始的 NES 控制器，所以他开发了一种插入式替代板，可以将设备转换为 USB。

正如我们在其他 NES 控制器黑客中看到的，[硬件使用一个简单的并行到串行移位寄存器](http://hackaday.com/2010/12/24/gaming-on-an-ibm-xt-using-an-nes-controller/)将按键传送到控制台。这意味着一次读取四个控制器无异于将数据从四个不同的来源转移到一个微控制器。问题的其余部分是提供一个 USB 连接，将设备枚举为一个操纵杆。我们已经看到了来自[西蒙]的一系列[USB 项目](http://hackaday.com/2011/10/31/do-you-know-what-youre-doing-when-integrating-pc-side-apps-with-usb-microcontrollers/)，所以他能够成功并不令人惊讶。

他选择了内置 USB 支持的 ATmega16U2。[Simon]编写了代码，这样虽然只有一根 USB 电缆，但四个控制器端口中的每一个都将作为独立的 USB 操纵杆出现在计算机上。为了完成这个项目，他仔细测量了原始电路板，并设计了自己的版本，使其符合所有原始组件以及机箱上安装支架的尺寸。顶级[西蒙]！