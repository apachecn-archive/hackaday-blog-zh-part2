# 通过安装 BusyBox，无需 Root 即可在 Android 上使用常见的 Linux 工具

> 原文：<https://hackaday.com/2012/12/05/common-linux-tools-on-android-without-root-by-installing-busybox/>

[Adam Outler]向我们展示了如何扩展 Android 上可用的 Linux 工具，而不影响设备。他通过安装 BusyBox 来做到这一点。使用 Android 开发者桥将二进制文件复制到设备上。然后，他打开一个 ADB shell，向二进制文件添加执行权限，并运行它。BusyBox 称自己为[嵌入式 Linux 的瑞士军刀](http://www.busybox.net/about.html)。它提供了一套非常常用的工具，您会发现这些工具在您的修补工作中非常有用。[Adam]在他的视频中展示的是 vi 编辑器，但是让 shell 工作的基础都在那里，比如:ls、mkdir、grep、dmesg、mount…你明白了。

那么，既然您已经掌握了这些命令，那么您将如何处理您的非根设备呢？那真的要由你自己去想了。[Adam]继续他的演示，安装了一个需要 root 访问权限的包。是 [BotBrew Basil](https://play.google.com/store/apps/details?id=com.botbrew.basil&hl=en) ，增加了 apt-get 和几个更复杂的包。然后，他使用 vi 编写一个 C++ Hello World 程序，然后编译并运行它。因此，如果你想在手机上做一些开发，这是一种方法。

[http://www.youtube.com/watch?v=L_bVC0x4l-g](http://www.youtube.com/watch?v=L_bVC0x4l-g)