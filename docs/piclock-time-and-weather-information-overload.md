# piclock 时间和天气信息霸主

> 原文：<https://hackaday.com/2015/06/10/piclock-time-and-weather-information-overload/>

[Kevin]想要一个可以快速浏览并获得他一天中使用的所有当前环境信息的显示器。这些信息当然包括时间和日期以及天气信息。我们不只是在谈论当前的天气信息，而是对未来一周的预测，以及显示当前天气模式的地图。为了做到这一点，[凯文]想出了一个独特的系统，他称之为 [PiClock](https://hackaday.io/project/6184-piclock-a-raspberry-pi-clock-weather-display) 。

[Kevin]做了一些严肃的程序来启动这个时钟项目。天气数据来自 Weather Underground API，地图数据来自 Google Maps API。主程序用 Python 编写，可以在任何运行 Python 2.7+和 PyQt4 的 OS 上运行。如果你有兴趣做类似的事情，可以查看 github 上的[源代码。](https://github.com/n0bel/PiClock/blob/master/Documentation/Overview.md)

从项目的名字来看，树莓派是这里的大脑就不足为奇了。USB WiFi 适配器允许访问互联网，但以太网连接也可以。让 raspi 到处挂着电线会有点懒，所以[Kevin]打开他的 19 英寸液晶显示器，将 raspi 安装在机箱内。他从显示器的电源中取出 5v 直流电压，用来给 RaspPi 供电，不需要外部电源！如果 PiClock 的背景不够酷，一些 RGB LED 灯条被安装在显示器的背面，以产生[环境光](http://en.wikipedia.org/wiki/Ambilight)效果。