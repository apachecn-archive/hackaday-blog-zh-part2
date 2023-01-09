# 基于 ESP8266 的智能电表

> 原文：<https://hackaday.com/2014/11/02/an-esp8266-based-smartmeter/>

在过去的几周里，我们一直在谈论 ESP8266，这是一款基于 4 美元微控制器的 Wifi 模块。由于 Espressif 最近发布了 SDK，许多廉价的物联网应用成为可能。

[Thomas]用一个模块制作了一个简单的智能仪表,用来测量他的加热器的工作时间和外部温度。他添加了 2 个 AT 命令来启动/停止测井过程，并使用一个 GPIO 引脚来监控加热器的油泵状态。然后，测量结果会定期通过 TCP 连接发送到他的数据收集服务器，这样他就可以生成漂亮的图表。

在下面嵌入的视频中，您将看到[Thomas]演示他的系统。在他的 [hackaday.io 项目页面](http://hackaday.io/project/3249-esp8266-smartmeter)上，他对如何复制这个令人敬畏的项目做了非常详细的解释。他使用和创作的所有资源也可以在[项目的 GitHub 页面](https://github.com/ThomasBarth/esp8266-ssm)上下载。

[https://www.youtube.com/embed/QxLYddb-40E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QxLYddb-40E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)