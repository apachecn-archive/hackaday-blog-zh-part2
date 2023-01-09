# Bootloader 为 ATtiny85 带来 USB、固件更新

> 原文：<https://hackaday.com/2012/10/09/bootloader-brings-usb-firmware-updating-to-the-attiny85/>

![](img/9d90fc76ace50e2635474ed5ec35f98b.png "vusb")

[Jenna]发送了一个非常酷的引导程序，她认为人们可能会喜欢。它被称为[微核](https://github.com/bluebie/micronucleus-t85)，它将不起眼的 ATtiny 85 变成一个带有 USB 接口的芯片，能够通过“病毒”上传程序进行升级。微核的重量刚刚超过 2 kB，是目前最小的 USB 兼容引导加载器之一。

USB 支持来自于 [V-USB](http://www.obdev.at/products/vusb/index.html) ，这是一个将虚拟 USB 端口放在一套 AVR 微控制器上的项目。使用 V-USB，很容易将 Tiny85 变成键盘、自定义操纵杆、数据记录器或计算机附带的 LED 显示器。

微核的一个非常有趣的特征是“病毒更新者”特征。该功能获取一个新的固件，并将其写入 Tiny85，从而禁用当前的引导加载程序。如果你正在设计一个项目，应该有一种通过 USB 而不是通常的 AVR 程序员来更新固件的方法，这可能是你的引导程序。

对于一个强调小代码大小的引导装载程序来说还不错。在刚刚超过 2 kB 的情况下，可以在类似的、更小的、更便宜的 ATtiny45 上使用这个引导程序。