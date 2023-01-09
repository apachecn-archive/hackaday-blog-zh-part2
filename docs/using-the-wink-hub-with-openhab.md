# 结合 openlab 使用 wink hub

> 原文：<https://hackaday.com/2015/01/08/using-the-wink-hub-with-openhab/>

花足够的时间观察家庭自动化设置，你会很快发现有两种相互竞争的哲学。第一个想在每个电灯插座上安装一个 Arduino，通过廉价的易贝无线电模块连接一切。第二种家庭自动化理念需要极其昂贵的硬件来与其他昂贵的模块对话。Arduino 解决方案是一个可以无限定制的系统，商业解决方案出于某种奇怪的原因与“云”对话。没有中间地带。至少在[Eric]开始研究和查看一些硬件解决方案之前没有[。](https://electronichamsters.wordpress.com/2014/12/31/hacking-the-wink-hub-to-work-with-openhab-for-local-control/)

[Eric]希望通过他的手机、电脑或互联网控制一些 GE Link 灯泡。就价格和性能而言，它们应该是市场上最好的灯泡，但它们只能用 Zigbee 来控制。这导致[Eric]出现了一个有趣的黑客技术，让 Wink Hub 的所有所有者都可以本地控制他们的设备。根据[Eric]的研究，这是他的照明不依赖于“云”的唯一方式。

只有在[【埃里克】阅读了一篇关于传情动漫的帖子](http://arahuman.blogspot.com/2014/11/how-to-root-your-wink-hub-step-by-step.html)(以及[几天前的这篇帖子](http://hackaday.com/2015/01/05/a-better-way-to-hack-the-wink/))之后，传情动漫的本地控制才成为可能。因为该设备可以被植入，而且事实上[Eric]已经在他的房子里集成了一些与[OpenHAB](http://www.openhab.org/)集成的东西，选择如何继续控制一些支持 Zigbee 的灯是很容易的。

一旦[Eric]让灯泡与 Wink 对话，将它们与他家中的其他设备集成起来就很容易了。新灯泡由他的 [Arduino 运动传感器](http://www.instructables.com/id/Uber-Home-Automation/step7/Uber-Sensor-Security-Area-Presence-Sensor/)、[门传感器](http://www.instructables.com/id/Uber-Home-Automation/step5/Battery-Powered-Reed-Switch-Door-Window-Drawer-Mai/)激活，可以通过智能手机或语音控制来控制。传情动漫也可以完全断网。这是个好主意，因为开关灯的能力不应该由你的网络连接质量决定。

[https://www.youtube.com/embed/Fpv2vUXJpwY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Fpv2vUXJpwY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/ABWmiR2CySk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ABWmiR2CySk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)