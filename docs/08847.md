# 启动基于路由器的开发板

> 原文：<https://hackaday.com/2015/04/21/kickstarting-router-based-development-boards/>

[Squonk]在再利用路由器领域相当有名，几年前它对 TP-Link 的 TL-WR703N 无线路由器进行了逆向工程。有了这些知识，[他为互联网上的事物开发了一个开放平台](https://www.kickstarter.com/projects/706167548/dominoio-an-open-hardware-wifi-platform-for-things)叫做 Domino。这和你破解在阿里巴巴上购买的路由器所得到的几乎一模一样，只是包装更方便，有更多的针脚。

Domino 建立在[Squonk]对 TP-Link TL-WR703N 无线路由器的逆向工程工作的基础上，这款路由器从 Linksys WRT54G 那里抢走了所有这些可爱的嵌入式黑客的风头。703N 和 Domino 都是围绕 Atheros AR9331 构建的。虽然该芯片组的路由器版本只突破了几个 GPIO 和其他有趣的引脚，但 Domino 几乎突破了所有东西——GPIO、JTAG、I2S、UART、SPI、USB 和以太网可以在设备上找到。

向 Kickstarter 活动认捐 25 美元，就有希望得到基本的多米诺骨牌。这比 WR-703N 的正常价格要低一点，[如果你把路由器放在帽子里](http://hackaday.com/2014/08/01/defcon-shenanigans-hack-the-hackaday-hat/)，这可能是值得的。有几个高级版本包含 ATMega32u4 微控制器，使其与 Arduino Yun 兼容。