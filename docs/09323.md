# 一个真正的卡车模拟器

> 原文：<https://hackaday.com/2015/06/18/a-real-dash-for-a-truck-simulator/>

[Leon]玩*欧洲卡车模拟器 2*，像任何好的模拟器一样，有人在那里建造控制台、驾驶舱和仪表板。在[莱昂]的例子中，他想要一个虚拟卡车[的仪表板，并用一辆大众 Polo](https://hackaday.io/project/6288-volkswagen-can-bus-gaming)的仪表板拼凑了一个。

这个项目的灵感来自于 Silas Parker 和他基于 Arduino 的仪表盘，它是由一个纸板盒、一些伺服系统和几个 led 组成的。这很有效，但[Leon]意识到，在过去十年左右的时间里，几乎所有的仪表盘都有 CAN 总线。你可以只为 Arduino 买一个 can 总线屏蔽,在任何垃圾场都能很容易地找到仪表盘。

现在，[Leon]正在寻找仪表盘上相关刻度盘和 led 的 CAN 总线地址。[他在 0x280](https://hackaday.io/project/6288-volkswagen-can-bus-gaming/log/19473-rpm-can-address-found) 找到转速表，[在 0x470](https://hackaday.io/project/6288-volkswagen-can-bus-gaming/log/19563-more-can-adresses-found) 可以找到一串指示灯。结合标准的电脑方向盘和*欧洲卡车模拟器 2* 的遥测 SDK，【莱昂】在他的桌子上有了一个虚拟大钻机的雏形。