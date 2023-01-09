# 本周失败:用于调节发光二极管的色度计

> 原文：<https://hackaday.com/2014/01/16/fail-of-the-week-color-meter-for-adjusting-leds/>

![fotw-color-meter](img/5b72c9eec91de5536ec07edd99bb38dd.png)

[John Peterson]回应了我们的号召，通过讨论他在构建这个色度计时学到的东西来记录您的黑客行为。他认为这个项目是一种精确匹配由 PWM 信号驱动的 led 颜色输出的方法。想法是它可以采样一个 LED 的输出，然后使用该数据来计算必要的值，以匹配其他 LED 的颜色。当使用不同类型的 led 时，这是一个好主意，但即使是来自同一条生产线的二极管也可能显示出颜色输出的差异。

当然，如果这个项目像他预期的那样成功，它就不会成为本周的败笔。原来他使用的传感器，SparkFun 分线板上的 Avago ADJD-S371-QR999，可以快速读取颜色。这对固体物体来说很好，但对像 PWM LEDs 这样开关的光源来说就不太好了。

我们喜欢[John]在项目上发布了[一系列经验教训。真正的失败是试图使用这种特殊的传感器，但我们认为一定有某种方法可以通过采样获得有意义的数据。查看](http://www.saccade.com/writing/projects/ColorMeter/LessonLearned.html)[退役传感器](https://www.sparkfun.com/products/retired/8618)的页面，其中也包括数据表的链接。你能想出一个允许硬件采样的固件破解方法吗？这样 PWM 值就可以通过求平均值或其他计算方法推断出来。请在评论中告诉我们。

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**