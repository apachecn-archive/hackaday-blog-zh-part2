# 用逆向工程制作无接触振动器

> 原文：<https://hackaday.com/2012/11/25/making-a-touchless-vibrator-with-reverse-engineering/>

这是给外面的女士们(我猜也是男士们)的。

[贝丝]最近为自己买了一个 LELO 林珈安振动器，但发现操作这个无线振动器是一种扼杀情绪的尴尬。想要一个更自然的界面，她决定对一个遥控振动器进行逆向工程。这里有一个[缓存](http://scanlime.org.nyud.net/2012/11/hacking-my-vagina/)；[Beth]的博客一整天都在起起落落。

LELO 林珈安配有一个霓虹粉红遥控器形式的无线控制。[Beth]认为这个遥控器有点笨重，想给 VCR 编程——她不喜欢在性玩具中使用。为了改进这款遥控器并提供更好的用户体验，[Beth]拆掉了这款遥控器，开始自己动手制作。

新的震动遥控器必须是无触摸的——没有什么比按按钮更能破坏气氛了。通过使用超声波传感器，[贝丝]将能够通过简单地挥动她的手来控制她的振动器的强度；更加自然的界面。有了控制接口，剩下唯一要做的事情就是弄清楚如何控制振动器的业务端。

股票 LELO 林珈安遥控器配有一个 MSP430 微控制器和一个通过 SPI 接口控制的 2.4 GHz CC2500 无线电。[Beth]决定嗅探 SPI 总线并制作自己的控制器，而不是拆卸微控制器并从头开始计算固件。

在将一些 0.1”接头连接到 stock remote 并将一些电线焊接到微控制器后，[Beth]用 Propeller 开发板捕获了 SPI 数据。通过将 SPI 数据流传输到一个终端，她能够准确地了解遥控器是如何工作的，并着手建造自己的遥控器。

新的遥控器是由 Arduino Pro Mini、超声波传感器、CC2500 无线电和四位 7 段显示器组成的。打印完附件后，[Beth]有了一个非常容易使用的免提振动器。

在休息后的视频中，你可以看到[Beth]的振动器在工作。她仍在寻找更多的方法来改进它，例如用锁相环预测她的手的动作，但现在我们只是向贝丝致敬，这是一次非常棒的黑客攻击。

[https://www.youtube.com/embed/QhXoYcwsEVI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QhXoYcwsEVI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)