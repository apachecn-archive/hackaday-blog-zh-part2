# 美味的 Dash Pi 驾驶数据

> 原文：<https://hackaday.com/2014/11/01/delicious-dash-pi-driving-data/>

几周前，[send ex]描述了 Python 如何改变了他的生活。特别是，它让他能够自动挖掘比特币，教其他人编程，并使用一个树莓 Pi 实现了一台不到 100 美元的[全车载计算机。](http://www.reddit.com/r/raspberry_pi/comments/2k4pm4/raspberry_pi_computer_in_the_car_w_screen/)

它基于一辆 B 型车，他把它装在一个结实的 Pi [相机盒](http://www.mcmelectronics.com/product/83-15553?scode=GS401&catargetid=530004080000291113&cadevice=c&gclid=CjwKEAjwzqKiBRCAydTZzOLi9CISJACm3irWrTMlZg_q5JbiEvbNEw_R9HYnpyRqXuB0B4ZHYQouYhoCZL_w_wcB)里，相机盒放在他的本田 S2000 的仪表板上。屏幕是一个 17 美元的互联网特殊与复合，这使得 BOM 的方式下降。一个 [3A 开关](http://www.mausberrycircuits.com/collections/car-power-supply-switches/products/3a-car-supply-switch)接入点火装置，确保 Pi 的电源不会被粗暴中断。

当[sentdex]启动汽车时，一个脚本将 Pi 直接带入桌面模式。他该项目的主要目标是安装一个仪表板摄像头，并与 OBD 电脑进行通信。Pi 提取包括油门位置在内的各种数据点，用户可以使用滚动键盘上的箭头键在列表中移动。

将来，他想升级它来实时记录油门位置，并增加一个传感器来显示刹车位置。休息之后，请务必观看走查/演示视频。

[https://www.youtube.com/embed/V_fSoViiNOo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/V_fSoViiNOo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)