# 利用 LTSpice 测量总谐波失真

> 原文：<https://hackaday.com/2015/09/07/using-ltspice-to-measure-total-harmonic-distortion/>

音响发烧友花费大量时间和精力担心音频规格，如总谐波失真(THD)。有道理，因为 THD 影响音频再现的质量。然而，THD 也会影响无线电信号的干扰，甚至影响功率传输系统的损耗。一个简单的定义是，THD 是所有谐波频率功率之和与基频功率之比。

如果电路产生完美的正弦波，就不会有谐波。在实践中有许多方法可以测量 THD，但是[迈克尔·杰克逊]有一个有趣的视频展示了他如何使用 lt spice 轻松地可视化 THD。假设你已经在 [LTSpice](http://www.linear.com/designtools/software/) 中有了这个系统(或者你可以使用另一个模拟工具，如果你喜欢的话)，这是相当简单的。

关键的概念是找到期望的输出是什么。在[Michael 的]例子中，他有一个带模拟输入的放大器，因此他将负载阻抗调得很高，以找到实际的电压增益。然后，他模拟了一个完美的差分放大器和一个与放大器预期输出相匹配的完美信号源。

剩下的可能很明显了。更换负载，观察差分放大器的输出。您可以对其进行 FFT，以进一步了解发生了什么。当然，尽管香料很好，但它不是现实。您在现实世界中的结果可能会有所不同。但是这项技术至少在寻找(并推测纠正)高 THD 的潜在来源方面是伟大的。

如果你对电子管放大器感兴趣，THD 是一个重要的话题。电子管放大器的建模可能比制造容易得多。连接板电源和在机箱上打孔只是为了发现你的总谐波失真比你希望的要高，这将是一种浪费。

[https://www.youtube.com/embed/GKlMVNoQGiY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GKlMVNoQGiY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)