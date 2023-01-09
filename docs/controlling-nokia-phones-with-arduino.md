# 用 Arduino 控制诺基亚手机

> 原文：<https://hackaday.com/2015/01/01/controlling-nokia-phones-with-arduino/>

当[伊利亚·吉查斯基尔]在等待他的 SIM900 盾到来时，他决定看看他能用一台旧的[诺基亚 6310i 和一台 Arduino](https://ilias.giechaskiel.com/posts/arduino_sms/index.html) 做些什么。他正在研究如何为一个家庭安全项目发送自动短信，发现可以通过摩托罗拉手机的耳机插孔发送 [AT 命令。但不幸的是，诺基亚不支持这一点，因为他们使用一种被称为](http://murchlabs.com/send-sms-from-your-arduino/) [FBus](https://en.wikipedia.org/wiki/FBus) 的协议。在几乎没有信息的情况下，[伊利亚斯]能够破解复杂的协议，并控制他的 Arduino。

连接就绪后，[伊利亚斯]能够使用一个名为 [Gnokii](http://gnokii.org/) 的程序与诺基亚手机进行通信，这是一个专门为用电脑控制手机而编写的实用程序。使用 Arduino 作为中介，他最终能够接入 FBus 并发送 SMS 消息。

请务必查看他的博客，因为[Ilias]详细介绍了诺基亚的 FBus 协议是如何工作的，并提供了复制他的黑客技术所需的所有源代码。最后还有一个视频演示，展示了黑客的行动。