# 具有软件无线电的 GSM 基站

> 原文：<https://hackaday.com/2014/07/05/a-gsm-base-station-with-software-defined-radio/>

如果你想知道如何获得更好的手机信号，或者只是想建立自己的私人手机网络，这款手机就是为你准备的。[这是一个 GSM 基站，由一个比格犬骨黑](http://discourse.criticalengineering.org/t/howto-gsm-base-station-with-the-beaglebone-black-debian-gnu-linux-and-a-usrp/56)和一个不太贵的软件无线电板制成。

这一构建的关键组件显然是软件定义无线电。[Julian]在这个项目中使用了一台 USRP B200 无线电。它并不便宜，但它是一个非常好的硬件，可以用 GNU Radio 做任何事情。该板由 BeagleBone Black 控制，这是一个非常便宜的解决方案，硬件总成本约为 750 美元。

构建的软件部分主要由 [OpenBTS](http://www.openbts.org/) 处理，OpenBTS 是基站软件部分的开源项目。它控制收发机，打电话和发短信，以及所有其他基站做的后端工作。OpenBTS 还支持 Asterisk，这是 PBX 和 VoIP 设置的首选软件。运行这个程序，你就可以在地球上的任何地方用你的装备了 SDR、支持互联网的 BeagleBone Black 打电话和发短信。