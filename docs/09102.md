# 禁果机

> 原文：<https://hackaday.com/2015/05/22/forbidden-fruit-machine/>

这是另一个例子，说明了当今的快速原型技术是如何让艺术家和工匠快速而轻松地创作出交互式艺术作品的。[Kati Hyypa]和[Niklas Roy]联手将一幅经典画作转变成一场互动展览。这是一幅画着亚当、夏娃和苹果的画，还附有一个操纵杆。观众可以用操纵杆控制苹果的命运，从而探索这幅画。

“禁果机”是基于【科内利斯·科内利斯·范·哈勒姆】于 1592 年创作的一幅名为[《人类的堕落》](https://www.rijksmuseum.nl/en/collection/SK-A-129)的画作。这幅画描绘了伊甸园中的夏娃和亚当被蛇诱惑去吃禁果。这幅画的公共领域高分辨率扫描可以从阿姆斯特丹国立博物馆下载。从那开始，手臂被编辑掉，代之以由伺服系统驱动的铰接版本(安装在丙烯酸上)。苹果被安装在由两个步进电机驱动的 X-Y 台架上。这些由一个马达护罩驱动，该护罩由一个 Arduino Uno 控制。Uno 还控制一个 Music Maker shield 来播放各种音轨和音效。最后，额外的 Arduino Pro-Mini 用于通过达林顿驱动器控制 LED 照明效果，并连接到 X-Y 机架的终点挡板。操纵杆连接到 Uno 的模拟端口。

LED 给出了使用操纵杆移动苹果的线索，按下红色按钮会播放适当的音频或声音效果。例如，在夏娃和亚当的脚边按下猫上方的按钮会发出令人心碎的喵喵声，而让夏娃吃苹果会产生包括雷雨在内的更戏剧性的效果。

这台机器是开源的，代码发布在 [Github](https://github.com/royrobotiks/ForbiddenFruitMachine) 上，3d 文件发布在 [Youmagine](https://www.youmagine.com/designs/forbidden-fruit-machine-xy-gantry-mechanism) 上。休息后看一段视频。有些读者可能对这位艺术家的名字很熟悉——这是因为他们都在我们的博客上展示了他们的早期作品，例如这个[超棒的吸球机](http://hackaday.com/2014/03/23/this-machine-sucks-balls/)和[另一个也是](http://hackaday.com/2014/07/04/another-ball-sucking-machine-leaves-you-wanting-more/)。

[https://player.vimeo.com/video/128072915](https://player.vimeo.com/video/128072915)