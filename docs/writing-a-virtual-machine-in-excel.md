# 在 Excel 中编写虚拟机

> 原文：<https://hackaday.com/2014/12/25/writing-a-virtual-machine-in-excel/>

[Á·达姆]参加了一个名为“科马尔”的比赛。这是一本面向初中和高中学生的杂志，每月 9 期，以数学和物理问题为特色。[保罗·erdős]，有史以来发表论文最多的数学家之一，是一个巨大的参与者，也是迄今为止最著名的学生，在一百年的历史中打开了一份柯马尔。[Á·达姆]正在尝试解决 Excel 中的一个问题，但是官方规定禁止使用 Excel 宏。迷迷糊糊中，他想出了 Excel 最巧妙的用法之一:[用最流行的电子表格程序](https://hackaday.io/project/3680-exembler)构建汇编解释器。

这是一台没有可写 RAM 的虚拟哈佛架构机器；堆栈只有很多很多的如果。指令——主要是 load、MOV、JNZ、INC 和 CMP [解决了这个问题](http://www.komal.hu/verseny/feladat.cgi?a=honap&h=201411&t=inf&l=en)，检查两个输入看它们是否是彼此的倍数。如果您想知道，来自[Á·达姆]的 Excel 表格的一个示例单元格如下所示:

```
=F6
   INDEX($C$2:$C99999,$G2,1),
   IF(AND(INDEX($B$2:$B99999,$G2,1)="JZ",$I2=0),
      INDEX($C$2:$C99999,$G2,1),
         IF(AND(INDEX($B$2:$B99999,$G2,1)="JNZ",$I2<>0),
         INDEX($C$2:$C99999,$G2,1),
         G2+1
         )
      )
   )
)
```

[Á·dám]在 hackaday.io 上提供了他的 Excel 解决方案。它是匈牙利语的，这真的不重要，因为它基本上是 Excel 和伪 x86 指令集。但是列标签需要一点谷歌翻译。