# 在三维空间中映射 WiFi 信号

> 原文：<https://hackaday.com/2015/02/17/mapping-wifi-signals-in-3-dimensions/>

[Charles]正在寻求利用流行的低成本 ESP8266 WiFi 模块完成更多令人瞠目结舌的黑客攻击。本周的项目是[在 3D 空间](http://hackaday.io/project/4329-wifi-power-mapping)绘制 WiFi 接收信号强度。虽然 ESP8266 能够提供接收信号强度指示(RSSI)，[Charles]没有直接使用它。他在笔记本电脑上编写了一个简单的 C 程序，以 500Hz 左右的频率 ping ESP8266。然后，笔记本电脑会将 ping 应答中的 RSSI 转换为颜色值，然后发送到 ESP8266。由于 ESP8266 运行的是[Charles']定制固件(正如他在 [WiFi 杯项目](http://hackaday.com/2014/11/11/test-your-signal-with-the-wifi-cup/)中看到的)，它可以直接在 WS2812 RGB LED 上显示颜色。

起初，这些颜色似乎是随机的，但[查尔斯]注意到有一种模式。他只是需要一种方法来观察 LED 随时间的变化。单帧长时间曝光可以，但视频也可以。[查尔斯]走视频路线，创造了[超长曝光](https://github.com/cnlohr/superlongexposure)，这是一个基于 FFMPEG 的工具，它提取每一个视频帧并将它们合成为一个帧。他看到的非常酷——有明确的好信号和坏信号的条纹。

有了这些信息，[Charles]孤注一掷，将他的 ESP8266 安装在一台大型龙门式磨机上。他拍摄了几个 360x360x180mm 毫米区域的长曝光视频。视频被提取成层。然后，整个数据集可以用 Voxeltastic、[Charles']自己的基于 HTML5/WEBGL 的渲染引擎进行可视化。结果是惊人的。信号强度在对应于 WiFi 信号的 12.4 厘米波长的节点和反节点中增强和减弱。最终的渲染看起来难以置信的有机，这并不完全令人惊讶。我们已经在商用天线模拟表征系统中看到过同样的图像。

[查尔斯]又一次让我们大吃一惊，我们迫不及待地想看看他接下来会做什么！

[https://www.youtube.com/embed/aqqEYz38ens?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aqqEYz38ens?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)