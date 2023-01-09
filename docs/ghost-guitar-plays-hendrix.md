# 幽灵吉他演奏亨德里克斯

> 原文：<https://hackaday.com/2015/07/30/ghost-guitar-plays-hendrix/>

> 紫色的阴霾充斥着我的大脑，
> [最近的吉他看起来不一样了](http://wp.josh.com/2015/07/28/self-strumming-ghost-guitar/)，
> 【乔希】演奏得很有趣，但我不知道为什么
> 在他通电时打扰我。

[Josh]想尝试用不同的方式弹吉他。我们已经见过一些使用伺服系统演奏的吉他黑客，以及用薄膜电位器代替琴弦的基于 T2 Arduino 的吉他，但是他决定尝试一种不同的方法。他利用永久磁铁和电磁效应来弹奏琴弦。

> 四周都是紫色的薄雾，所有的放大器都在上下跳动。我的琴弦是向左还是向右？
> 不管是什么，电磁把我推得看不见了。

为了做到这一点，他把一块大的永久磁铁放在绳子旁边，让交流电通过绳子本身。当电流和磁场相互作用时，弦被推动，[，就像马达的轴承](https://en.wikipedia.org/wiki/Fleming%27s_left-hand_rule_for_motors)。当电流流向另一个方向时，弦被推向相反的方向。因为他使用交流电(通过连接到频率发生器的 MOSFET 驱动)，他能够控制频率，并找到使琴弦共振的频率，包括赋予吉他独特声音的谐波。这是一个非常巧妙的攻击，但不要忘记他正在处理相当多的电流:如果你不小心触碰到绳子并将其接地，电路中的电流足以杀死你。

> 是的，[乔希]的黑客是[所有关于右手法则](https://en.wikipedia.org/wiki/Fleming%27s_left-hand_rule_for_motors)，
> 我知道他不是黑客傻瓜，
> 你已经得到了我的 E 弦共鸣，共鸣如此之好
> 只是不要碰它，否则你会结束你的时间
> 帮助我，耶，紫雾！

(向[吉米·亨德里克斯]的鬼魂道歉，吉他黑客至尊)

[https://www.youtube.com/embed/p_qayCRUdlU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/p_qayCRUdlU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/fjwWjx7Cw8I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fjwWjx7Cw8I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)