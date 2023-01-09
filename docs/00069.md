# 用遗传算法构建单词时钟

> 原文：<https://hackaday.com/2012/04/10/building-a-word-clock-with-genetic-algorithms/>

[![](img/6c12036ab8dbcb7aec3d0342a130bb66.png "wordclock")](http://hackaday.com/wp-content/uploads/2012/04/wordclock1.png)

也许这是他遇到的语言障碍，或者可能是他倾向于用困难和聪明的方式做事，但我们真的很喜欢(阿莱西奥)为他的单词钟建造显示屏。他没有依赖预先设计的单词布局，而是用遗传算法制作了[自己的单词模式。](//miniaturegiantspacehamster.blogspot.com/2011/03/building-word-clock-part-1-genetic.html)

在查看互联网上的其他单词时钟时，[Alessio]注意到所有的 DIY 副本都使用了与原始 [QLOCKTWO](http://www.qlocktwo.com/) 单词时钟相同的字母模式。原因显而易见，其中最主要的是懒惰，但是阿莱西奥决定做得更好。他用 [JGAP](http://jgap.sourceforge.net/) 做了一个 10×10 的德语单词钟和一个 11×11 的英语单词钟。

[Alessio]的算法采用了一系列正则表达式——“过去四分之五”和“四分之五”都是 4:05 的有效表达式——并将解决方案组合在一起，希望得到最佳解决方案。[阿莱西奥]的方法还有一个额外的好处，就是能够产生非方形字时钟。在他的项目页面上，[Alessio]展示了圆形、三角形和菱形单词钟的例子。

[Alessio]最终用 Arduino Nano、DS1307 实时时钟、RGB LEDs 和几个移位寄存器构建了一个 10×10 平方的德语单词时钟。对于一个定制设计的单词时钟来说，这是非常好的工作。