# 样板房模拟房子，反之亦然

> 原文：<https://hackaday.com/2015/05/30/model-house-models-house-vice-versa/>

[Eric Tsai]正在掀起家庭自动化狂潮。不满足于通常的基于智能手机的图形用户界面，[Eric] [建造了一个纸板模型房子来模拟他的房子](http://www.instructables.com/id/Physical-Home-Automation-Interface/?ALLSTEPS)。打开车库门，样板房的车库门就开了。打开真正的前门，一个微小的伺服电机打开纸板前门。

样板房还配有一个电表，可以显示他当前的用电量，这对于判断电子设备是否出现了严重故障非常有用。你应该从头到尾看完这段视频(休息后发现的)，这里是他打开电动吹叶机的地方。尽管有一点大的滞后，这很酷！

但是系统并不止于此。既然他可以通过 WiFi 远程控制车库门和一些灯，那么下一个合乎逻辑的步骤就是添加几个按钮，这样[模型房子就可以控制真实的房子](https://www.youtube.com/watch?v=pdKfJtnpNzs)。

[我们已经在](http://hackaday.com/2015/02/12/ridiculously-complicated-home-automation-made-simple/)前搜查了【Eric】的家。他在他的房子周围设置了简单的基于 Arduino 的传感器包，通过 pub/sub 框架 [MQTT](http://mosquitto.org/man/mqtt-7.html) 将它们连接在一起，并添加了开源 [OpenHAB](http://www.openhab.org/) 软件接口。门传感器连接到一个[被黑掉的眨眼集线器](http://arahuman.blogspot.de/2014/11/how-to-root-your-wink-hub-step-by-step.html)。从他的狗是否在叫到他的衣服是否洗好了，[埃里克]的系统无所不知。

[https://www.youtube.com/embed/ctkZrf_t-X8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ctkZrf_t-X8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们不能等到纸板房子赶上所有[埃里克]的家庭自动化能力。一只带压电扬声器会叫的小纸板狗？是的，请吧。说真的，这是一个很酷的想法，我们认为[埃里克]只是触及了表面。

当然，他需要一些东西来监控纸板屋的状态。我们建议在纸板房子里放一个更小的纸板房子。您会将哪些功能集成到您自己的物理家庭自动化控制器中？