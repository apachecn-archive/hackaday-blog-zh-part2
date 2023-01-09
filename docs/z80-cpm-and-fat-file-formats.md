# Z80、CP/M 和 FAT 文件格式

> 原文：<https://hackaday.com/2014/12/30/z80-cpm-and-fat-file-formats/>

[加里·基尔代尔]和 CP/M 是计算世界的伟大“失败者”;CP/M 可以在数千台不同的 20 世纪 80 年代的电脑上运行，由于 CP/M 的流行，[Gary]每年看到几百万的收入。微软、DOS 和环境已经把[Kildall]和 CP/M 贬为微型计算机历史上一个相当长的脚注，但这并不意味着 CP/M 已经完全死亡。[【Marcelo】写了一个在 Arduino 内部运行 CP/M 的 Z80 仿真器](http://hackaday.io/project/3709-cpmduino)，他以一种实际上方便且有用的方式完成了它。

[Marcelo]的模拟器不使用 CP/M 磁盘映像，而是在常规的 FAT 文件系统上模拟 CP/M 磁盘驱动器。驱动器被映射到 FAT 文件系统中的文件夹，因此名为“A”的文件夹将显示为 CP/M 中的 A:磁盘。支持高达 P:的驱动器，这是 CP/M 下可用的最大驱动器数量。BIOS 驻留在 SD 卡的根目录中，到目前为止，Microsoft Basic、Turbo Pascal、UCD micro 腮腺炎和 Wordstar 工作正常。

Arduino 项目是建立在[Marcelo]早期的一个项目[之上的，这个项目将 CP/M 模拟器放在了 Windows](http://sourceforge.net/projects/runcpm/)上。[Due](http://sourceforge.net/projects/cpmduino/)的版本完全按照你想的那样工作，串行连接和终端仿真器提供 IO，Due 上大量的处理能力和 RAM 完成所有繁重的工作。