# 一台非常聪明的热成像相机

> 原文：<https://hackaday.com/2013/01/03/an-absurdly-clever-thermal-imaging-camera/>

热成像相机是一种能够在拍照的同时测量物体温度的相机，价格非常昂贵。对于一辆新车的价格，你可以拿起这些红外摄像机之一，并检查出草案在你的房子里。[Max Justicz]认为他甚至可以做得比专业级热成像相机更好，并发明了[一种聪明得离谱的 DIY 红外相机](http://www.maxjusticz.com/light-painting-with-temperature/)。

虽然热成像相机—[即使是便宜的自制相机(](http://hackaday.com/2012/12/15/a-thermal-imaging-camera-for-your-phone/))也有一个红外传感器，其工作原理很像相机的 CCD，但有一种更便宜的替代品。非接触式红外温度计售价 20 美元，唯一的缺点是它们只能测量一个点，而不能像更贵的同类产品那样测量多个区域。[Max]的想法是使用这些温度计中的一个和一些 RGB LEDs 在场景周围绘制不同颜色的光，以响应由[红外温度计传感器](https://www.sparkfun.com/products/9570)检测到的温度。

为了把他的想法变成一个可用的工具，[Max]拿起一个 LED 手电筒，把现有的 LED 阵列留到下一天使用。在用一些 RGB LEDs 填充手电筒的内部后，他添加了红外温度计传感器和 Arduino，以根据传感器给出的温度改变 LED 的颜色。

之后就是简单的光绘问题了。[Max]拿了一台相机，让快门开着，用他的 RGB 温度计手电筒画了一个场景，用多色 led 代表红外温度计感应的温度。这是一个非常聪明的方法，实现如此简单，以至于我们惊讶于我们以前没有见过。