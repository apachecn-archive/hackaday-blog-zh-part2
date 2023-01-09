# 再次解锁 Rigol 范围

> 原文：<https://hackaday.com/2013/07/02/unlocking-a-rigol-scope-once-again/>

Rigol scopes 正在走向世界各地制造商的工作台上。这是有原因的——它们很容易升级。通过简单的软件更新，您可以将 50 MHz 的 Rigol o'scope 变成 100 MHz 带宽的型号。一个型号的设计决策有时会被带到不同的产品线，所以最终有人会想出如何[将 70 MHz DS2072 示波器变成 200 MHz DS2202](http://freneticrapport.blogspot.com/2013/07/raspberry-pi-rigol-ds2072-200mhz.html) 。一个很棒的 mod，可以把一个 800 美元的示波器变成一个 1600 美元的示波器。

没有必要对这个模型进行内部修改；它的工作原理很简单，通过 USB 向示波器发送一些工程解锁代码，这是一个简单的任务，[Blair]用 Raspberry Pi 和一点 Python 代码实现了这个任务。黑客的唯一错误是每次关机时都会重置示波器。事实上，这可以用任何带有 Python 解释器的微控制器来完成。

下面是一个相当简单的演示视频，或者你可以查看 EEVBlog 线程，这里是这个 mod 的构思。

我们在 Hackaday 期待一个小型、廉价的 USB/微控制器加密狗，它可以自动更新 DS2072，随时出现在我们的收件箱中。我们感谢所有寄来的人。

[https://www.youtube.com/embed/DnOGmsP-iVQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DnOGmsP-iVQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)