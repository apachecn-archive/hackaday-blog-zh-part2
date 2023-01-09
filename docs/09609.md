# 咖啡好了，闹钟会通知办公室

> 原文：<https://hackaday.com/2015/07/24/alarm-notifies-the-office-when-the-coffee-is-ready/>

[Stian]认为如果他的同事可以在最新一批咖啡准备好时得到电子通知，那会很好。他最终建造了一个便宜的咖啡警报系统来做这件事。当咖啡煮好了，冲泡者可以按下一个巨大的按钮来通知办公室的其他人该喝茶了。

[Stian 的]第一个项目要求是使用一个大的物理按钮激活系统。他从 Sparkfun 选择了一个按钮，尽管他最终修改了它以更好地满足他的需求。最初的按钮带有一个内置的 LED。这对[Stian]来说还不够，所以他又增加了两个 led。所有三个 led 均由 ULN2003A NPN 晶体管阵列驱动。现在，他可以将它们依次闪现，制作一个简单的动画。

该瞬时按钮使用软锁电源开关向 [ESP8266](http://hackaday.com/2015/03/18/how-to-directly-program-an-inexpensive-esp8266-wifi-module/) 微控制器供电。当按下瞬时开关时，它向锁闩供电。然后，闩锁给主电路供电，即使松开按钮也继续供电。这种功率欺骗的原因是为了保存来自 18650 li-on 电池的功率。

警报的核心功能使用物理硬件和两种基于云的服务的组合。选择 ESP8266 是因为它包括一个内置的 WiFi 芯片，而且它只需要 5 美元。微控制器被配置为通过按下按钮来连接到 WiFi 网络。该设备还监控着巨大的报警按钮。

当按钮被按下时，它向运行在云服务 Heroku 上的自定义 clojure 应用程序发送 HTTP 请求。clojure 应用程序然后将酿造信息存储在数据库中，并向 Slack 云服务发送通知。Slack 是一种项目管理应用程序，允许多个用户在项目上工作，并通过互联网更容易地交流。[Stian]已经利用它来向他的同事发送实际的文本通知，让他们知道咖啡已经准备好了。请务必观看下面的演示视频。

[https://www.youtube.com/embed/U0oF-PBfZIg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/U0oF-PBfZIg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)