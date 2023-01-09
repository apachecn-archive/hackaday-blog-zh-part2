# 鼠标中的恶意软件

> 原文：<https://hackaday.com/2014/03/30/malware-in-a-mouse/>

硬件和软件形式的键盘记录器已经存在了很久很久。更狡猾的键盘记录者足够聪明，可以将命令“输入”计算机，并安装特洛伊木马、后门和其他真正令人讨厌的东西。但是，老鼠呢？毫无疑问，不起眼的 USB 鼠标不可能成为一些疯狂的安全恶作剧的攻击途径，对吗？

事实证明，是的，除了一个 USB 鼠标，什么都没有的情况下闯入一台电脑是可能的。卓越的德国计算机杂志 CT Magazine 的人[制作了木马鼠标](http://www.heise.de/ct/heft/2014-8-Computermaeuse-laden-Schaedlinge-aus-dem-Netz-nach-2156334.html)(德语，[可怕的谷歌翻译](http://www.google.com/translate?hl=en&ie=UTF8&sl=de&tl=en&u=http%3A%2F%2Fwww.heise.de%2Fct%2Fheft%2F2014-8-Computermaeuse-laden-Schaedlinge-aus-dem-Netz-nach-2156334.html)

鼠标接收到的唯一输入是按钮按压、滚轮滴答声和嵌在底座上的一个又小又破的摄像头的图像。构建用 Arduino 读取这个相机，当某个灰色和更灰色的像素模式出现时，它会触发一个从互联网下载文件的命令。从安全的角度来看，鲍勃是你的叔叔。

通过相机观察老鼠的内部并不是什么新鲜事；在互联网上完成的变成了[史上最差的扫描仪](http://spritesmods.com/?art=mouseeye)。尽管如此，能够处理这些图像数据并利用它们做一些事情还是很酷的。只是不要接受陌生人送的鼠标垫。

Danke [Ianmcmill]给小费。