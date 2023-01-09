# 移动黑客空间状态指示器

> 原文：<https://hackaday.com/2014/02/18/mobile-hackerspace-status-indicator/>

![HACKERSPACE LIGHT](img/b02674c08662945e6c35d2975c5b98a0.png)

在镇上闲逛，不知道该做什么——哦，嘿，看，有人在黑客空间！介绍[移动空间状态指示器！](https://ackspace.nl/wiki/Mobile_Spacestate_Indicator)

在我们的[欧洲黑客空间之旅](http://hackaday.com/2013/11/06/hackerspacing-in-europe-conclusion/)中，我们有幸参观了位于荷兰赫尔伦的[ack space](http://hackaday.com/2013/10/23/hackerspacing-in-europe-ackspace-in-heerlen/)。像许多黑客空间一样，他们有一个在线状态指示器，让会员和非会员都知道空间是否开放。[Vicarious]是一位好心从火车站接我们的绅士，他刚刚完成了对他的汽车的一次令人敬畏的改装。使用 Arduino Uno 和 Raspberry Pi，他创建了一个移动指示器来显示他的黑客空间的状态。

Raspberry Pi 会自动绑定到他的手机上，并在线检查黑客空间的状态。然后，它将数据发送到 Arduino Uno，Arduino Uno 控制一小片 RGB LEDs。他巧妙地将所有这些藏在他的中控台里，看起来棒极了！

要查看更多 ACKspace 的酷项目，请查看他们的 wiki！