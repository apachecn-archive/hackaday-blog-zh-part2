# 比格犬 PRU 简介

> 原文：<https://hackaday.com/2014/06/22/an-introduction-to-the-beaglebone-pru/>

虽然 BeagleBone 通常被比作 Raspberry Pi，但它的一些特性使它成为一台功能强大得多的单板计算机。处理器的能力略有不同，但 BeagleBone 的真正力量来自可用的 pru:两个小内核使 BeagleBone 的硬件相当于 bitbanging 引脚。[Texane]提供了两个关于在 BeagleBone 中使用 PRU 的很棒的教程，应该是每个 BeagleBone 所有者的必读书目。

[第一篇教程](http://www.embeddedrelated.com/showarticle/586.php)讲述了 BeagleBone 中 PRU 的功能，以及设置软件环境来开发您自己的与 PRU 的硬件接口。虽然为 PRU 编写代码通常涉及[的 Beagleboard 包](https://github.com/beagleboard/am335x_pru_package)，但 TI 最近[发布了 Code Composer Studio](http://www.element14.com/community/community/knode/single-board_computers/next-gen_beaglebone/blog/2014/04/30/bbb--pru-c-compiler) 版本，该版本提供了为 PRU 编译 C 代码的选项。

[【Texane】使用这个 C 编译器](http://www.embeddedrelated.com/showarticle/603.php)重新编写了早期的纯汇编 PRU 程序，使得开发变得非常容易。仍然有一点内联汇编，内联汇编支持没有 GCC 中那么先进，但它仍然比只汇编的变体容易得多。

虽然[Texane]正在使用他的 BeagleBone 中的 PRU 在同步加速器设施中开发一些东西，但有三样东西可以派上用场:它可以用来制作老式 mac 电脑的视频卡，或者 T2 的任何 VGA 视频卡。非常酷的东西，特别是现在你可以用 c 写东西了。