# 在 YouTube 上解码新闻直升机信号

> 原文：<https://hackaday.com/2014/02/02/decoding-news-helicopter-signals-on-youtube/>

一个偶然的 YouTube 视频推荐让[Oona]看到了一个新闻直升机追车视频的原始拷贝。看视频时，她注意到左边的扬声器发出奇怪的声音。这就是让乌娜开始狩猎的全部原因。解码神秘信号对她来说有点困扰。我们最后一次看到【Oona】[解码公交车站显示屏的无线电信号。](http://hackaday.com/2013/11/25/sniffing-data-from-radio-controlled-bus-stop-displays/)她分离出左声道音频，并通过 [baudline](http://www.baudline.com/) 软件发送，这帮助她确定这是一个[二进制频移键控(BFSK)](http://en.wikipedia.org/wiki/Frequency-shift_keying) 信号。用 SoX[再做一点工作，她就有了 1200 波特的比特流。](http://sox.sourceforge.net/)

在十六进制编辑器中打开解码文件显示了数据。每个包是 47 字节。大多数数据包是静态的。然而，这三组字节不断变化。[Oona]将这些数字解码为纬度和经度，并将结果数据绘制在谷歌地球上。将她的数据与视频中汽车的位置进行比对，发现了一个匹配。[Oona]有一个完整的跟踪新闻直升机，因为它跟着汽车。遥测数据是 7 位 [Bell 202](http://en.wikipedia.org/wiki/Bell_202_modem) ASCII 码，很可能是直升机新闻工作人员和演播室制片人使用的[可中断折返(IFB)](http://en.wikipedia.org/wiki/Interruptible_foldback) 系统的一部分。点击过去的休息，为 YouTube 视频开始这一切。

[https://www.youtube.com/embed/TCKRe4jJ0Qk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TCKRe4jJ0Qk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

【[新闻直升机图片来源](http://commons.wikimedia.org/wiki/File:BBC_News_helicopter_watching_over_the_cuts_protest.jpg)