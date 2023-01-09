# 警察激光雷达拆除

> 原文：<https://hackaday.com/2015/07/20/police-lidar-tear-down/>

在消费者开始购买雷达探测器后，大多数警察部门都从雷达转向了激光雷达。很多这样的激光雷达设备现在都在过剩的市场上。如果你没有 500 美元左右来买一把激光雷达枪，只是为了看看它是如何工作的，你很幸运。[阿列克谢·波尔卡诺夫]花了一个小时[拆卸一辆超轻型 LTI 20-20 LR 100](https://www.youtube.com/watch?v=enjxwCsNp6g) 所以你不必。

一个小时对于一个拆除的视频来说似乎太多了，但[阿列克谢]加快了无聊部分的速度，花了很多时间谈论光学和设备如何工作(有很多手绘的图表)。他还把它组装起来，并连接一个示波器来显示设备的电子操作。

他提到显示和控制板使用串行接口与控制板通信。主板上还有一个未填充的接头，这显然是一个串行端口，可能是为了对板载微控制器进行重新编程。通过一点逆向工程工作，这种激光雷达枪应该是高度可破解的。

除了显示和控制板之外，该装置还包含激光器和光电二极管的高压电源。制造一个足够干净的电源来驱动激光器，不会干扰传感器，这是设计驱动因素之一。与系统中的其它板相比，电源是一个大而复杂的板。

[https://www.youtube.com/embed/enjxwCsNp6g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/enjxwCsNp6g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

在之前，我们已经介绍过用于机器人的[激光雷达，但是相比之下，超轻单位是非常重要的工业强度单位。如果你想更多地了解专业激光雷达设备的工作原理，或者你只想知道下次你因超速被拦下时该对什么技术感到愤怒，请观看[亚历克西的]视频。](http://hackaday.com/2014/01/23/lidar-with-leds-for-under-100/)