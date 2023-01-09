# 原型 X 四轴飞行器无线电的逆向工程

> 原文：<https://hackaday.com/2014/12/10/reverse-engineering-the-proto-x-quadcopter-radio/>

就在几年前，手掌大小的无线电遥控玩具还只是一个梦想。今天，你可以在每一个商场、玩具店和玩具店找到它们。无法抗拒小小的 Estes Proto X 四轴飞行器。虽然他很喜欢驾驶 Proto X，但他发现这个小小的控制器还有很多不足之处。这对阿尔瓦罗来说不成问题，因为他开始着手一个项目，对这个小飞行器进行逆向工程。

在四轴飞行器和它的小人国无线电中，[Alvaro]发现了一个基于 STM8 的处理器和一个 amicom a 7105 2.4G FSK/GFSK 收发器无线电。A7105 是有据可查的，数据手册很容易从互联网上获得。处理器和无线电芯片之间的接口是开始逆向工程工作的最佳场所。

在他的 Saleae 逻辑分析仪的帮助下，[Alvaro]能够在四轴飞行器和发射器协商连接时从两者捕获 SPI 数据。产生的十六进制文件不是很有用，所以[Alvaro]写了几个 Python 脚本来解码数据。通过在抓捕过程中操作每一个控制器，[阿尔瓦罗]能够对 Proto X 的控制协议进行逆向工程。他测试了这一点，从远程控制单元移除微控制器，并将 A7105 连接到 STM32F4 开发板。通过 USB 将 STM32 连接到他的电脑上，[Alvaro]能够命令四轴飞行器起飞。这不是一次非常优雅的飞行，但它确实证明了他移植的控制系统是有效的。有了基本的控制之后，[阿尔瓦罗]在他的电脑上完成了一个快速的用户界面。他现在可以用键盘和鼠标驾驶四轴飞行器了。这不仅证明了控制系统的工作原理，也显示了用 FPS 控制驾驶一架真正的飞机(即使是一架很小的模型)有多困难。

Estes Proto X 实际上是由 Hubsan 制造的，Hubsan 是一家以 x4 系列迷你四轴飞行器而闻名的中国制造商。由于 Proto X 和 x4 共享相同的通信协议，[Alvaro 的]工作可以应用于两者。完全由计算机控制的无人机售价不到 30 美元，我们只需要几个摄像头(和大量的编码)就能与宾夕法尼亚大学 GRASP 实验室的无人机群合作。

[https://www.youtube.com/embed/BfARBlWldN0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BfARBlWldN0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/5Op-pvrtTcU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5Op-pvrtTcU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)