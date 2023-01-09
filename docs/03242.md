# Weather-O-Matic 在模拟界面上显示数字天气

> 原文：<https://hackaday.com/2013/05/07/weather-o-matic-displays-digital-weather-on-an-analog-face/>

![SANYO DIGITAL CAMERA](img/af0c71ea6198bda4230bc8e4a0f2d1a2.png)

这个外观简洁的读数器[使用模拟刻度盘显示天气](http://nunobmartins.com/?p=47)。[Nuno Martins]称之为天气自动控制，在跳跃之后，他解释了项目的内容。

硬件非常简单。每只手上都有一个伺服电机。MSP430 通过与计算机的串行连接获取天气信息(数据由 Python 脚本抓取),并相应地设置表盘。微控制器还以框架侧面的单个按钮的形式接收用户输入。表盘左侧的文字是葡萄牙语，分别表示今天、明天和后天(意为后天)。多次按下该按钮将滚动浏览这三个单词，然后显示当天的最高和最低预测温度。

这件事的好处是，如果你切断电源，伺服电机将留在原地。我们打赌，如果他想让这成为他家的永久设备，他可以通过使用微控制器的睡眠功能并添加射频收发器与服务器通信，让它在电池上运行良好。

[https://www.youtube.com/embed/w2r1genlnOA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/w2r1genlnOA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)