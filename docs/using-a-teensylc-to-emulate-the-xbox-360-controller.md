# 使用 TeensyLC 模拟 XBOX 360 控制器

> 原文：<https://hackaday.com/2015/07/14/using-a-teensylc-to-emulate-the-xbox-360-controller/>

在《真人快打 X》发布后，Zachery 的游戏团队想扩展到格斗类游戏。他们很快意识到，为了最大化他们的体验，他们需要一个比标准游戏手柄更好的控制器。键盘也不能切断它。他们想要一根格斗棍。这些大型控制器看起来非常像街机格斗控制器，包括操纵杆和大按钮。[Zachery 的]小组决定[制造他们自己的格斗棍](http://www.zlittell.com/2015/07/fightstick/)用于个人电脑。

[Zachery]以 TeensyLC 为基础进行构建，这是一个带有 ARM 处理器的 32 位开发板。它也兼容 Arduino。他的项目的最初版本将控制器设置为 HID，本质上是模拟键盘。这在一段时间内有效，直到他们遇到了一些游戏的兼容性问题。[Zachery]了解到他的控制器与 DirectInput 兼容，但 direct input 已被弃用。新的东西是 Xinput，它需要更多的工作。

使用 Xinput 意味着[Zachery]不能再使用通用的微软 HID 驱动程序。他决定模仿 XBOX 360 控制器，而不是自己编写驱动程序。当 fight stick 插入电脑时，它会显示为 XBOX 360 控制器，Windows 可以轻松安装预建的驱动程序。为了执行仿真，[Zachery]首先必须将设备的 VID 和 PID 设置为与 XBOX 控制器相同。这是允许微软驱动程序识别设备的原因。

接下来，设备描述符和配置描述符必须添加到 Teensy 的固件中。设备描述符包括诸如 USB 版本、设备类别、协议等信息。配置描述符包括关于设备配置的附加信息。[Zachery]使用 Microsoft Message Analyzer 从真实的 XBOX 360 控制器中提取配置描述符，然后在他自己的定制控制器中使用相同的数据。

[Zachery]用 Arduino IDE 给 TeensyLC 编程。他在这里遇到了一些麻烦，因为 IDE 没有包含 Xinput 设备的正确设备类型。[Zachery]必须编辑 boards.txt 文件并添加三行代码，以便向 IDE 的菜单添加新的硬件设备。还必须修改其他几个文件，以确保编译器知道什么是 Xinput 设备类型。所有这些都解决了之后，[Zachery]终于能够为他的控制器编写代码了。