# RFID 阅读器从 3 英尺外窥探卡片

> 原文：<https://hackaday.com/2013/11/03/rfid-reader-snoops-cards-from-3-feet-away/>

安全研究员[弗兰·布朗]给我们发来了这个关于他的[美味 RFID 窃贼](http://www.bishopfox.com/resources/tools/rfid-hacking/attack-tools/)的提示，这种窃贼可以远距离偷偷窃取 RFID 卡上的信息。如果你以前用过无源 RFID，你会知道大多数阅读器只能在离卡几英寸的地方工作。在今年夏天[【弗兰】的 DEFCON 演讲中](http://www.youtube.com/watch?v=6VaG1mwoukQ)他称之为“抓屁股法”，试图让隐藏的天线离目标的钱包足够近。

他的解决方案采用现成的高功率阅读器，(如 [HID MaxiProx 5375](http://www.hidglobal.com/products/readers/hid-proximity/5375) )，并通过嵌入 12 节 AA 电池和一个定制的 PCB(使用 Arduino Nano 来解释阅读器的输出)，使其具有惊人的便携性。当读取器看到附近的卡时，信息通过 Nano 进行解析，数据被发送到 LCD 屏幕，并存储到可移动 microSD 卡上的. txt 文件中，供以后检索。

休息后有两个短视频:Tastic RFID 小偷的演示和快速查看其内脏。如果你正在考虑复制这个工具，并且你对阅读器的价格感到惊讶，你总是可以[尝试构建你自己的…](http://hackaday.com/2010/04/19/build-your-own-rfid-reader/)

[https://www.youtube.com/embed/gP9f_TiKHIY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gP9f_TiKHIY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Hc4y7givo_o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Hc4y7givo_o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)