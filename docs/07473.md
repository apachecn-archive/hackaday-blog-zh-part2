# 将覆盆子变成 CAD 工作站

> 原文：<https://hackaday.com/2014/11/02/turning-the-raspberry-into-a-cad-workstation/>

Inventables 一直在努力开发非常受欢迎的 Shapeoko 数控铣床的继任者，为了将数字制造带给大众，他们创造了 [Easel](http://www.easel.com/) ，这可能是你用过的最简单的 3D 设计软件。[Sacha]正在试用测试版的画架，并向 dev 邮件列表提到他正在树莓 Pi 上运行他的装置。一名开发人员插话说，经过一段时间的反复[，我们现在有了一个将画架与树莓派](http://thesimpleswitch.blogspot.com/2014/10/shapeokoarduinoraspberry-pieasel.html)一起使用的工作流程。

Easel 是一个网络应用程序，但由于图形、设计和 g 代码生成都是在本地处理的，即使是最基本的 CAD 套件也会让明显低功耗的 Raspi 窒息。相反，[Sacha]正在使用 Raspberry 获取 2D 和 3D 文件，将其转化为机器的 g 代码，并将其发送到 Shapeoko 路由器。

Easel 还没有在 Linux 上工作的本地发送器支持，所以使用一个单独的软件通过串口将 g 代码发送到机器上。这可能会在 Easel 的后续版本中添加，使树莓 Pi 成为控制路由器或铣床的一种很好的方式。