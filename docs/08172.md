# 带键盘装备的激光绊线

> 原文：<https://hackaday.com/2015/01/28/laser-trip-wire-with-keypad-arming/>

我们大多数人都有过这样的兄弟姐妹，他们会溜进我们的房间去偷晶体管，弹你的吉他，或者随便乱动你的东西。现在有一种方法可以在兄弟姐妹越界时立即得到提醒。[罗尼]制造了一个[激光绊线](http://www.instructables.com/id/Arduino-Laser-Trip-Wire/?ALLSTEPS)，配有一个液晶显示屏和键盘，用于装备和解除系统。

这个项目的大脑是一个 Arduino。有一个键盘用于输入密码，还有一个液晶显示屏用于显示输入的密码是否正确。[Ronnie]使用 keypad.h、liquidcrystal.h 和 password.h 库编写了自己的程序。一个小型激光指示器照射在光敏电阻上，光敏电阻反过来向 Arduino 输出模拟信号。当激光束中断时，输出电压下降，Arduino 会发现电压下降，然后打开报警蜂鸣器。触发警报的值设置在正常日光产生的值和激光束击中 LDR 时产生的值的中间。[Ronnie]将他的代码和接线图提供给任何对制作自己的激光绊网感兴趣的人。

希望，[罗尼的]讨厌的小弟弟没有看他的 YouTube 视频(休息后再看)来找出秘密通行码。对于没有键盘的激光绊线，看看这个[便携式的](http://hackaday.com/2011/09/11/laser-trip-wire-in-an-easy-to-use-form-factor/)。

[https://www.youtube.com/embed/efA9lwmE5zA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/efA9lwmE5zA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)