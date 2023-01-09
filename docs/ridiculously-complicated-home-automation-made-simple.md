# 荒谬复杂的家庭自动化变得简单

> 原文：<https://hackaday.com/2015/02/12/ridiculously-complicated-home-automation-made-simple/>

[Eric T]写了他的[疯狂全面的家庭自动化设置](http://www.instructables.com/id/Uber-Home-Automation)。当他的狗吠叫时，最初是一种通知他的方法，后来发展成为一个全屋的 Arduino 供电的传感器盛会。我们之前已经从这篇庞大的文章中看到了两个不同的步骤。一个[让他的狗](http://hackaday.com/2014/11/08/dog-tracker-knows-where-the-dirt-is/)自动化，另一个专注于[的 Wink hub，以连接智能灯泡等商业硬件](http://hackaday.com/2015/01/08/using-the-wink-hub-with-openhab/)。现在让我们从整体上来看这个项目。

该项目的基本框架实际上非常简单。他用 Arduino、RFM69 无线电单元和连接到 Raspberry Pi 的以太网屏蔽制作了一个无线电网关基站，以提供 GUI 界面。开源家庭自动化项目 [OpenHAB](http://openhab.org) 让这一切都可以通过浏览器或智能手机实现。

接下来，他用 Arduino 和 RMF69 无线电制造了额外的传感器节点。这些传感器节点可以彼此分离，这使得[Eric]能够随着时间的推移逐步扩展他的系统。

特别感兴趣的模块是优步传感器和[洗衣机-烘干机模块](http://www.instructables.com/id/Uber-Home-Automation-w-Arduino-Pi/step13)。对于优步传感器，[埃里克]基本上把他能找到的所有传感器都扔向了一个 Arduino 它发送噪音水平、亮度、运动、温度、湿度以及烟雾、火焰或可燃气体的存在。其中一些情况会触发电子邮件警报，而其他情况则被简单地存储起来以备将来查看。

在更简单的一端，他使用噪音水平检测器来检测洗衣周期的结束，然后触发通知。聪明的是，当一个附加的运动探测器触发时，这条信息会自动清除，大概是因为有人去地下室清空烘干机了。非常整洁。

16 简单的 Arduino 库和可在 Ebay 上购买的廉价硬件模块的出现，基本上使所有这一切变得实用和经济。如果你对 DIY 家庭自动化项目感兴趣，这款产品值得一看，以获取灵感和一个很好的概述。