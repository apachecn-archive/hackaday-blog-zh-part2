# 适合 Kerbal 的火箭控制器

> 原文：<https://hackaday.com/2015/03/12/rocket-controls-fit-for-a-kerbal/>

Kerbal 太空计划是一个太空模拟游戏。你为一个名为 Kerbals 的虚拟种族设计宇宙飞船，然后将这些勇敢的 Kerbals 送入太空。有时候他们回不了家。

如果用你的 WASD 键控制飞船对你来说还不够沉浸式的话，[marzubus]已经创造了一个功能齐全的 [KSP 控制台](http://forum.kerbalspaceprogram.com/threads/111724-Psimax-CS40-Telemetric-Joystick)。它有一个操纵杆，多个显示器，以及一系列按钮和开关，可以满足你所有的飞行控制需求。该控制台采用模块化方法构建，因此不同的控件可以根据需要进行交换。

在引擎盖下，三个 Arduinos 提供了游戏和控制之间的接口。一个 Arduino Mega 运行 [HoodLoader2](https://github.com/NicoHood/HoodLoader2) 通过 HID 提供游戏杆数据。第二个 Mega 使用 [KSPSerialIO](https://kerbalstuff.com/mod/385/KSP%20Serial%20IO) 通过标准 COM 端口接口与游戏通信。最后，一个 Due 与显示器接口，它提供关于你的宇宙飞船当前状态的信息。

所有的部件都装在一个现成的外壳里，有点阿波罗任务控制的感觉。现在[马尔祖布斯]需要的是一件上面有克巴尔徽章的白色背心。