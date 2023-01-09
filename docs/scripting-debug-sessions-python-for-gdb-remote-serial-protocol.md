# 脚本调试会话:Python For GDB 远程串行协议

> 原文：<https://hackaday.com/2014/09/22/scripting-debug-sessions-python-for-gdb-remote-serial-protocol/>

你厌倦了在 GDB 一遍又一遍地敲同样的命令吗？如果没有，我们强烈建议您充分利用 GNU 项目调试器，这是一种在微控制器运行程序时探索其内部的绝佳方式。

回到手头的事情。[Stef]编写了一个利用 GDB 远程串行协议的 Python 程序。他称之为 pyrsp，他最近关于它的演讲可以在下面看到。

核心特性是能够在 C 代码中添加回调来触发 Python 脚本。这有点像打印声明，除了你有这么多的权力，因为它是 Python 和 GDB 做的“打印”。在 GDB 可以在断点处完成的任何事情现在都可以自动执行。因此，如果你需要在每次循环执行时检查一组寄存器来完成数百次循环，你的手腕会感谢你的。更好的是，您可以使用 Python 自动进行健全性检查，当数据良好时继续检查，当数据不好时提醒您。整洁！

[https://www.youtube.com/embed/NVeZFxTroEw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NVeZFxTroEw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)