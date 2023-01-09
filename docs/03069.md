# 名片上画有[ch00f]的标志

> 原文：<https://hackaday.com/2013/03/27/business-card-draws-ch00fs-logo/>

[ch00f]又来了，[拓展了 PCB 名片艺术的视野](http://ch00ftech.com/2013/03/25/making-a-cooler-business-card/)。这个人通过 USB 接口在任何电脑上画他的商标。

卡片的物理设计很大程度上受到[【弗兰克·赵】的卡片](http://hackaday.com/2010/10/29/tiny-usb-business-card/)的启发；两者都使用 ATtiny85 和 V-USB 封装来处理 USB 协议和通信。[ch00f]的卡不像[Frank]那样在文本编辑器中键入文字，而是在 MS Paint 或其他图像编辑器中绘制 ch00ftech 徽标。

不过，简单地模仿鼠标在屏幕上画一个标志有一个问题；因为不同的计算机有不同的鼠标加速设置，ch00ftech 的标志几乎总是失真的。[ch00f]通过模拟绝对输入设备，基本上将他的名片变成了单一功能的手写板，从而解决了这个问题。

徽标是手工绘制的，并放入固件中的几个数组中。令人惊讶的是，这个标志并没有占用太多空间——tiny 85 的闪光灯只有 4k。对于更复杂的绘图来说有更多的空间，但现在简单的 ch00ftech 标志(休息后的视频)就可以了。

[https://www.youtube.com/embed/lF31aDuSZ6E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/lF31aDuSZ6E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)