# 硬盘变成硬盘活动灯；不存储数据

> 原文：<https://hackaday.com/2015/03/15/hard-drive-becomes-hard-drive-activity-light-stores-no-data/>

不久前,[Frank Zhao]在一个水族馆里建造了一台计算机。这正是你所期待的——一堆零件被塞进一个装满矿物油的容器里。是的，里面有 i7 和 GTX970，但也有一堆新像素和一个整洁的小气泡宝箱。这对[Frank]来说还不够，他还想增加一个硬盘活动监视器。固态硬盘最荒谬的活动监视器是什么？[当然是老式的基于盘片的驱动器](http://eleccelerator.com/naked-hdd-activity-indicator/)。

建造过程相对简单，而且是[弗兰克]在一天内用零部件组装而成。在打开一个旧的 PATA 硬盘驱动器后，硬盘驱动器臂的音圈通过几个 MOSFETs 连接到主板的 HDD 活动信号。盘片电机由一个 [MTD6501](http://www.microchip.com/wwwproducts/Devices.aspx?product=MTD6501C) 电机驱动器控制，设置为当电路接通时旋转。

就控制硬盘驱动器的组件而言，这是一台组装机，但这并不是重点。这只是一个显示水族馆计算机中的 SSD 何时被访问的简洁项目。也就是说，活动监视器目前是断开的，因为旧的硬盘驱动器是如此的吵。不过，看起来真的很酷。