# 家庭自动化设置让您随时了解信息

> 原文：<https://hackaday.com/2014/12/01/home-automation-setup-keeps-you-informed/>

[johannes]写信告诉我们他的最新项目，一个他命名为*bot man*T3 的[家庭自动化装置。虽然他称之为家庭自动化系统，但控制灯光和家用电器(它通过 433MHz 无线传输)只是其功能的一小部分。*机器人*的前面板包括一个伺服系统，它指向当前天气的激光蚀刻图标。它还有一个显示屏，可以显示室内和室外的天气状况，以及[johannes]家周围的公共交通状况。](http://zeitwesendiylog.spreitzer.at/?p=133)

Botman 是围绕一个带有以太网屏蔽的 Arduino 构建的。Arduino 的内存非常少，所以[johannes]使用 Google Apps 引擎作为他的 Arduino 和他的数据源的 JSON APIs 之间的缓冲。这大大减少了 Arduino 必须保存在内存中并解析的数据量。

[johannes]还写了一个与 *Botman* 通信的 Android 应用。该应用程序有控制他家灯光的按钮，并复制前面板上显示的所有信息。[johannes]还在 *Botman* 中内置了一些日志功能。温度读数和其他信息从 Arduino 上传到 Google Docs 电子表格，他可以在任何地方查看和绘制这些数据。休息后看看视频，看看*机器人*的动作。

[https://www.youtube.com/embed/TsERkRO1cn0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TsERkRO1cn0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)