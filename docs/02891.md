# 适用于 3D 打印机的 RPi 打印机服务器

> 原文：<https://hackaday.com/2013/03/03/rpi-printer-server-for-your-3d-printer/>

[![OctoPrint](img/a706218bbbd1c8e162017daf56f71302.png)](http://hackaday.com/?attachment_id=95474)

想要在不连接笔记本电脑的情况下运行 3D 打印机吗？想让你的黑客空间打印机网络无障碍？OctoPrint 的目标是为 Raspberry Pi 制作一个 3D 打印服务器。

开源 Python 项目允许您在 RPi 上上传和管理 GCODE 文件。然后，您可以选择要打印的文件，并在运行打印机之前获取基本统计数据。包括温度在内的信息可以通过 UI 报告回来，并且可以运行任意 GCODE 命令进行设置和测试。

其他一些漂亮的功能包括将视频流式传输到用户界面，以便可以远程观看打印作业。还支持创建延时视频。将 wifi 加密狗和网络摄像头添加到 RPi 后，它就变成了一台功能齐全的打印服务器。

该项目使用 Flask web 框架为 UI 提供服务，使用 Tornadio 和 Socket.io 与 UI 进行异步通信。您可以从项目的 Github 中提取代码并进行测试。

感谢[Camerin]发送此邮件。