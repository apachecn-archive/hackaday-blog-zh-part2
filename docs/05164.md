# 穿上这款 7 模式 LED 跑步夹克，停止交通

> 原文：<https://hackaday.com/2014/01/27/stop-traffic-in-this-7-mode-led-running-jacket/>

米里雅厌倦了在夜间跑步时与骑自行车的人纠缠。对她来说，照亮自己是显而易见的，但她认为如果灯光能响应她的心率，那将非常酷。向我们透露消息的简短摘要是纽约电阻器的[，【米里雅】](http://www.nycresistor.com/2014/01/24/heart-rate-running-jacket/)[在她的博客上给出了血淋淋的细节](http://blog.grunick.com/pulse-jacket/)。发光二极管以七种不同的发光模式工作，其速度与她的心率成正比。

她开始围绕 Arduino 进行构建，但发现兼容的心率传感器大多是光学传感器，读数不准确。由于她已经在使用 Garmin GPS 手表和心率监测带，她决定侵入两人之间的对话。Garmin 为此使用了蚂蚁协议。虽然[米里雅]发现这些文档是一种有效的安眠药，但她也发现 SparkFun 有一个 ANT 收发器分线板。可惜已经停产了。

[米里雅]继续使用 SparkFun 板进行原型制作。她的最终版本使用 Teensy 2.0 和这个 ANT 收发器来代替命运多舛的 SparkFun 板。她找到了一个[增能器电源包](http://www.amazon.com/Energizer-XP1000-Universal-Rechargeable-Power/dp/B002K8OQWS)，直接插入 Teensy，可以为两个 [Adafruit 防风雨 LED 灯条](http://www.adafruit.com/products/306)供电大约一个小时。看看两边，休息后看看她的演示。

[https://www.youtube.com/embed/B-mrleAj3Xs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/B-mrleAj3Xs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)