# Android Hack:用你的手机破解 WiFi 密码

> 原文：<https://hackaday.com/2012/09/18/android-hack-cracking-wifi-passwords-with-your-phone/>

您笔记本电脑中的 WiFi 适配器有一个特殊的模式——监控模式——可用于监听 WiFi 流量，只要有点耐心，就可以用来破解 WEP 密码。令人惊讶的是，这种监控模式在任何 Android 设备上都找不到，部分原因是硬件的限制。一个由三名研究人员组成的小组，[Ruby]、[Yuval]和[Omri]决定利用他们的假期[为他们的 Android 智能手机](http://bcmon.blogspot.com/)添加监控模式，从而实现一个更加便携的 WiFi pwnage 工具版本。

研究人员使用的手机 Nexus One 和 Galaxy S II——使用了不支持监控模式的 Broadcom 芯片组。为了绕过这一限制并允许操作系统看到完整的 802.11 帧，该团队需要对该 Broadcom 无线电芯片的固件进行逆向工程。

该团队发布了 Nexus One 和 Galaxy S II 中的 bcm4329 和 bcm4330 芯片组的固件更新。更新*可能*适用于其他具有相同芯片组的手机，但不要相信我们的话。

还有很多工作[Ruby]、[Yuval]和[Omri]需要去做。他们想在他们的固件中加入数据包注入，当然也想创建一个 APK 来更容易地实现这一点。

如果您有内核开发的经验，并且愿意提供帮助，请给团队发一封电子邮件。如果你想玩的话，可以在 google code 找到源代码[。](https://code.google.com/p/bcmon/)