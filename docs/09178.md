# 物联网让托马斯拥有了坦克引擎

> 原文：<https://hackaday.com/2015/06/02/iot-enabled-thomas-the-tank-engine/>

这个月，广受欢迎的“坦克发动机托马斯”玩具庆祝了它的 70 周年纪念。作为一个有趣的项目，[tinkermax]希望将这个[传统玩具带入物联网](http://tinker.yeoman.com.au/train/)时代，同时保留其物理外观和简单的魅力。

他使用了一种被称为“柴油”的模型，这种模型似乎足够大，可以容纳电子设备，但一旦他检查了内部结构，就证明情况并非如此。他需要安装一个 ESP8266 模块、一个加速度计突破、一些分立器件、一个漂亮的模拟多路复用器和一个 14500 3.7V LiPo。一旦完成，他就能够通过 WiFi 远程控制它的速度，当加速度计感应到火车正在上坡时，它会自动“加速”，并远程监控电池状态、发动机负载、倾斜度和轨道振动——所有这些都是通过 WiFi 使用 MQTT 实时进行的。这很好地展示了这些超级便宜的 WiFi 模块的力量，这些模块正在推动当前的物联网创新浪潮。

火车马达依靠一个 1.5V 的电池工作，所以[tinkermax]尝试了几个升压转换器来让 ESP-12 工作。但是模块有点大，不能提供 ESP-12 所需的高峰值电流。所以他用了一块 14500 的 3.7V LiPo 电池代替。串联二极管将 LiPo 电压降至电路友好的 2.9V ~ 3.6V 范围。ADXL345 加速度计用于测量“俯仰”以检测上坡和下坡，测量“滚动”以检查倾斜或翻倒，测量振动以识别轨道缺陷。它使用他编写的特殊 Lite-SPI 库与 ESP-12 进行通信。

进行两次模拟测量。一种方法是使用一个与 PWM 驱动电机串联的电阻来测量其电流，同时使用一个低通滤波器来消除 PWM 噪声。另一个是电阻分压网络，用于监控电池电压。但是 ESP-12 只有一个 ADC 通道。没有增加另一个 ADC 模块，【tinkermax】使用了一个简洁的设备 [FSA3157](https://www.fairchildsemi.com/datasheets/NC/NC7SB3157.pdf) ，它允许[将两个模拟输入引导到一个输出](http://tinker.yeoman.com.au/2015/05/26/when-you-need-multiple-analog-inputs-for-your-esp8266-application/)，就像 SPDT 开关一样。一个 PWM 输出用于控制电机速度，另一个用于驱动 LED。

传感器数据通过 MQTT 协议以每秒 5 次的速度传输到基于 Raspberry Pi 的 MQTT 代理。最后， [JavaScript 网页接收 MQTT 消息，并以图形方式绘制数据](http://tinker.yeoman.com.au/2015/05/11/simple-browser-based-graphical-display-of-mqtt-data/)。他想实现的一个升级是速度测量，以允许恒速驱动。如果您对如何从加速度计中提取信息有任何想法，请在下面发表您的评论。在下面的短视频中查看他的构建日志。如果你想看看所有这些如何在现实世界中使用，请查看另一个视频，其中[tinkermax]的同事介绍了一个连接到 Thomas the Tank Engine 的商业企业[物联网云平台](https://www.youtube.com/watch?v=vXQV1EvmG0Q)。

[https://www.youtube.com/embed/-o6LYynn95E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-o6LYynn95E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)