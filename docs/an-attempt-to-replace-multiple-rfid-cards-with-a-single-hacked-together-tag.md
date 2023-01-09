# 试图用一个黑客攻击的标签代替多个 RFID 卡

> 原文：<https://hackaday.com/2013/01/21/an-attempt-to-replace-multiple-rfid-cards-with-a-single-hacked-together-tag/>

这是一个令人费解的标题，但[Hudson]试图用一个 AVR 芯片取代多个 HID Prox 卡并没有完全成功。当他想把工作中携带的 RFID 门禁卡的数量减少到只有一张时，这个项目就开始了。这些卡使用 HID 邻近协议，这与我们看到的大多数业余 RFID 项目中使用的协议略有不同。他最终选择了一个支持不同协议的 AVR 汇编文件，并根据自己的需要进行了编辑。

上面的设备是使用的完整替换标签[Hudson]。只是一个 AVR ATtiny85 和一个漆包线做的线圈。线圈从读卡器的磁场中获取电流，并通过输入引脚上的泄漏为芯片供电(我们已经见过[这种把戏](http://hackaday.com/2009/06/27/avr-rfid-tag/) a [几次](http://hackaday.com/2011/05/20/using-an-avr-as-an-rfid-tag/))。他的想法是在设备上存储多个代码，并连续发送。他能够让标签只为一个代码工作，但是 HID Prox 阅读器的细节使得发送多个代码变得困难，如果不是不可能的话。卡片必须连续两次发送相同的代码，然后从磁场中移开，阅读器才会查询另一个组合。