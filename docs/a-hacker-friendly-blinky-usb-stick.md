# 一个黑客友好的 Blinky 盘

> 原文：<https://hackaday.com/2015/03/16/a-hacker-friendly-blinky-usb-stick/>

智能 RGB LED 的出现，无论是作为单独的单元，作为条带，甚至作为面板，都使得具有各种颜色控制和过渡效果的 blinky 灯光项目易于使用最简单的控制器来实现。允许控制这些智能 led(或有时被称为智能像素)的库使得软件开发相对容易。

奥地利维也纳 Metalab hackerspace 的[overflo]最近完成了对 [usblinky 的开发，这是一款对黑客友好的 blinky 盘](https://metalab.at/wiki/Usblinky)。通过外部电源供电时，它可以控制多达 150 个 WS2812B 智能 LED，通过计算机 USB 端口供电时，它可以控制多达 20 个 LED。微控制器是运行[微核](https://github.com/micronucleus/micronucleus)引导程序的 ATTiny85，该引导程序使用 [vUSB](http://www.obdev.at/products/vusb/index.html) 实现软件 USB。硬件基于 [DigiSpark](http://digistump.com/wiki/digispark/tutorials/connecting) 平台。usblinky 软件源代码可以在他们的 [Github repo](https://github.com/hackerspaceshop/usblinky) 上获得。关于陷阱和经验教训的部分是有趣的读物。

Metalab 计划围绕这个小设备举办研讨会，让孩子们开始编程，因为它足够简单，并提供快速的视觉反馈来帮助您入门。为了圆满完成整个项目，[overflo]使用 OpenSCAD 设计了一个可定制的，3D 可打印的[参数球](http://www.thingiverse.com/thing:661318)，它可以容纳 LED 灯条，并制作一个漂亮的外壳或迷幻的夜灯。休息之后，请查看 usblinky Orb 的迷人视频。

感谢[papst]发送此提示。

[https://www.youtube.com/embed/cYPhyNVSkh4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/cYPhyNVSkh4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)