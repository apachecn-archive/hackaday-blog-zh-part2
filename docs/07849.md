# 霍比特人的剑发出蓝光，征服无保护的无线网络

> 原文：<https://hackaday.com/2014/12/18/hobbit-sword-glows-blue-then-vanquishes-unprotected-wifi/>

虽然最初的刺闪着蓝色作为防御警报，但 Spark 的"[警告](http://blog.spark.io/2014/12/17/warsting-a-wifi-scanning-sword-for-hobbits/)"完全是关于侵略性的。该项目破解了一把玩具霍比特人剑，并教会它在检测到易受攻击的 WiFi 时发出蓝光。一旦得到警报，战斗就开始了。如果它的持有者挥砍，这把剑将与无助的网络战斗，摇摆和叮当作响，直到它从被击败的 DHCP 服务器获得一个 IP。一旦被征服，剑向火花的云发布“被征服”的消息，教剑从此忽略它。

虽然自第一部《指环王》电影问世以来，“驾车”并没有真正成为一件事，但我们上次看到有人做类似的事情时，硬件仅限于检测 WiFi，而不是连接。

Spark 首席执行官(扎克)选择了这把特殊的剑，因为它可以在不被切开的情况下拆卸，并且已经配备了易于破解的 led、运动控制和音效。自然，他添加了自己的产品之一——Spark Core——以将 WiFi 功能移植到武器上(一个更便宜的替代方案是您选择的 MCU 和新的 ESP8266)。该项目然后劫持 LED 照明，声音和击中检测传感器。一旦连接上，我们的读者可能会提出一些更有想象力的行动，尽管该项目的现有核心代码是在 Github 上发布的[。事实上，在许多司法管辖区，现在连一个不安全的 WiFi 都是非法的，所以要小心你当地的限制。](http://github.com/spark/warsting)

许多公司可以简单地用简单的方式做广告，虽然很明显是广告，但 WarSting 仍然是一个有创意和有趣的黑客。

见下面的视频剑在行动和火花的关于黑客的知识。谢谢[克里斯]的提示。

[https://www.youtube.com/embed/rmjkUv5OtLM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rmjkUv5OtLM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)