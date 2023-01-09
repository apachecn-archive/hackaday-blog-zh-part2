# 使用路由器作为无线嵌入式平台

> 原文：<https://hackaday.com/2012/06/10/using-a-router-as-a-wireless-embedded-platform/>

![](img/acf680cbcac6045031dbda8a9f88586b.png "router")

如果你打算让你的下一个项目无线化，你不需要 XBee，WiFi shield，甚至蓝牙模块。将旧硬件转换成开发板[非常容易](http://taiksonprojects.blogspot.com.es/2012/06/i2c-bitbanging-con-openwrt-en-fonera.html)，正如【Taikson】通过给 Fonera 路由器添加 I2C 总线向我们展示的那样。(西班牙语，这里是[谷歌翻译](http://translate.google.com/translate?sl=es&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Ftaiksonprojects.blogspot.com.es%2F2012%2F06%2Fi2c-bitbanging-con-openwrt-en-fonera.html&act=url))

为了添加一条 I2C 总线，[Taikson]将原本用于路由器状态引脚的两个引脚焊接在一对导线上。[Taikson]的路由器运行的是 OpenWrt，所以添加对 I2C 设备的支持只是改变一些内核设置的问题。

至于你能用路由器开发平台做什么，没有限制。去年，[泰克森]通过一个网页浏览器控制了一架四轴飞行器[,该浏览器带有一个经过类似修改的 I2C 路由器。这是一个聪明的黑客技术，只需要一点点工作，就可以给他的四轴飞行器添加一些传感器甚至一个摄像头。](http://hackaday.com/2011/08/01/fonera-based-quadcopter-can-be-controlled-from-a-web-browser/)