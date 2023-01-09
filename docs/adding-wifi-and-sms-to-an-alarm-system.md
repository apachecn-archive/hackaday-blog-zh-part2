# 向警报系统添加 WiFi 和 SMS

> 原文：<https://hackaday.com/2015/01/16/adding-wifi-and-sms-to-an-alarm-system/>

[Don]想把他的警报系统带入现代。他认为让它更有联系会成功。具体来说，他想让他的警报系统在警报触发时给他发送一条短信。

[Don]首先必须想出一种方法，当警报响起时触发一个事件。他发现了一个通向警报器的螺丝终端。当警报触发时，该螺丝端子输出 12V 电压以启动警报器。这是监控警报跳闸的好地方。

[Don]正在用 Arduino nano 监控警报信号。这意味着需要降低 12V 信号。他让它通过一个电阻和一个齐纳二极管来降低电压到 Arduino 可以处理的程度。一旦 Arduino 检测到信号，它就会使用 ESP8266 WiFi 模块发送电子邮件。[Don]使用的地址是 email-to-SMS 地址，这导致一条文本消息通过手机网络到达他的手机。

Arduino 也需要动力。[Don]在警报系统电路板上发现了一个螺丝端子，它提供稳定的 12V 输出。他让另一个电力调节板把电压降到稳定的 5V。这正好提供了 Arduino 运行所需的电量，而且它不依赖电池。[Don]在下面的视频中很好地解释了该系统。

[https://www.youtube.com/embed/TchYLpPWnbE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TchYLpPWnbE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/ERHM496qbQA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ERHM496qbQA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)