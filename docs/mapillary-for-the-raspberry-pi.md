# 树莓的梅子

> 原文：<https://hackaday.com/2015/04/24/mapillary-for-the-raspberry-pi/>

如果你住在偏远地区，谷歌地图车无法到达，你可能会注意到互联网上没有太多你所在地区的照片。mapi pile 希望通过众包的全球照片来改变这种情况，通过手机应用程序拍摄照片并上传到网上。[sabas1080] [将这一功能带到了最受欢迎的 ARM 开发板](http://www.instructables.com/id/Mapillary-en-Raspberry-Pi/?ALLSTEPS)、Raspberry Pi 上。

Raspberry Pi 不是手机，也不是通常上传照片到 mapi pile 的方式。没有全球定位系统，所以地理标记是不可能的。Pi 没有相机或屏幕，如果你要拍摄偏远地区的照片，电池将是一个好主意。

不过，所有这些作品都可以在 Pi 上看到；[sabas1080]从 Adafruit 采购显示器，摄像头是标准的 Raspi 事务，GPS 是众多中国零售商之一的 GY-NEO6MV2 模块。再加个大的动力银行电池，硬件都有了。

软件是这个构建变得棘手的地方。mapi pile[有一套用 Python 编写的很好的免费工具](https://github.com/mapillary/mapillary_tools)，但这只是构建的一部分。[sabas1080]需要连接摄像机，设置显示器，并弄清楚如何使用 mapi pile 工具让一切正常工作。最终，[sabas]能够让整个设置作为一个可编程的移动照相亭工作。