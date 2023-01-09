# 熵降低了你的 Android 设备的速度吗？

> 原文：<https://hackaday.com/2013/01/04/is-entropy-slowing-down-your-android-device/>

![071210_1705_AndroidDev11.jpg](img/989e714abbe77a69b4f722cf6b44aada.png)

[Lambgx02]厌倦了他的 Android 设备停滞不前，决定深挖问题的原因。他的研究让他相信熵导致了减速。他认为他的解决方法减少了普通 Android 设备上 90%的延迟。

那么熵是如何导致这个问题的呢？当一个应用程序从运行在设备最底层的 Linux 内核请求一个随机数时，似乎存在一个瓶颈。Android 设置为对所有随机数请求使用/dev/random，但是[Lambgx02]说那个位置有非常浅的可用数字池。当它们用完时，内核必须重新加载新的种子，这阻止了请求数据的应用程序继续运行。 [](http://forum.xda-developers.com/showthread.php?t=1987032&nocache=1)

他的解决方案是编写自己的应用程序，使用/dev/urandom 中的一个数字每秒钟播种/dev/random 一次。他提到，这可能会导致安全漏洞，因为以这种方式播种随机数据并不那么随机。也可能有电池寿命的问题，所以如果你尝试一下，一定要监控性能。

[via [Reddit](http://www.reddit.com/r/Android/comments/15w1qi/fix_90_of_lags_in_android_needs_root/)