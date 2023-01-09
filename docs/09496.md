# 在现代电脑上观看 Macintosh SE 的视频

> 原文：<https://hackaday.com/2015/07/09/viewing-a-macintosh-ses-video-on-a-modern-computer/>

有一台旧的麦金塔 SE 电脑。他正在寻找一种方法，在更新、更现代的计算机上查看 SE 的视频输出。他最终使用 STM 32 f 4 发现板设计出了一个非常聪明的解决方案。

首先，SE 的逻辑板从机箱中取出，放在桌子上，以便于拿取。然后，使用普通跳线将发现板连接到 SE 的处理器直接插槽(PDS)。“发现板”在较新的 Mac OSX 电脑上充当 USB COM 端口。发现板监视 SE 对视频存储器的写入。当它看到 R/W 引脚变为低电平时，它知道正在进行写操作。然后等待/AS 变为低电平，这表示总线上有地址。发现板读取该地址，并验证它是否在视频帧缓冲器的范围内。如果是，则发现板会将数据副本写入本地缓冲区。

OSX 电脑运行一个简单的应用程序，可以通过 USB 向发现板发出请求。当板接收到请求时，它通过 USB 连接将其本地帧缓冲数据发送回主机。然后，OSX 计算机使用 CGImage 在窗口中显示这些数据。下面的演示视频就是用这种技术拍摄的。

[https://www.youtube.com/embed/hhg5Lg_VTaQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/hhg5Lg_VTaQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢拉斯]