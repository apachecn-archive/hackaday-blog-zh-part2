# 幼儿用的彩色时钟

> 原文：<https://hackaday.com/2015/02/24/a-colorful-clock-for-toddlers/>

[Don]和他的妻子正在寻找一种方法来教他们两岁的女儿如何看时间。她明白白天和黑夜的区别，但她还没有大到能够真正理解说出实际时间的地步。[Don]的解决方案是通过将时间分成代表不同任务或活动的[个彩色块](http://dhowdy.blogspot.com/2015/02/building-clock-to-help-kids-tell-time.html "A colorful clock for toddlers")来简化问题。例如，如果时钟是黄色的，这可能表明是时候玩了。如果是紫色，那就该收拾房间了。

[Don]从一个当地零售商那里买了一个价值 10 美元的小型电池时钟。这个简单的时钟有一个数字读数，在外壳内有一些多余的空间来放置额外的部件。它也足够重，可以放在柜台或架子上。唐打开时钟，开始用他的 Dremel 来释放一些额外的空间。然后他添加了一个 ShiftBrite 模块作为背光。 [ShiftBrite](http://hackaday.com/2009/06/29/parts-shiftbrite-rgb-led-module-a6281/ "ShiftBrite") 是一个高亮度 LED 模块，可通过串行控制。这允许[Don]将背光设置为他想要的任何颜色。

[Don]已经有一个 Raspberry Pi 运行他的 DIY 婴儿监视器，所以他选择劫持相同的设备来控制 ShiftBrite。[Don]开始使用 Hive13 GitHub repo 来控制 LED，但他发现它不适合这个项目。他最终放弃了这个项目并对其进行了修改。他的修改允许他设置特定的颜色，然后通过在命令行中键入一个命令来退出程序。

ShiftBrite 的颜色会根据系统的 crontab 中定义的时间表进行更改。[Don]安装了 Minicron，它提供了一个很好的 web 界面，使更改系统上的 cron 作业变得更加容易。现在[Don]可以根据需要通过网页轻松调整女儿的日程。