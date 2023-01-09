# Arduino 驱动的数字万花筒

> 原文：<https://hackaday.com/2014/09/06/arduino-powered-digital-kaleidoscope/>

最新项目将一个古老的视觉效果玩具与数字电子技术结合起来。我们大多数人都熟悉廉价的[万花筒](http://en.wikipedia.org/wiki/Kaleidoscope "kaleidoscope")玩具。我们中的一些人甚至用纸管、镜子和珠子制作了它们的廉价版本。[Jose]想尝试使用 Arduino 和可寻址 LED 灯条重现万花筒创造的彩色图案效果。

构建实际上非常简单。底座是一个直径只有几英寸的聚氯乙烯圆盘。[Jose]从包含 60 个 LED 的可寻址 LED 条开始。然后他把它切成 12 段，每段包含 5 个发光二极管。然后将较小的条带安装到圆盘上，类似于自行车车轮上的辐条。LED 灯带已经有一个粘性的背衬，所以这部分是微不足道的。

最后一步是添加某种类型的扩散屏幕。LED 灯带本身并不那么有趣。漫射器允许光线混合在一起，形成有趣的图案，这些图案更容易让人想起您可能在真正的万花筒中看到的图案。没有漫射器，你只能看到单个的光点，而不是混合的颜色图案。

整个事情由一个小 Arduino 控制。[Jose]在他的博客文章的底部提供了代码。请务必观看下面的系统运行视频。

[https://www.youtube.com/embed/wxn9jKqD9k4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wxn9jKqD9k4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)