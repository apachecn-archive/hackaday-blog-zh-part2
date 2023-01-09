# 物联网变色龙灯用 Python 做

> 原文：<https://hackaday.com/2015/03/16/iot-chameleon-lamp-does-it-with-python/>

如果物联网这个东西要离开发射台，它将需要实用和半实用的项目想法的帮助，使日常用品智能化。让这些项目起步的一部分是克服人类和硬件之间的语言障碍，人类希望轻松地将复杂的想法原型化，而硬件需要具体的指令。一家名为 Things on Internet [TOI]的公司创建了一个名为 VIPER 的系统，通过在板上创建一个虚拟机，可以轻松地用 Python 编写任何 Spark Core、UDOO 或 Arduino。

该套件包括一个屏蔽、一个 IDE 和应用程序。通过[修改一个简单的鹅颈宜家灯](http://www.instructables.com/id/Smartify-FRYEBO-the-Ikea-Lamp/),【TOI】演示了[蝰蛇](http://viper.thingsoninternet.biz/)(蝰蛇是实时嵌入的 Python)。他们打开灯，添加了一个 24 LED Adafruit neo pixel 戒指，可以通过智能手机使用 VIPER 应用程序远程控制。为了展示蝰蛇盾的电容感应能力，他们在灯的头部衬上了箔片。这个[代码示例](http://www.instructables.com/files/orig/FF8/H2F2/I6RSELP8/FF8H2F2I6RSELP8.py)会在应用程序中每次按下按钮时将新像素变为随机颜色。

休息后，观看灯演示，并停留在遥控汽车上。

[https://www.youtube.com/embed/Y_8kytJ8fgs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Y_8kytJ8fgs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/RSNw9ZjTB0E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/RSNw9ZjTB0E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)