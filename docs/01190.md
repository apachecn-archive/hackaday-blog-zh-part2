# 从希捷硬盘固件错误中恢复

> 原文：<https://hackaday.com/2012/07/30/recovering-from-a-seagate-hdd-firmware-bug/>

硬盘固件是你最不想发现错误的地方。但事实证明，这是他在 RAID 阵列中使用的希捷硬盘的问题。它完全停止工作，他后来发现固件有一个错误，使驱动器认为它永远处于忙碌状态。有一个固件升级可用，但你必须在问题出现之前应用它，否则你就要倒霉了。经过一番搜索，他找到了解决问题的硬件解决方案。

[Brad Garcia]将说明解除 7200.11 硬盘繁忙状态错误所需步骤的教程放在一起。右下方的图像显示了在 PCB 和控制磁头的连接器之间有一张纸的驱动器。这是必要的，以引导驱动器没有它挂起由于错误。在那里，他发出一系列命令，将它放入访问级别 2，然后移除纸板进行剩余的修复。

在教程中[Brad]使用了一个串行 TTL 转换器。[BBfoto]取而代之的是一个 Arduino，[用它作为 USB-ttl 桥](http://www.reddit.com/r/sysadmin/comments/xcjdw/arduino_saved_a_10tb_raid5_array_from_total/)。