# THP 四分之一决赛:WALLTECH 智能手表

> 原文：<https://hackaday.com/2014/09/17/thp-quarterfinalist-walltech-smartwatch/>

虽然有很多关于一家大公司推出新的可穿戴产品的炒作，但我们对[Walltech]的开源有机发光二极管智能手表更感兴趣。Hackaday 奖的参赛作品将一系列传感器和一个有机发光二极管屏幕合并到一个可穿戴设备中，该设备可以通过蓝牙低能耗与智能手机对话。

该设备基于 BTLE 的开发板。这个微小的 Arduino 克隆体包含一个惯性测量单元(IMU)、一个 Nordic nRF8001 蓝牙无线电和一个 ATMEGA32u4 微控制器。

1.5 英寸的有机发光二极管显示屏来自基于 [SSD1351](http://www.buydisplay.com/default/serial-spi-1-5-inch-color-oled-display-128x128-graphic-module-ssd1351) 制造 [OLED 模块](https://www.tindie.com/products/miker/15-color-oled-spi-display-33v-50v/?pt=directsearch)的【miker】。一个 [STP200M](https://www.tindie.com/products/NiceRF/iic-interface-embedded-3d-pedometer-module-stp201m-for-wrist-pedometer-products-/) 3D 计步器在一个小包装中提供活动监测。

在硬件方面，将所有这些组件包装成适合你手腕的东西是相当困难的。原型硬件主要由现成的组件构建而成，但仍能达到手表大小。

在这一点上，看起来代码是剩下的主要挑战。有很多功能可以实现，而且[Walltech]甚至提到它被设计成非常可定制的。它甚至支持 AndroidApple Watch 做不到这一点。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[黑客日奖的四分之一决赛。](http://hackaday.io/list/2864-The-Hackaday-Prize%3A-Semifinalists)**