# 这是什么，蚂蚁用的微控制器板？

> 原文：<https://hackaday.com/2014/10/21/what-is-this-a-microcontroller-board-for-ants/>

你们年轻人可能不记得这个了，但是几年前 Kickstarter 上有一场军备竞赛，要创造最小的 Arduino 兼容微控制器板。从那时起，一些人意识到他们可以通过欺诈或土豆沙拉在 Kickstarter 上赚更多的钱，创造最小“duino 板”的比赛逐渐结束。

很遗憾[美珠]没有参与 Kickstarter 的大型微型 arduino 化项目，[，因为这个项目本可以赢得](http://hackaday.io/project/3117-a-even-smaller-nanite)。这是一个 Atmel ATtiny85，带有 USB 端口、电阻器、二极管、复位按钮、LED 和引脚接头，*比 tiny85 的 PDIP 封装大 72 密耳。*除了得到一个“tiny85s”的裸骰子之外，这个棋盘不太可能变得更小。

[Meizu]从[[Tim]的 Nanite 85](http://hackaday.com/2014/05/07/the-smallest-attiny85-based-usb-board/)中获得灵感来创建该板，直到几天前，该板还是微型微控制器板的当前冠军。在 KiCAD 中做了一点工作，新的电路板布局就创建出来了，只比 PDIP ATtiny85 的 0.4”x 0.4”尺寸大一点点。要得到这么小的工作板有一些挑战；你可能会惊讶引脚接头周围的塑料块有多大，但通过一些非常巧妙的焊接，[美珠]能够让它工作。