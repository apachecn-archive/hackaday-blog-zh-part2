# 入侵 Nike+ Fuelband

> 原文：<https://hackaday.com/2015/01/30/hacking-the-nike-fuelband/>

[Simone]试图对他的 Nike+ Fuelband 的蓝牙协议进行逆向工程，并取得了一些惊人的发现。[Simone]发现 Fuelband 的认证系统可以很容易地被绕过，并发现一些低级功能(如任意读取和写入内存)完全暴露给最终用户或任何其他通过认证过程的人。

[Simone]从 Fuelband 的 Nike 官方应用开始。他将 APK 转换为 JAR，然后使用 JD-Gui 读取应用程序的 Java 源代码。通读源代码后，他发现认证方法完全无效。认证器要求连接设备知道 pin 码和随机数，但实际上认证算法只是检查硬编码的令牌 *0xff 0xff 0xff 0xff 0xff 0xff* ，使得整个认证过程无效。

在他通过 Fuelband 认证后，[Simone]开始尝试各种命令，看看他可以通过蓝牙接口控制什么。他发现他可以将设备发送到 bootloader 模式，配置 RTC，甚至通过蓝牙接口读/写第一个 65k 的内存——这不是您通常希望暴露的事情，尤其是在身份验证机制失效的情况下。如果你想自己尝试这个漏洞，[Simone]写了一个 Android 应用程序，他[把它发布在 GitHub](https://github.com/evilsocket/nikeplus-fuelband-se-reversed)上。