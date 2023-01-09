# 用 Python 编写 FUSE 文件系统

> 原文：<https://hackaday.com/2013/11/06/writing-a-fuse-filesystem-in-python/>

[![photo](img/cf49e08fd51d4cf78d89a1cae6428034.png)](http://hackaday.com/wp-content/uploads/2013/11/photo.jpg)

你有没有想过，如果你能直接控制文件访问，某个项目会更好？[Stavros Korokithakis]做的，特别是他正在做的一个备份程序。随之而来的是认识到[编写一个 FUSE 文件系统](http://www.stavros.io/posts/python-fuse-filesystem/)，特别是用 Python 编写，并不像看起来那么复杂。真的，通过开源的力量，繁重的工作已经为我们完成了。如果你想自己尝试，你需要[安装 fusepy](https://github.com/terencehonles/fusepy) 。从那时起，您只需要定义将要使用的文件系统方法。

Python 不会在文件系统领域赢得任何速度竞赛，但这并不是重点。使用这项技术为新的数据访问方式带来了巨大的机遇。如果你让自己的思想自由驰骋，你可以设想加密文件系统、无缝远程数据访问、新的键值存储设计等等。也许更有趣的是使用 Python 与物理设备通信的想法…也许是一个 proc 文件系统来跟踪你的机器人遥测技术？我们希望在评论中听到你的想法。

我们在 Linux 和 OSX 上成功地使用了[Stavros 的]示例脚本。(公平的警告，如果你在 Mac 上，fusepy 的 pip 版本似乎是针对 [fuse4x](http://fuse4x.github.io/) 而不是 OSXFUSE 的，但一旦你安装了先决条件，你就万事大吉了。)我们没有 Windows 机器可以测试。有人能证实那里是否也有同样的可能吗？