# Raspberry Pi 锅炉控制使用网络摄像头读取模拟仪表

> 原文：<https://hackaday.com/2014/05/09/raspberry-pi-boiler-control-uses-a-webcam-to-read-the-analog-gauge/>

![sub-image](img/a8ebe4a9cff399f515de22d1d08dd1af.png)

家庭自动化的最大问题之一是试图与旧的或模拟设备接口。你升级设备只是为了自动化吗？还是像[Seb]那样找到了一个[的变通办法？](http://hackingbeaver.com/?p=97)

[Seb]没有按需热水，因此如果他想洗个热水澡或淋浴，就必须打开他的锅炉。不太方便，早上必须提前一个小时醒来，只是为了打开锅炉，这样他就可以在早上洗澡了！面对不得不继续忍受这种情况的困惑，他决定尝试使用树莓派来实现家庭自动化。

问题是没有简单的方法来反馈锅炉正在做什么——当然他可以使用 Pi 的 GPIO 使用电源继电器来打开和关闭它，但是他如何轻松地测量锅炉内部的温度呢？

答案？网络摄像头！[Seb]拿了一个旧的廉价网络摄像头，把它安装在他的锅炉上的温度计前面。然后，他编写了一个简单的 python 脚本，使用 OpenCV 库来计算像素——当这些像素变成红色时，指针处于他的理想温度(45℃)。复杂？一点点，但是这个项目只花了他多少钱，35 美元？爱死树莓派有多便宜了！

[https://www.youtube.com/embed/7xG8IllBSoc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7xG8IllBSoc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)