# 狗追踪者知道泥土在哪里

> 原文：<https://hackaday.com/2014/11/08/dog-tracker-knows-where-the-dirt-is/>

[Eric]正在用他的[狗跟踪系统](http://www.instructables.com/id/Uber-Home-Automation/step15/Dog-Tracker/)让养宠物这个不太愉快的杂务变得简单一点。狗追踪器实际上是更大的 [OpenHAB 系统](http://hackaday.io/project/1720-20-wireless-arduino-home-automation-w-openhab)的一小部分，我们[早在 7 月](http://hackaday.com/2014/07/19/long-range-wireless-sensors-for-the-home-area-network/)就展示了这个系统。

作为一个狗主人，[埃里克]讨厌在院子里寻找他的宠物的粪便。他一直在计划一个系统来使这变得更容易，而当地的黑客空间活动正好提供了一个机会来充实他的想法。狗追踪器的主要传感器是全球定位系统。大多数狗在做自己的事情时会一动不动几秒钟。[Eric 的]基于 Arduino-frg 的系统利用这一事实，结合倾斜传感器来确定家庭宠物是否留下了任何礼物。

跟踪器使用 HopeRF RFM69 收发器将此信息转发给家庭基站。RFM69 只有大约 900 英尺的范围，因此拥有较大资产的人可能会希望购买基于蜂窝网络的跟踪系统。一旦粪便被追踪，OpenHAB 就有了一个接口

[Eric]在他的设计中也包括了逃跑的狗。如果 Fido 通过地理围栏，OpenHAB 将发出警报。自带 RFM69 的手持狗追踪器可以用来追踪逃跑的狗。未来的计划是将狗追踪器小型化，这样狗穿起来会更舒服。

[https://www.youtube.com/embed/4ro3_JDt2K0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4ro3_JDt2K0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)