# Brewdoo 有助于保持办公室咖啡新鲜

> 原文：<https://hackaday.com/2015/04/25/brewdoo-helps-keep-the-office-coffee-fresh/>

直到午饭时间，我们办公室的咖啡都喝得很快。不过，只有少数人会喝到下午，当我们需要 4 点钟提神时，谁也不知道咖啡放了多久。安装一个像[Paul]的 [Brewdoo](http://whirlingchair.com/brewdoo-a-coffee-age-timer.html) 这样的咖啡计时器来记录这些事情会很棒。

Brewdoo 干净简洁的设计让办公室里的任何人都能轻松使用。[Paul]的办公室有两个玻璃瓶，所以每个玻璃瓶都有一个按钮、一个 RGB LED 和 LCD 上的一条线。煮好一壶后，按下相应的按钮，计时器就会重置。RGB LED 开始时为绿色，但在一个小时内会变成黄色并最终变成红色。Brewdoo 也有一个故障保护装置:如果计时器四个小时没有重置，它的 LED 就会关闭，LCD 会显示一个问号。

[Paul]知道他不能接触现有的系统，因为他的公司租赁了设备，所以 Brewdoo 生活在一个外壳中，[Paul]用定制的 g 代码进行数控加工，并用硬盘驱动器磁铁固定在酿造机器上。虽然[Paul]设计了 Arduino Uno 以便于测试和代码修改，但 Brewdoo 有一个 328P 的定制 PCB。代码、Fritzing 图和 Eagle 文件在[Paul]的[GitHub](https://github.com/kerchen/BrewDoo)上。