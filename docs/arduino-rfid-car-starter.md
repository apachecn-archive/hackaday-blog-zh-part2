# Arduino RFID 汽车启动器

> 原文：<https://hackaday.com/2013/12/08/arduino-rfid-car-starter/>

[Pierre]最近买了他的第一辆车，并决定为它制作自己的 [RFID 电动启动器！](https://www.youtube.com/watch?v=bxU4K-7F5sI)

Arduino Nano 控制两个继电器，这两个继电器依次可以打开、启动和关闭汽车。他没有添加“一键启动”按钮，而是选择了 13.56MHz 的 RFID 模块。现在，当他将他的 RFID 徽章穿过仪表板时，汽车就会启动——如果它保持在那里超过一秒钟，汽车就会启动。再传一遍，它就关了。

他的最终目标是将这条电路重新定位到更靠近方向盘的位置，并使用一个 [NFC 环](http://nfcring.com/)来启动它！到目前为止，他把所有部件都藏在车内装饰下面，做得非常出色，你看不出有什么不对劲！休息之后请看视频中的演示。

[https://www.youtube.com/embed/bxU4K-7F5sI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bxU4K-7F5sI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

虽然他使用 NFC 戒指的目标令人钦佩，但我们的一位读者几年前更进了一步，在他的手中植入了一个 [RFID 标签，启动了他的汽车！](http://hackaday.com/2010/01/14/start-the-car-with-a-wave-of-your-hand/)就个人而言，我们更喜欢【皮埃尔的】方法。