# 长达一年的延时照相机

> 原文：<https://hackaday.com/2014/12/22/a-year-long-time-lapse-camera/>

所有[val3tra]想要的是一个射频可访问的相机。这种相机可以拍照，将照片保存到 SD 卡上，偶尔还会通过射频链路将照片发送到电脑上。这个项目已经失去控制，现在它已经成为一个开源相机，能够拍摄长达一年的延时电影。

该产品最初是一台低功耗相机，使用的是易贝 JPEG 相机，为 3.3V。它只有 640×480，但每帧平均只有 48kb——小到足以在 FAT16 格式的 SD 卡上存储几千张照片。一个 4 美元的射频模块，一个 ATMega 和一个 RTC 组成了该建筑的其余部分，其功耗约为每小时 100 焦耳。一个 D 电池大约有 60，000 焦耳，悲观地估计，一个四节串联电池，两节并联电池的运行时间为 200 天。

这种构造后来得到了改进，将总电池消耗降低到每帧约 3.5-4 焦耳，或每 10 分钟一帧，约每小时 24 焦耳。这令人印象深刻，让这台相机运行超过十几个月带来了一些有趣的挑战。必须考虑电池的自放电，环境问题也很重要，尤其是让相机在莫斯科的冬天运行，见下面的视频。

如果你不想精简设备，你可以把你的 [DSLR、Pi 和一些重要的电池](http://hackaday.com/2013/07/30/self-contained-time-lapse-rig-braves-elements-from-thirty-feet/)密封在一个防风雨的外壳里。

[https://www.youtube.com/embed/aYzQma_5TN0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aYzQma_5TN0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)