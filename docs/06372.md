# THP 入门:一个无线 Bootloaders 和 Linux 构建系统

> 原文：<https://hackaday.com/2014/06/23/thp-entry-a-wireless-bootloaders-and-linux-build-systems/>

有了 Hackaday 大奖，你不仅仅局限于一次参赛。当然，如果你在竞争一次太空之旅，把你的时间和精力只投入到一个项目上会更好，但是如果你是[死灵法师]，你可能会从事两个高度相关的项目，这两个项目都足以获得 Hackaday 奖

[死灵]的第一个项目[是 rf24boot](http://hackaday.io/project/1585-rf24boot%3A-The-NRF24L01-bootloader) ，一个使用非常便宜和非常受欢迎的 NRF24L01 2.4GHz 无线模块的空中引导加载器。有很多很多项目使用 XBees 和 NRF24 将无线引导加载添加到微控制器中，但[死灵]在这个项目中做了一些不同的事情:他正在构建对各种微控制器的支持，包括 STM32、MSP430、PIC32、8051，当然还有 AVR 芯片，用于非常流行的 Arduino 兼容性。

对多种微控制器平台的支持是[死灵]获得 Hackaday 奖的另一项成果， [Antares，这是一个面向微控制器的 Linux 内核构建系统](http://hackaday.io/project/1470-Antares%3A-Linux-kernel-like-buildsystem-for-uCs)。Antares 背后的想法是将微控制器的代码编写与编译和烧录分开。可以把它想象成一个巨大的 makefile，它可以与任何东西一起工作，还包括一些用于公共项目的库。

Antares 支持的平台包括前面提到的流行的目标，并允许你使用任何你可能想要的 IDE。emacs？当然可以。月食？好极了。Arduino？你是个受虐狂。为了更好地了解 Antares [，你可以查看 Readme](https://github.com/nekromant/antares) ，或者[我们大约一年前发布的帖子](http://hackaday.com/2013/09/06/antares-one-bare-metal-build-system-to-rule-all-micocontrollers/)。

这都是非常酷的东西，很容易看到[死灵]正在研究的潜力。将这两者结合在一起，它几乎是一个完整的系统，用于开发我们一直听说的物联网——将代码上传到简单传感器的简单 AVR，并为您的臂式洗碗机或微波炉部署复杂得多的代码。