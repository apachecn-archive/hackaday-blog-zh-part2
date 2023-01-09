# 当您的服务器融化时，LED 会告诉您

> 原文：<https://hackaday.com/2013/02/11/led-tells-you-when-your-server-has-melted/>

![LED](img/8e11fa5a82fe2c5bf06ad537ec0817c3.png)

为 Hackaday 写作的好处之一是能够随意命令大批读者登陆毫无防备的网络服务器。大多数时候，一台服务器可以处理数千个连接的负载。不过，在极少数情况下，服务器会变成一堆渣滓和废物，这让我们 Hackaday 感到满意，却让世界各地的管理员感到愤怒。

不过，检查您的服务器是否还在运行并不是非常有趣。[Eric]认为对他的服务器有多忙进行适当的物理可视化会很酷，并最终使用一个闪烁的(1) USB 可控 LED [来显示他当前的服务器负载](http://www.ericerfanian.com/server-status-and-website-traffic-monitoring-with-blink1-and-the-google-analytics-api/)。

[闪光灯(1)](http://thingm.com/products/blink-1.html) 是一种小型 USB 控制的 RGB LED，可用作通用指示灯。[Eric]想到将它插入他的一台服务器，并根据服务器的负载改变 LED 的亮度。他用一个 Python 脚本完成了这项工作，该脚本查询 Google Analytics API 并返回一个 0 到 255 之间的值，以响应他的服务器在过去 10 分钟内的受欢迎程度。

当然，黑客日总是有机会黑掉他的服务器。在这种情况下，闪光灯会发出稳定的红光，提醒[埃里克]他受欢迎了。