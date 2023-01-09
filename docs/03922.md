# 构建以太网连接的 RFID 阅读器

> 原文：<https://hackaday.com/2013/08/26/building-an-ethernet-connected-rfid-reader/>

[![](img/6a7ff446f430536704a55dceb664c106.png)](http://hackaday.com/wp-content/uploads/2013/08/kdqktmch.jpg)

在过去的几年里，[Lt_Lemming]是布里斯班黑客空间的主席。直到几个月前，对本地的访问还需要使用 125KHz 的 RFID 标签和一个带原型屏蔽的 Arduino 板。随着黑客空间成员的增加和设施的迁移，[Lt_Lemming]决定为自己建造一个更加紧凑和先进的平台。

他的简单可联网 RFID 控制器(SNARC)是一个平台，可以连接到以太网和不同的 RFID 阅读器，以实现智能访问控制功能。通孔组件是精心挑选的，所以即使是焊接学徒也可以组装它。PCB 采用 Fritzing 设计，开发甚至可以在 Arduino IDE 内部完成，因为板上提供 ISP 和串行接口。最后，一个 N 沟道 mosfet 控制门锁机制。

该项目是开放的硬件和软件，所有源代码都可以从[Lt_Lemming]的 [github repo](https://github.com/LemElec/SNARC_PTH_V1.3) 下载。