# Leapcast 在你的浏览器中模拟 Chromecast

> 原文：<https://hackaday.com/2013/08/02/leapcast-emulates-chromecast-in-your-chrome-browser/>

我们的 Chrome 浏览器认为它是一个 Chromecast 加密狗。这是它播放 YouTube 视频的截图。请注意标题和屏幕控件，它们就像您在实际硬件上看到的一样。下载[dz0ny]编写的 Leapcast Python 包,亲自尝试一下。

在克隆 GitHub repo 之后，我们在编译这个包时遇到了一些问题。结果我们需要安装 python-dev，这就解决了问题。启动守护进程是一个简单的命令，我们指定了 Chrome 二进制路径，并添加了一些标志

```
leapcast --name HAD --chrome /usr/bin/google-chrome --fullscreen
```

一旦运行，Android YouTube 应用程序会自动检测 Leapcast 是否为 Chromecast 设备。它给了我们一个教程覆盖图，提到了界面上新的共享图标。在回放时按下那个图标会启动一个播放视频的匿名窗口。[dz0ny]链接到自述文件中的设备配置 JSON 文件。如果你检查一下，你会注意到网飞被列为“外部”，而其他人没有。这是因为 Chromecast 协议使用二进制来表示网飞。其他人用本地 websockets 或云代理来做，所以他们在这种设置下工作得很好。