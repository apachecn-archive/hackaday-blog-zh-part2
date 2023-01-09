# 更多小型无线电模块，满足您的无线需求

> 原文：<https://hackaday.com/2012/08/23/more-small-radio-modules-for-your-wireless-needs/>

为了永无止境地追求微控制器项目的廉价无线通信，[kiu] [推出了一款小型电路板](http://www.schoar.de/tinkering/rfm12trx/)，它允许通过 433MHz 无线电链路进行串行通信。

[kiu]的收发器使用一个网上仅售几美元的 RFM12 无线模块。该模块旁边是一个 ATMega8 和一个 USB 转串行 FTDI 芯片。当[kiu]将这个板插入他的计算机时，他能够运行一个终端，连接到这个板，并以 115，200 bps 的速率从这些板中的另一个接收和发送十六进制值。

根据[kiu]的 BOM，10 块电路板只花了他 180 欧元，约合 225 美元。考虑到 XBee 等现成的解决方案很容易就要贵两倍，我们认为[kiu]在这方面做得非常好。

[kiu]把所有的电路板文件、原理图和代码[放到他的 GitHub](https://github.com/kiu/rfm12trx)上，准备好供你阅读。一个非常酷的建筑，对于高空气球，火箭或者无线传感器非常有用。