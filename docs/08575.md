# 用压电传感器测量心率

> 原文：<https://hackaday.com/2015/03/19/measuring-heart-rate-with-a-piezo/>

四处寻找可以轻松与微控制器接口的心率传感器，你会发现一些项目使用 led 和其他微控制器来完成过滤光线中脉冲的肮脏工作。

[托马斯]正在做一个项目，用几个压电传感器检测水是否流经管道。出于好奇，他将传感器贴在手指上，令所有人惊讶的是，他的微控制器发出的值[是他的心率](http://www.ohnitsch.net/2015/03/18/measuring-heart-rate-with-a-piezoelectric-vibration-sensor/)的一个极其无噪声的版本。

问题中的压电[是标准的现成模块](http://www.dfrobot.com/index.php?route=product/product&product_id=399)，将其添加到微控制器就像将压电放在模拟引脚上一样简单。从那里，它只是平均测量值，并从数据中提取心跳。

这是一个简单得多的测量心率的解决方案，因为有两个人没有听说过这项技术，很可能更多的人也没有听说过这项技术。如果你正在寻找进入[hack aday 奖](http://hackaday.io/prize)的机会，这将是一个很好的起点，无论是在健身还是医疗领域。