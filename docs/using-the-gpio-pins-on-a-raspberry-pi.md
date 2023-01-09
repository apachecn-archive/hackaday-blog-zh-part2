# 在 Raspberry Pi 上使用 GPIO 引脚

> 原文：<https://hackaday.com/2012/06/17/using-the-gpio-pins-on-a-raspberry-pi/>

除了是一个可维护的单板计算机外，Raspberry Pi 还有一个装满 GPIO 引脚的接头，供您随时调用。[Tedbot]发来了一篇关于在 Python、Bash 和 c 语言中使用这些引脚的精彩教程。

Raspi 上的 GPIO 引脚排列在一个 2×13 的接头中。在 Sparkfun 设法制造出像样的 Raspi 原板之前，最简单的方法是用一根旧的 IDE 带状电缆断开这些引脚。将另一端插入试验板后，[Tedbot]就有了一套易于使用的 Raspi 引脚。

为了控制这些管脚，[Tedbot]找到了两个库:第一个是 [WiringPi](https://projects.drogon.net/raspberry-pi/wiringpi/) ，它在 Raspi 上实现了一个 C 风格的类似 Arduino 的编程环境。第二个是 [RPi。GPIO Python 包](http://pypi.python.org/pypi/RPi.GPIO)。由于 Raspi 运行 Linux，*Unix 中的一切都是一个文件*，【ted bot】[使用一个 shell 脚本](http://elinux.org/RPi_Low-level_peripherals#GPIO_Driving_Example_.28Shell_script.29)来闪烁 LED。

如果您正在构建一个电路板来扩展 Raspi 的功能，有一点需要提醒:这些引脚不支持 5 V，因此在构建 Raspi 电路时，您需要加入一个缓冲器或电平转换器。

编辑:Adafruit 将在几周后发布一款 [Pi Plate 原型板](http://www.adafruit.com/products/801)。很整洁，是吧？