# 眨三下眼睛让我进去

> 原文：<https://hackaday.com/2015/04/08/blink-thrice-to-let-me-in/>

现在这里有一个非常酷的家庭黑客。[Luis Rodrigues]已经自动打开了他的车库门，只需对着它闪一下前灯。

但是等等，那不是意味着任何人都可以闯入他的房子吗？没有。起初，我们以为他只是添加了一些光电传感器和一点计算机逻辑，以便将灯光图案转化为打开车库的输出，但事实上，这只是针对他的汽车的。这很棒，因为如果有人试图模仿他闯入，他们闯入的是一种非常混乱的精神状态。

你可以看到它实际上是如何工作的，前灯输出连接到他汽车引擎盖下的控制盒。A [Moteino](http://hackaday.com/2014/09/12/thp-hacker-bio-felix-rusu/) (RF Arduino 变体)读取闪烁三次的大灯的输入信号，然后与车库门进行无线通信，以便打开车库门。

但是[路易斯]在他的房子外面也有一个门——所以如果你让灯亮一秒钟，车库的门和外面的门也会打开。

[https://www.youtube.com/embed/3GPqGToYURY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/3GPqGToYURY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

非常棒——请注意，车库门按钮真的那么难用吗？如果有人偷了你的车，并且碰巧有你的地址，这绝对是安全的！