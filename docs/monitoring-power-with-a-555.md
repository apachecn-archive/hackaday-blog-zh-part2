# 用 555 监控电源

> 原文：<https://hackaday.com/2015/06/07/monitoring-power-with-a-555/>

[Diederich]正在运行一个加载了 Pimatic 的 Raspberry Pi，这是一个很棒的家庭自动化服务器，可以做任何你可以扔给它的事情。有一点它不能做到，那就是直接从电表上监控电力和天然气——你需要硬件来实现这一点。[Diederich]挺身而出，[只用一个 555 定时器就完成了硬件](https://github.com/dkroeske/emon-server)。给他的 Pimatic 系统增加这个的总成本不到一美元。

555 可以当定时器，触发器，一堆可以[拼凑成一个 CPU](http://www.pmonta.com/555-contest/logic/logic.html) 。[Diederich]在这里没有使用一些奇特的逻辑；他只是将 555 用作施密特触发器，带有光电晶体管和电表。555 的输出连接到 Raspberry Pi 的 GPIO，一个 Python 脚本绑定到 Pimatic。

这是一个简单的解决方案，只需要一美元，使用 555 有几个优点:555 可以使用细长的导线连接到 Pi，这意味着[Diederich]的 Pi 不必位于他的电表旁边。