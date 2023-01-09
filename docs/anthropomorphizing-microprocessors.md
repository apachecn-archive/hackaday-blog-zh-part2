# 拟人化微处理器

> 原文：<https://hackaday.com/2014/11/26/anthropomorphizing-microprocessors/>

老式微处理器通常会做一些事情，无论是坐在一个空闲的循环中，计算一些东西，还是只是在收藏家的橱柜中看起来很酷。[Lee]为旧的微处理器想出了一个更酷的用法:[他把它拟人化了](http://www.sunrise-ev.com/projects.htm#facecard)，把发光二极管连接到地址线上，并把这些发光二极管排列成一张脸。接通正确的电路后，发光二极管的表面会慢慢改变表情，使这个小小的电路板对随机的电子波动做出反应。

这个项目使用的 CPU 是 RCA 1802，最出名的是 COSMAC Elf 中的 smarts，这是一台非常早期的微处理器培训计算机，但今天仍然能够教授计算的基础知识，尽管处理器不再使用任何现代技术都几乎不支持的指令集。

[李]显然有很多这样的 1802，为了展示微型计算机可以变得多么简单，他为 CPU 创造了我们所见过的最奇怪的用途。你不能对发光二极管的这一面进行编程；数据总线悬空，因此随机值“显示”在表面上。只有一条数据线被拉高。这可以防止数据总线成为 0x00，即 HALT 指令。

如果你想用 RCA 1802 MPU 做点更有用的事情，[Lee]还有一张 COSMAC Elf 会员卡。这是著名的 COSMAC Elf 的复制品，[重新包装成一个 Altoid 锡](http://www.sunrise-ev.com/membershipcard.htm)大小的板。它有 1802 板载，几个开关和闪光灯，以及一个用于与外设交互的并行端口。