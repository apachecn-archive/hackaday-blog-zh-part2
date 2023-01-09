# 荷马机器人确保你不会错过一集

> 原文：<https://hackaday.com/2014/10/14/homer-robot-ensures-you-dont-miss-an-episode/>

随着我们忙碌的生活，谁有时间去关注电视节目的时间表？[Tamberg]当然没有，这就是为什么他想出了网络电视移除器，他称之为[智能荷马](http://www.instructables.com/id/Smart-Homer-Web-enabled-TV-remote/?ALLSTEPS)。这个神奇的装置知道《辛普森一家》何时播出，打开电视并切换到合适的频道。

像真正的荷马一样，这个玩具的脑袋里没有太多东西。几个红外线发射器被安装在瞳孔的位置，相关的电线向下延伸到他的体内。一个 Arduino 和以太网屏蔽就位于一个粉色甜甜圈和一个 Krusty 汉堡之间。这个电子二人组充当网络服务器，向网络寻找在线脚本。该脚本轮询在线电视节目指南，如果“辛普森一家”正在播放，它会向 Arduino 发送信号以打开电视。

![Homer Smart Remote](img/6d6b1d5ada329ac8cb8b343983647442.png) ![Jolly Homer](img/e7c562b184aa55a68a1bd70f3efac3f6.png)