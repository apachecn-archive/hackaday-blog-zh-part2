# 欺骗汽车音响以为你的手机是录音机

> 原文：<https://hackaday.com/2015/08/13/tricking-a-car-stereo-to-think-your-cellphone-is-a-tapedeck/>

当你有一辆旧车时，在库存音响部门没有太多选择，通常你只能得到一台 CD 播放器和一个磁带卡座。当你想用手机播放音乐时，你会怎么做？购买适配器或新的主机并不好玩。那么为什么不黑掉它呢？这不仅仅是蓝牙加密狗和老年立体声音响的机械结合。一些真正的工作进入说服立体声，BT 接收器是股票磁带走带设备。

![car-stereo-logic-analyzer](img/e98098c57a00fcee995f74c8fa8df9e3.png)攻击过时的卡式录音机【kolonelkadat】知道在齿轮和叶片的迷宫中，大部分都在移动，启动开关，让收音机知道里面有磁带，它可以切换到那个输入并播放。欺骗收音机以为有磁带插入是由 Arduino 处理的。使用逻辑分析仪[kolonelkadat]计算出原始单元输出的逻辑信号，并将其复制到他的 Arduino 代码中。

音频由蓝牙扬声器的内部进行处理，输出被重定向到收音机，从磁带头发出的信号通常会被定向到收音机。休息之后，请加入我们，观看几个视频，了解所有细节。

[https://www.youtube.com/embed/AZ5rok6ThZo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AZ5rok6ThZo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/xgWfCX4zc00?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xgWfCX4zc00?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)