# 黑客移除 NVIDIA 显卡的固件瘫痪

> 原文：<https://hackaday.com/2013/03/18/hack-removes-firmware-crippling-from-nvidia-graphics-card/>

如果硬件制造商想要保守他们的固件瘫痪的秘密，也许他们不应该和 Linux 用户捣乱？我们认为，如果你使用 Linux，你比普通 Windows 用户更有可能打开某些东西，看看里面藏着什么。因此，我们开始讲述[Gnif]如何发现 NVIDIA GTX690 可以像 Quadro k 5000 一样运行的故事。事情是这样的，后者比前者贵了将近 800 美元！

[Gnif]想要该卡用于游戏并支持多显示器。它在 Windows 下驱动多达三个屏幕没有问题。但是 Linux 驱动程序只允许在 GTX690 的专业版本 Quadro K5000 上使用。原来，卡响应由一系列模拟值分配的设备 ID。这些可以通过交换、猛拉或在正确的位置添加电阻来调整。正如我们几天前看到的用安捷伦万用表解锁他的的[一样，他不知何故设法找到了解锁隐藏在这张卡中的能量的秘方。](http://hackaday.com/2013/03/14/eeprom-hack-unlocks-crippled-features-in-agilent-multimeter-and-lcr-meter/)