# 三星 NX300 扎根

> 原文：<https://hackaday.com/2014/05/14/samsung-nx300-gets-rooted/>

![sammy](img/5704a1c128014f77f39cdcfe3439c676.png)

[Ge0rg]给自己买了一台新的三星 NX300 无反光镜相机。我们中的许多人只会拍一些漂亮的照片，但[Ge0rg]不会，他[想看看是什么让他的相机滴答作响](http://op-co.de/blog/posts/hacking_the_nx300/)。他没有拿出螺丝刀，而是开始测试相机的安全功能。

NX300 作为具有 NFC 和 WiFi 连接的“智能相机”出售。NFC 连接原来只是嵌入相机某处的一个[恩智浦 NTAG203 标签](http://www.nxp.com/products/identification_and_security/smart_label_and_tag_ics/ntag/series/NTAG203.html)。这类似于我们[在洛杉矶的聚会上分发的](http://hackaday.com/2014/01/23/the-gathering-huge-success/)NFC 标签。该标签旨在在配置良好的智能手机上启动 android 应用程序。标签可以写锁，但是三星没有设置锁位。这意味着你可以重新编程并永久锁定标签，作为你最喜欢的[网站](http://hackaday.io/)的链接。

[Ge0rg]接下来是主要事件，NX300 的 WiFi 接口。端口扫描显示摄像机正在运行一个未受保护的 X 服务器和 [Enlightenment](https://www.enlightenment.org/) 。让那件事过去一会儿。open X 服务器意味着攻击者可以欺骗击键，推送图像，并将应用程序指向相机屏幕。

在第二篇博文中，【Ge0rg】解决了在相机上获得 root 访问权限的问题。根据他已经发现的信息，[Ge0rg]知道相机运行的是 Linux。访问三星的[开源软件中心](http://opensource.samsung.com/reception.do)下载 NX300 的开源部分证实了这一点。经过一番挖掘和一些转移注意力的事情后，[Ge0rg]找到了他要找的东西。相机在启动时总是试图从 SD 卡的根文件夹运行 autoexec.sh。[Ge0rg]给了摄像机它正在寻找的脚本，并用命令填充它来运行 [BusyBox 的](http://en.wikipedia.org/wiki/BusyBox) telnet 守护进程。这就是他所需要的——root shell 访问权限是他的。

[图片通过[维基媒体共享](http://commons.wikimedia.org/wiki/File:NX300_White_front.jpg) /Danrok]