# 地下室木材干燥窑

> 原文：<https://hackaday.com/2014/09/27/extrinsic-motivation-basement-wood-drying-kiln-2/>

很久很久以前，一个木工遇到了另一个木工，他碰巧有一个树木生意。他们达成了一项协议，规定第一个木工将烘干第二个木工提供的锯材，双方将分享木材。这正是发生在[Tim]身上的事情，这导致[他进入了 Hackaday 奖](http://hackaday.io/project/2030)。

[Tim]很好地解释了他建造窑炉的过程、他的控制以及操作要点。这个想法是以恰到好处的速度将水分从木材中抽出。否则，电路板可能[在外部检查](http://www.vermonttimberworks.com/learn/wood-textures/shake-checking/)，在内部出现蜂窝，或者承受残余张力。他使用除湿器将干燥空气泵入窑中，并使用控制系统监控窑中的相对湿度，并将原料干燥至含水量在 6-8%的范围内。

这座窑是由[Tim]根据自己的需要切割的有轻微瑕疵的托盘架搭建而成的。他用 1/2 英寸的绝缘板蒙皮，用铝带密封，并计划添加金属片来保护绝缘。

[Tim]想要控制风扇和除湿器，监控窑内的相对湿度，记录数据，并将其发送到互联网。为此，他使用了 Arduino Due、DHT-22、RTC、中继板、以太网屏蔽和 LCD 来显示正在发生的事情。硬件都在这一点上工作，软件正在路上。看看下面他的参赛视频。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png)这个项目是[正式进入](http://hackaday.io/submissions/prize/list)hack aday 奖，遗憾的是[没有进入四分之一决赛选择](http://hackaday.io/list/2864-The-Hackaday-Prize%3A-Semifinalists)。这仍然是一个伟大的项目，它本身就值得在 Hackaday 上发表。

[https://www.youtube.com/embed/CA3SO7-P0So?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CA3SO7-P0So?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)