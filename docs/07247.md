# 网络浏览器挑战 Arduino 的极限

> 原文：<https://hackaday.com/2014/10/05/web-browser-pushes-arduinos-limits/>

我们构建的一些项目满足了对一种新的硬件或软件的真正需求，这种新的硬件或软件将使生活变得更容易或解决一个常见的问题。另一方面，我们做其他项目只是因为有可能做。[Gilchrist]已经完成了一个完全属于第二类的项目:一个专门在带有以太网屏蔽的 Arduino Uno 上运行的网络浏览器。

Arduino 可以为连接的 LCD 提供纯文本网页，并可以跟随超链接。用户输入由一个小操纵杆处理，但令人印象深刻的部分是在软件方面。Arduino 只有 2KB 的 RAM 来处理网页，所需的库占用 20KB 的内存，只剩下大约 12 KB 用于 HTML 解析器/渲染器和 LCD 渲染器。

Arduino 浏览器是一项正在进行中的工作，并且[Gilchrist]提到该项目的目标包括更强的健壮性以处理糟糕的 HTML(尽管 [Hackaday retro edition](http://retro.hackaday.com/) 加载完美)、终端和 WiFi 功能。为此，也许一个好的解决方案是使用[新的 ESP8266 芯片](http://hackaday.com/2014/08/26/new-chip-alert-the-esp8266-wifi-module-its-5/)来保持小而便宜？