# 双轴太阳追踪器总是被晒黑

> 原文：<https://hackaday.com/2014/03/29/2-axis-solar-tracker-always-gets-a-tan/>

让我们面对现实吧——太阳能电池板仍然没有那么高效。那么，为什么不从它们身上榨出尽可能多的汁液呢？建造一个 [2 轴太阳跟踪单元](https://polyideas.com/post/137926811349/building-the-solarbot-a-18-month-journey-as-a)可以增加 30%左右的日发电量！

[Jay Doscher]早在 2011 年就停电了，尽管只有 12 个小时，但他们意识到他们在应对停电时准备不足。食物变质了，手电筒没电了，蜡烛稀少了……他们需要为下一次发生这种事情做更好的准备。这催生了杰伦在他的博客上持续时间最长的项目之一。

他的目标是建立一个全自动的太阳能跟踪装置，可以安装在任何地方，并自动跟踪太阳，以确保最佳的光线捕捉。它使用 12V 齿轮减速电机来提供平移，并使用带位置跟踪的线性致动器来控制倾斜。为了追踪太阳，他有一个数字罗盘和一个 Adafruit Ultimate GPS 分线板。为了控制它，他使用的是一个 Arduino UNO，但他已经经历了多次迭代，包括他的第一个比格犬骨。这是一个非常巧妙和设计良好的系统，杰伊希望将它推广到全世界——整个系统都是开源的。好家伙！

它还没有完全完成，但是他有[一个惊人的构建日志](http://www.polyideas.com/blog/2014/3/27/building-the-solarbot-a-18-month-journey-as-a-maker)和一个充满信息的 [GitHub 库](https://github.com/polyideas/Outdoor_Solar_Robot)——加上下面的视频展示了它的当前状态！

[https://www.youtube.com/embed/wIDUBpB8a5U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wIDUBpB8a5U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果你想买一个便宜的太阳能追踪器，看看这个[婴儿大小的太阳能追踪器](http://hackaday.com/2009/10/01/solar-tracking-without-overkill/)，它也使用 Arduino！或者这个用五金店的零件组装的[怎么样？](http://hackaday.com/2013/07/21/hardware-store-goods-and-an-mbed-combine-help-solar-panels-track-the-sun/)