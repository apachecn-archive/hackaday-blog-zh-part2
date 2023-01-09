# ChipWhisperer 点击 Kickstarter

> 原文：<https://hackaday.com/2015/02/27/chipwhisperer-hits-kickstarter/>

如果有人足够聪明，将示波器连接到处理器上，即使设计得最好的加密算法也能被破解。在过去 15 年左右的时间里，围绕电源和侧信道分析技术出现了一个完整的嵌入式安全领域。这些工具既昂贵又稀有，但是[【科林·奥弗林】和芯片语者在这里](https://www.kickstarter.com/projects/coflynn/chipwhisperer-lite-a-new-era-of-hardware-security)为大众带来一个硬件安全的新时代。

ChipWhisperer 是去年 Hackaday 奖的第二名。这是一个有趣的安全研究领域，也是以前研究起来极其昂贵的领域。如果你想对“芯片密语者”做些什么有个大概的了解，你可能想看看去年我们在 DEFCON 上偶遇[科林]时的[。](http://hackaday.com/2014/08/20/the-chipwhisperer-at-defcon/)

虽然 ChipWhisperer 的最初目标是将电源和侧信道分析所需的工具成本降低到黑客空间或研究人员可以承受的水平，但对于 Kickstarter 活动来说，这仍然过于昂贵。为此，[科林]设计了 ChipWhisperer Lite，这是一个精简版，但仍能做原版能做的大部分事情。

ChipWhisperer Lite 由两部分组成，主要部分包含一个大型微控制器、一个大型 FPGA 和一个高增益、低噪声放大器。这是 ChipWhisperer 的核心，也是所有功耗分析发生的地方。另一部分是包含 XMega 微控制器的目标板。这是您运行所有加密算法的地方，也是您发现它们是否能被功耗分析破解的地方。主板和目标板通过分离连接固定在一起，因此如果您想在另一个板上运行*功耗分析，只需将 ChipWhisperer 一分为二。*

[Colin]将推出一款约 200 美元的 ChipWhisperer Lite，远低于这些工具仅在一年前的价格。我们期待着一次成功的宣传活动，以及这个委员会的成员将会发现的所有有趣的发现。