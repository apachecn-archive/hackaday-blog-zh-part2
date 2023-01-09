# 一种简单廉价的 GPS 导航装置

> 原文：<https://hackaday.com/2015/04/29/a-simple-and-inexpensive-gps-navigation-device/>

现在市场上有很多 GPS 导航装置，但是自己动手做点东西总是很有趣的。这就是[middelbeek]用他 25 美元的 GPS 设备所做的。他设法在网上找到了一些不错的电子元件交易，包括 Arduino Uno、GPS 模块和 TFT 显示屏。

为了在设备上获取地图图像，[middelbeek]必须通过手动过程。首先，他必须下载他想要绘制地图的区域的 GEOTIFF。GEOTIFF 是一种元数据标准，允许将地理配准信息嵌入到 TIFF 图像文件中。[middle beek]然后必须将 GEOTIFF 转换成 8 位 BMP 图像文件。BMP 图像与描述每个 BMP 边界的. dat 文件一起存储在 SD 卡上。的。dat 文件也是手动创建的。

Arduino 加载这些数据，并在 320×240 TFT 显示屏上显示正确的地图。[middle beek]在他的 [github 页面](https://github.com/middelbh/GPSnavigator "github")上解释说，他目前无法同时显示来自两个地图文件的数据，这可能会在位置移动到地图边缘时导致问题。我们怀疑，通过更多的工作和调整，这个系统可以得到改善，更容易使用，当然，25 美元以下，你不能期望太多。