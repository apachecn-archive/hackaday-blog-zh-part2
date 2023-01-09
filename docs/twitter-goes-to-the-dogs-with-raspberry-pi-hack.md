# Hackaday 奖参赛作品:Twitter 因树莓 Pi Hack 而被淘汰

> 原文：<https://hackaday.com/2015/08/21/twitter-goes-to-the-dogs-with-raspberry-pi-hack/>

狗是非凡的动物。任何和它们一起生活过的人都会知道它们是非常善于发声的动物，它们的叫声从注意到院子里有松鼠到警告性的呜呜声，说“如果你不带我出去，我就要在你的鞋子上撒尿了。”[亨利·康克林]决定将这些噪音的分析电脑化，把他的狗[奥利弗·特维奇]放在推特上，这样他就可以在工作的时候听到他在说什么。[亨利]那就是:[奥利弗]呆在家里。

他用一个树莓派来做这件事，它被设置成记录超过一定音量的声音。该系统位于[奥利弗]最喜欢的窗户旁，记录下了它的叫声。然后使用 [PyAudioAnalysis](https://github.com/tyiannak/pyAudioAnalysis) 对录音进行分析，这是一个分析声音的库，将它们与参考声音进行比较，并对它们进行分类。然后，Raspberry Pi 使用 [Python-twitter](https://github.com/bear/python-twitter) 将结果发布到 twitter 上。

![The setup used by [Oliver] to capture the barks: a USB microphone, Raspberry Pi and WiFi USB dongle.](img/db414770665c6fe85564894e187c984b.png)

【奥利佛】用来捕捉狗吠声的装置:一个 USB 麦克风、树莓派和 WiFi USB 加密狗。

或者更确切地说，当【亨利】修复了几个错误后，它会的:现在它只是发布一个随机的字符串，这个字符串是基于树皮的长度，而不是类型。[Henry]说他现在正在翻译狗。这仍然是一个很好的项目，它向您展示了使用少量代码从您的环境中收集信息并通过互联网共享这些信息是多么简单。[Henry]还说下一步是为[Oliver]创建每周播客。就我而言，我将订阅他的想法，听听邮递员有多讨厌，看到一只松鼠却无法追逐它们有多烦恼。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)