# 带树莓派的 WiFi 控制电源插座

> 原文：<https://hackaday.com/2015/02/11/wifi-controlled-power-outlets-with-raspberry-pi/>

[Tim]正在寻找一种使用 WiFi 控制电源插座的方法。他考虑购买一辆 WeMo，但他意识到他可以用更多的钱制造出更好的东西。他首先购买了五包 Etekcity 无线遥控插座开关。这些有点像 [WeMo](http://hackaday.com/2013/02/23/wemo-without-a-smartphone/ "WeMo") ，只是它们不是通过 WiFi 控制的。相反，它们配有一个射频控制器。[Tim]只是需要找到一种方法来弥合射频遥控器和 WiFi 之间的差距。

[Tim]决定用树莓皮作为控制器的大脑。他还购买了一个 SMAKN [433MHz RF](http://hackaday.com/2014/08/14/thp-entry-a-433mhz-packet-cloner/ "Packet cloner") 接收器和发射器，用于与无线插座开关通信。模块的布线非常简单。只有四根电线。每个模块都有电源线和接地线。那么发送器需要两个 GPIO 引脚，而接收器只需要一个。

[Tim]从一个新的 Raspbian 装置开始。然后，他安装了接线 Pi，这使您能够以类似于 Arduino 的方式与 GPIO 引脚接口。他还安装了 Apache 和 PHP 来创建一个用于切换插座的 web 界面。最后一步是编写一些定制软件。该软件包括一个脚本，允许[蒂姆]嗅出他的射频遥控器的控制。将正确的代码输入到“toggle.php”文件中，一切都设置好了。[Tim]现在所要做的就是浏览到他的 Pi 的 web 服务器并点击一个按钮。所有的定制代码都可以通过 git 获得。