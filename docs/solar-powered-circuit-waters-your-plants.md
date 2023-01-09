# 太阳能电路浇灌你的植物

> 原文：<https://hackaday.com/2014/11/09/solar-powered-circuit-waters-your-plants/>

如果你想让你的植物保持健康，你需要确保它们得到浇水。[Dimbit]决定建造自己的[太阳能电路](http://hacksandbodges.wordpress.com/2014/11/08/solar-powered-automated-plant-waterer/ "solar powered plant waterer")来帮助自动保持他的植物健康。像许多事情一样，剥这只猫的皮不止一种方法。[Dimbit]之前见过其他[类似的](http://hackaday.com/2014/09/27/automated-watering-system-uses-neat-diy-water-valve/ "DIY watering valve") [项目](http://hackaday.com/2014/07/16/solar-powered-diy-plant-watering-system/ "Solar plant waterer")，但是他想让自己的比一般的浇水项目聪明。他还希望它消耗很少的能量。

[Dimbit]首先解决电源问题。他怀疑他的项目不需要超过 5V 的电压。他能够通过使用四个现成的太阳能花园灯来构建自己的太阳能电源。这些灯都有自己的低质量太阳能电池板和 AAA 镍氢电池。[Dimbit]设计并 3D 打印了他自己的塑料支架来固定所有的太阳能电池。所有的电池和电池组串联连接以增加电压。

接下来[Dimbit]需要一个电子可控水阀。他环顾四周，但无法找到任何现成的、只需很少能量就能工作的东西。他尝试了定制零件和现成零件的所有不同组合，但就是做不出完美密封的东西。这个解决方案来自一个不太可能的来源。

一天，当[Dimbit]用完洗衣液时，他注意到洗涤剂瓶盖上有一个完美的洞，应该可以用钢珠轴承密封。然后，他使用一个螺栓、一些电磁线和一个定制的 3D 打印外壳设计了自己的电磁铁。这些都与清洁剂盖配合在一起，形成了一个功能性的低功耗水阀。

实际电路运行在微芯片 PIC 微控制器上。系统被设计为一次睡眠大约九分钟。在睡眠周期后，它醒来并测试土壤中的探针。如果阻力足够低，PIC 知道植物需要水。然后，它打开定制的阀门，从重力供水系统中释放出大约两茶匙的水。几个周期后，即使非常干燥的土壤也能达到正确的湿度水平。请务必观看下面运行系统的视频。

[https://www.youtube.com/embed/DtDD8zL9SS4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DtDD8zL9SS4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)