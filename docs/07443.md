# 黑客日奖:对一位芯片语者的采访

> 原文：<https://hackaday.com/2014/10/29/the-hackaday-prize-interview-with-a-chipwhisperer/>

![chipwhisperer](img/ad0cc0c1393743f03c01c622f8781402.png)

每个 Hackaday 奖的决赛选手都有一些以前没有做过的事情；用一些 3D 打印部件找到所有东西的化学成分是一件新奇的事情，用现成的部件建立一个全球卫星地面站网络也是如此。[【科林】的《ChipWhisperer》有一些可怕而有趣的暗示。](http://hackaday.io/project/956-chipwhisperer-security-research)通过观察微控制器内部的运行情况，ChipWhisperer 能够验证或破解这些芯片的安全性。另外*非常有趣*而且有点神奇的是，仅仅通过查看功耗就能知道芯片在处理什么数据。

我们还不知道谁是 Hackaday 奖的得主，我希望在两周后的派对前不知道这个事实。在那之前，你可以看看对[科林·奥弗林]的简短采访，或者看看他为下面的 ChipWhisperer 制作的五分钟视频:

[https://www.youtube.com/embed/Y_Gg0aiN2Eo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Y_Gg0aiN2Eo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

```
*How seriously are the backdoors the Chipwhisperer opens taken
in the industry? Are we looking at a huge problem with on-chip
security out there, simply because the tools to investigate
them have been really expensive?*
```

对于关心安全的人，因为他们直接有钱可输
(想想芯片& pin 信用卡，卫星机顶盒等。他们认真对待这些问题已经很久了。但是大多数嵌入式
系统都不属于这一类，而正是这些产品最终容易受到攻击。部分问题是设计工程师或者
不知道这些攻击。或者工程师们相信他们购买的供应商，他们出售加密库、硬件加速器或独立的芯片作为完全防弹的系统。

这个问题可能不是
密码设计中的基本缺陷之一，而是更多的用户(即设计工程师)没有完全
理解密码的具体实现有多“安全”。

```
*If you could give 100 words of advice to embedded designers 
implementing* *encryption, what would you tell them?*
```

加密不是复选框。每个实现都有漏洞，你的问题是我需要多安全？如果有人能够确定一个设备中的秘密密钥，这是否意味着他们现在能够获得所有类似设备的
访问权？旁道分析
暴露的问题通常会因经典错误而变得更糟，例如跨多个设备重用密钥材料
以使部署更容易，但当设备
实际上不需要共享密钥时(想想固件映像)。

```
*You’ve already said a few people have gotten the files* *and 
built their own ChipWhisperer. You’re also selling the 
complete kit.* *Who is buying it? Are we looking at academics,
security researchers,* *companies verifying their own hardware,
or just random people who sign their* *emails ZeroCool?*
```

到目前为止，大部分是学者，尽管也有一些安全研究人员和公司。我的设计意图是让它成为一个学习工具，并且尽我所能
合理地让它远离‘攻击性攻击工具’。除非你理解
攻击的基本理论，否则你永远不会成功。

```
*What was the reaction from different communities? What was the
response* *from security researchers versus the general public? 
Are you surprised at* *how popular your project was?*
```

最大的反应来自嵌入式工程师，因为他们在设计过程中经常被“因为数学而安全”所说服。例如，他们
使用 AES-256，并假设这意味着有人攻击系统
将需要物理解封芯片，重置熔丝位，然后读取
闪存以获得密钥。他们从未见过
旁道攻击的实际演示，只是隐约听说过。

我很惊讶这个项目在这个领域之外如此受欢迎！比我第一次意识到的多得多的人参与了侧信道功耗分析，这很值得学习。我创办了一个网络论坛，目的是
尝试收集一些社区信息，因为以一种更非正式的方式分享
研究成果会很棒。

```
*Hypothetical, and we’re not going to hold you to whatever answer
you give. You win the grand prize, a trip to space or about
$200,000 USD. Which one to you take, and what is your reasoning 
for doing so?*
```

太空之旅会很棒，但我想我会有一段地狱般的时光
拒绝 20 万美元！不过，毫无疑问，我会将这笔钱再投资到这个
项目中。我真的想创造这些工具的低成本版本，
，其中很大一部分是用更先进的
技术进行更大规模的生产(将 FPGA 直接安装在多层 PCB 上)。到目前为止，我一直避免使用
Kickstarter，因为我希望这个项目保持相当的技术性——如果我
走 Kickstarter 的路线，我担心我会和那些只
使用过 Arduino 支持这个项目的人一起结束，然后当我
要求他们编译 C 代码时，我会感到沮丧。我也避免尝试获得外部投资者，因为他们想要缩减项目的开源/免费性质。我还在攻读博士学位，所以不能太分心，因为我想先完成它！

无论哪种方式，我都需要检查该奖项的税收影响——如果我必须为该奖项支付全部加拿大所得税，我无论如何都负担不起太空之旅，即使赞助商的规定提供了价值的 20%来覆盖 T2！不幸的是，实际问题可能会左右我的选择。