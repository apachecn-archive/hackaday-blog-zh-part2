# 侵入无线电控制的插座

> 原文：<https://hackaday.com/2014/03/10/hacking-radio-controlled-outlets/>

毫不奇怪，现在有很多设备使用简单的射频通信，安全性极低。为了探索这一点，[戈登]看了一下[攻击无线电控制的插座](http://leetupload.com/blagosphere/index.php/2014/03/08/replay-attack-remote-control-outlets-and-rfcat/)。

他从一个 [CC1111 评估套件](http://www.digikey.com/product-detail/en/CC1111EMK868-915/296-22732-ND/1739551)开始，它支持 [RFCat](http://code.google.com/p/rfcat/) RF 攻击工具集。RFCat 允许您使用 Python 接口与 CC1111 进行交互。在[用 RFCat 固件](http://leetupload.com/blagosphere/index.php/2014/02/16/you-know-how-to-send-my-signal-setting-up-rfcat-from-scratch/)刷新 CC1111 之后，设备就可以使用了。接下来，[Gordon]详细介绍了使用 RFCat 重放幅移键控消息的细节。他使用 Arduino 和 [rc-switch](http://code.google.com/p/rc-switch/) 库来生成与插座兼容的信号。

为了与插座配合工作，必须嗅出信号。这是使用 [RTL-SDR](http://sdr.osmocom.org/trac/wiki/rtl-sdr) 和一个低成本电视调谐器加密狗完成的。通过输出嗅探到的信号并对其进行分析，可以确定调制。最后一步是编写一个 Python 脚本来使用 RFCat 重放消息。

黑客是软件定义无线电技术的良好组合，以成功的攻击结束。休息之后观看重放攻击的视频。

[https://www.youtube.com/embed/zpc0Eg7eMo4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zpc0Eg7eMo4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)