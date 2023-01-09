# 问 Hackaday:无电池蓝牙物品定位标签能存在吗？

> 原文：<https://hackaday.com/2014/05/21/ask-hackaday-can-battery-free-bluetooth-item-locating-tags-exist/>

[Vishak]向我们透露了关于[I find Kickstarter 活动](https://www.kickstarter.com/projects/yuansong84/ifind-the-worlds-first-battery-free-item-locating)的消息，这是一个 1.25×1.06×0.09 英寸(32×27×2.4 毫米)的标签，可以贴在你日常生活中可能会丢失的任何东西上。该设备与支持蓝牙低能耗(BLE)的智能手机通信，具有 200 英尺(60 米)的检测范围和响亮的警报。有趣的是，这个装置不需要任何电池来操作

> 回收电磁能量并将其储存在一个独特的电源库中。

正如你所猜测的，这个特别的声明引起了 Hackaday 团队的兴趣，因为我们从来没有展示过这么小的能量收集设备。我们想到的“最接近”的东西是 [Allsee 项目](http://hackaday.com/2014/04/15/extracting-gesture-information-from-existing-wireless-signals/)，这是一个简单的手势识别设备，它使用现有的无线信号(电视和 RFID 传输)来提取发生在它面前的任何运动。然而，天线相当大，提取的功率很小。

[快速谷歌搜索](https://www.google.ch/search?q=ble+power+consumption)让我们知道蓝牙低能耗解决方案通常消耗大约 10uA @ ~3V 的空闲电流。(非常)成功的 [Sticknfind 活动](https://www.indiegogo.com/projects/sticknfind-bluetooth-powered-ultra-small-location-stickers/x/470367)推广了相同的电池供电产品，声称使用 CR2016 电池和 100 英尺范围可自主运行一年，导致约 90mAh/24/30.5/12 = 10.2uA 的空闲电流。由于我们不是这方面的专家，我们想问问我们的读者，他们是否在正常的家庭环境中遇到过这样的能量收集性能(3V*10.2uA = 30uW)。我们非常糟糕的数学表明，如果一个人想从距离你 2 米远的典型 Wifi 路由器中提取功率，发射 0.5 瓦特的功率(在完美的真空环境中)，带有 32 * 27 毫米= 864 毫米= 0.000864 米的标签，你只能得到 0.5 *(0.000864/(4 * pi * 2 * 2))=8.6 uw。

因此，我们不能在演示视频中看到 iFind 内部的内容，也不能看到更多有关正在申请专利的技术的细节，这太糟糕了。我们希望我们亲爱的读者能在下面的评论部分给我们启发。