# 使用 MSP430 构建媒体播放器

> 原文：<https://hackaday.com/2012/04/02/building-a-media-player-with-an-msp430/>

![](img/6cc716c55609a02e10aef1779b27ea5e.png "MSP")

基于 Arduino 和 SD 卡的媒体播放器已经被重复使用了好几次，但这并不意味着我们不能欣赏[【Matt】的 MSP430 音频播放器](http://www.43oh.com/forum/viewtopic.php?f=9&t=2519)。这是一个非常好的工作，支持 FAT16 文件系统，只占用 54 字节的内存。

为了实现他的 430 媒体播放器的梦想，[Matt]将他的工作建立在[DIY Life Talking MSP 430](http://www.diylife.com/2008/04/25/make-a-talking-msp430-microcontroller)项目上。与之前使用 430 和 SD 卡播放音乐的尝试不同，[Matt]加入了完整的 FAT16 文件系统，允许他将计算机上的音频文件拖放到 SD 卡上。

现在[Matt]的版本可以通过扬声器播放立体声音频文件，但单声道文件的音质会大大降低。最大采样率为 16kHz 如果你戴着糟糕的耳机听音乐，这是一个“足够好”的采样率。在广告之后的视频中，[Matt]在他自制的媒体播放器上播放了[这首美妙的科学交响曲](http://www.youtube.com/watch?v=BZ5sWfhkpE0)。我们猜测他的相机没有完成他的项目正义，但它仍然令人印象深刻。

[https://www.youtube.com/embed/g_SGHgO7Hus?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/g_SGHgO7Hus?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)