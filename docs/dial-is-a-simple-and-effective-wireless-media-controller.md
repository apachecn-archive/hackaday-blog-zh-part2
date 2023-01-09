# 拨号是一种简单有效的无线媒体控制器

> 原文：<https://hackaday.com/2015/01/17/dial-is-a-simple-and-effective-wireless-media-controller/>

[Patrick]正在寻找一种更简单的方法来从房间的另一端控制他的计算机上的音乐和电影。有大量的遥控产品可以购买，但作为一名黑客[Patrick]想自己做点什么。他把他的发明称为“拨号”，这是一个简单而优雅的解决方案。

表盘看起来像一个放在平面上的小圆柱形容器。它实际上分为上下两个圆柱体。底部充当底座并保持静止，而顶部充当刻度盘和按钮。该案例是在 SOLIDWORKS 中设计的，并在 3D 打印机上打印出来。

表盘在带有蓝牙模块的 Arduino Pro mini 上运行。最初的原型使用蓝牙 2.0，大约一天后需要充电。最新版本使用蓝牙低能耗规范，据报道一次充电可以持续几周。一旦 LiPo 电池耗尽，插入 USB 端口就可以轻松充电。

刻度盘的机械部件实际上是现成的[旋转编码器](http://hackaday.com/2012/03/08/building-a-magnetic-rotary-encoder/ "DIY Rotary Encoder")。编码器包括一个内置按钮，使事情变得更容易。固件能够检测任一方向的旋转、按钮按压、双击和按住。这给出了五种不同的可能功能。

[Patrick]写了两个软件来处理与表盘的交互。第一个是处理蓝牙通信的 C 程序。第二个实际上是一组苹果脚本，用于处理表盘和电脑上各种媒体程序之间的交互。这允许用户更容易地为他们想要的任何软件编写他们自己的脚本。虽然这可能读起来像一个产品评论，但表盘实际上是开源的！

[https://www.youtube.com/embed/mPxt0JK9kQ4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mPxt0JK9kQ4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)