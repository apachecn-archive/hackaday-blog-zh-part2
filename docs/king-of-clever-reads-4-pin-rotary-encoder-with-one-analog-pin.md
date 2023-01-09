# 用一个模拟引脚读取 4 引脚旋转编码器

> 原文：<https://hackaday.com/2015/06/15/king-of-clever-reads-4-pin-rotary-encoder-with-one-analog-pin/>

旋转编码器是非常有趣的技术。它们是精确测量旋转(包括方向)的可靠方法。[David]最近编写了一些软件来处理这些输入设备，但与其他人不同的是，[他的应用程序只能在一个微控制器引脚](https://analog10.com/posts/rotary_encoder_analog_input.html)上运行。

大多数人会使用三个引脚来处理带微控制器的旋转编码器:一个引脚处理开关，两个引脚处理正交输入。在他的项目中只剩下一个销可用的情况下，[David]不得不寻找另一个解决方案，他专注于编码器销在转动轴时以非常特定的方式表现的原理。他设计了一种电路，可以根据这些引脚的状态产生模拟电压。他还编写了一个程序，可以识别他的旋转编码器和新电路产生的新模拟模式。

如果你在一个使用旋转编码器的项目中被卡住了，因为你已经没有针了，这种新颖的方法可以帮助你摆脱卡住。这是一个令人印象深刻的电路设计壮举。想想[有多少其他项目](http://hackaday.com/2015/05/08/relays-calculate-square-roots/)使用这些类型的输入设备并从中受益！

【via [Hackaday.io 项目页面](https://hackaday.io/project/6311-analog-input-hack-push-button-encoder)去给它来个脑壳！]