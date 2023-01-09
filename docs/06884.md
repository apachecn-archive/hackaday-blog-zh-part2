# 斯图尔特平台滚珠轴承平衡器

> 原文：<https://hackaday.com/2014/08/22/stewart-platform-ball-bearing-balancer/>

为了他们在圣何塞州立大学的机械工程高级设计项目，[Tyler Kroymann]和[Robert Dee] [设计并建造了一个赛车运动模拟器](http://www.fullmotiondynamics.com/)。这稍微超出了大多数黑客的预算，所以在他们全面投入使用之前，一个更实惠的 Arduino powered Stewart 平台概念验证已经建立。Stewart 平台通常使用六个电动或液压线性致动器来提供六个自由度(6 DOF)、浪涌(X)、摇摆(Y)、起伏(Z)、俯仰、滚动和偏航的运动。通过简单的软件转换矩阵，考虑到伺服臂的角位移，您可以将所需的线性运动转换为标准业余伺服的 PWM 信号。

6 DOF 平台，加上电阻式触摸屏，也是他们机电控制系统类的一个辅助项目。然而，在这种配置下，平台只能俯仰和滚转。Arduino 读取电阻式触摸屏并记录滚珠轴承的位置。然后 PID 将其与目标位置进行比较，产生一个误差矢量。误差向量用于找到一个[逆运动学解](http://wikipedia.org/wiki/Inverse_kinematics)，该解使致动器将球移向目标位置。整个过程每秒钟重复 50 次。目标位置可以预先编程或使用 Wii 双截棍上的模拟棒来控制。

休息后观察滚珠寻找目标位置。

感谢[Toby]提供这条提示。

[https://www.youtube.com/embed/j4OmVLc_oDw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/j4OmVLc_oDw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们 Hackaday 期待着[大理石疯狂](http://wikipedia.org/wiki/Marble_Madness)在现实生活中的实现！

需要帮助[揭秘 PID 控制](http://hackaday.com/2011/07/21/demystifying-pid-control-with-a-look-at-the-new-arduino-pid-library)？或者，也许你想建立自己的[斯图尔特平台](http://hackaday.com/2013/09/18/stewart-platform-reinvents-the-wheel-so-you-dont-have-to/)？