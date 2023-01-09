# Irrighino，一个基于 Arduino Yun 的浇水系统

> 原文：<https://hackaday.com/2015/08/10/irrighino-an-arduino-yun-based-watering-system/>

有许多不同的方法可以让你的植物按时浇水。[Luca Dentella]刚刚建造了一个新的灌溉系统。他使用现成的标准硬件来保持简单。Irrighino 是一个基于 Arduino Yun 的完整的浇水系统，具有用户友好的 AJAX 界面。这允许以类似于在 Outlook 中创建约会的方式安排日程。也可以手动控制各种水螺线管。代码是完全可定制和开源的，代码可从[卢卡的] [github](https://github.com/lucadentella/irrighino) 库获得。web 界面分为三个选项卡——用于手动控制的“运行时间”,用于配置计划的“设置”,以及用于查看系统日志的“事件”。

Arduino Yun 通过继电器保护罩激活电磁阀。开关面板有指示器状态 LED 和三个位置开关。这些允许手动关闭或打开输出，或在自动模式下通过 Yun 控制输出。[Luca]描述了当连接到 Arduino 的单个模拟输入时，如何读取开关的三种状态(开-关-开)。他还有另一个教程，描述[如何将 USB WiFi 适配器连接到云](http://www.lucadentella.it/en/2014/11/08/yun-adattatore-wifi-usb/)。这很方便，因为 Yun 安装在信号强度非常弱的外壳内。虽然 Yun 具有车载 WiFi，但无法将外部天线直接连接到测试 SMA 插座。

一个有趣的部分是[商用雨水传感器](http://www.lowes.com/pd_172955-74985-57069_0__?productId=1043275)。这是一个被海绵状材料包裹的开关。当这种材料吸收雨水时，它开始膨胀并触发开关。Arduino 将传感器视为简单的数字输入。

休息之后，请查看视频中他的系统的简短演示。

[https://www.youtube.com/embed/KOz55u_fhdU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KOz55u_fhdU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)