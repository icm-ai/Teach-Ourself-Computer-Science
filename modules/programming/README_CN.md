# 编程

[English](README.md) | 简体中文

## 概述

基础编程概念和计算思维。本模块涵盖基本的编程范式、递归、抽象和程序设计原则，这些构成了所有计算机科学学习的基础。

## 为何要学？

不要做一个「永远没彻底搞懂」诸如递归等概念的程序员。许多自学成才的工程师在编程培训中跳过了这些基础概念，只学习了特定语言的语法和框架使用。深入理解编程的基本原理将使你：

- 更深入地理解程序如何工作
- 更轻松地学习新的编程语言和范式
- 编写更优雅、更易维护的代码
- 解决更复杂的问题

> 不要做一个只写样板代码的程序员。相反，给用户和其他程序员创造工具。
>
> — Ras Bodik

## 前置要求

无。这是一门基础科目，适合初学者。

**注意：** 本指南假定你有基本的编程熟悉度。对于完全的初学者，在开始之前可能需要额外的入门资源。如果你从来没有学过编程，建议先从 [r/learnprogramming FAQ](https://www.reddit.com/r/learnprogramming/wiki/faq#wiki_getting_started) 开始。

## 编程语言

- **Scheme/Racket**（初级到中级）- 强调函数式编程；SICP 中用于教授基本概念
- **Python**（初级到中级）- Composing Programs 的替代方法；实用且易于应用

## 推荐资源

### 教材

#### 《计算机程序的构造和解释》（SICP）

**作者：** Harold Abelson, Gerald Jay Sussman, Julie Sussman

**中文版：** [《计算机程序的构造和解释》](https://book.douban.com/subject/1148282/)

**英文版：** [免费在线阅读](https://mitpress.mit.edu/sites/default/files/sicp/index.html)

**难度：** 中级

**推荐章节：** 至少前三章

**为什么选择这本书：**

SICP 是独一无二的，它可以——至少很有可能——改变你对计算机和编程的基本认识。这本书涵盖：

- 函数式编程和高阶函数
- 递归和迭代
- 数据抽象
- 流（Streams）
- 元语言抽象（解释器）

不是每个人都有这样的体验。有的人讨厌这本书，有的人看了前几页就放弃了。但潜在的回报让它值得一读。

**替代方案：**

- 如果 SICP 过于难：[*Composing Programs*](https://composingprograms.com/)（Python版本）或 [《程序设计方法》](https://book.douban.com/subject/1140942/)
- 如果 SICP 过于简单：[*Concepts, Techniques, and Models of Computer Programming*](https://book.douban.com/subject/1782316/)

#### *Composing Programs*

**作者：** John DeNero

**在线版：** [composingprograms.com](http://composingprograms.com/)

**难度：** 初级到中级

**语言：** Python

这本书「继承自 SICP」但使用 Python 讲解。对于那些更喜欢 Python 或觉得 Scheme 过于陌生的学习者，这是一个很好的替代选择。

### 视频课程

#### Brian Harvey's Berkeley CS 61A（SICP）

**讲师：** Brian Harvey

**学校：** UC Berkeley

**平台：** Internet Archive

**链接：** [课程视频](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E)

**中文字幕版：** [B站英文字幕版](https://www.bilibili.com/video/av40460492/)

**描述：** 对 SICP 概念的精炼讲解，教学清晰，特别适合新学生。这是我们对于视频课程的首选推荐。

#### MIT 6.001 - SICP 课程

**学校：** MIT

**平台：** MIT OCW

**链接：** [MIT 视频课程](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/)

**中英字幕：** [B站中英字幕版](https://www.bilibili.com/video/av8515129/)

经典的 SICP 视频课程，由作者之一 Gerald Jay Sussman 讲授。

#### John DeNero's CS 61A（Python）

**讲师：** John DeNero

**学校：** UC Berkeley

**平台：** Berkeley 课程网站

自从 2016 年以来，这门课程使用 Python 并配合 *Composing Programs* 教材。对于偏好 Python 的学生是很好的选择，但我们仍建议把 SICP、Scheme 和 Brian Harvey 的课程作为首选。

### 在线资源

- [Exercism - Scheme 练习](https://exercism.org/tracks/scheme) - Scheme 编程练习题
- [Exercism - Python 练习](https://exercism.org/tracks/python) - Python 编程练习题
- [Scheme 学习资源](https://github.com/DeathKing/Learning-SICP) - SICP 学习相关的中文资源

## 练习

### 课本习题

**来源：** SICP 书中嵌入的习题

**难度：** 初级到中级

**预计时间：** 总共 100-200 小时学习

**主题：**

- 递归和迭代过程
- 高阶函数
- 数据抽象
- 符号数据
- 流和惰性求值
- 元循环解释器

**建议：** 至少完成前三章的习题。这些习题对于理解概念至关重要。

### 编程练习

**来源：** [Exercism](https://exercism.org/)

**难度：** 多样

**预计时间：** 每个问题集 2-5 小时

**主题：** Scheme 或 Python 的特定语言练习

**建议：** 在学完 SICP 章节后，解决一些小的程序设计问题以巩固理解。

## 学习方法

### 推荐学习路径

1. **开始阅读 SICP**（或 Composing Programs）
   - 至少完成前三章
   - 不要跳过习题！
   - 每个概念都要亲手编写代码实践

2. **观看视频课程**
   - 配合阅读观看 Brian Harvey 的课程
   - 视频可以帮助你理解难点
   - 暂停视频自己思考问题

3. **完成练习**
   - SICP 书中的习题是必做的
   - 使用 Exercism 获得额外练习
   - 编写小程序巩固理解

4. **深入探索**（可选）
   - 实现书中的解释器项目
   - 探索第四章（元语言抽象）
   - 如果时间允许，学习第五章（寄存器机器）

### 时间分配建议

- **最少投入：** 100 小时（前三章 + 习题）
- **推荐投入：** 150-200 小时（包括视频课程和额外练习）
- **完整学习：** 250+ 小时（全书 + 所有项目）

### 学习技巧

1. **不要急于求成** - 这些概念需要时间消化
2. **动手实践** - 光看不练不会真正理解
3. **重复是关键** - 遇到困难的概念多练习几次
4. **参与讨论** - 加入学习社区分享理解

## 常见问题

### 为什么你们还在推荐 SICP？

先尝试读一下，有些人觉得 SICP 让人神魂颠倒，这在其他书很少见。如果你不喜欢，你可以尝试其他的东西，也许以后再回到 SICP。

### Scheme 是不是过时了？

语言只是载体。SICP 教授的是永恒的编程概念，而不是特定语言的语法。学完 SICP，你会发现学习任何新语言都变得容易。

### 我应该选择 SICP 还是 Composing Programs？

- **选择 SICP** 如果：
  - 你想要经典的、被时间验证的学习体验
  - 你不介意学习 Scheme
  - 你想要深入理解函数式编程

- **选择 Composing Programs** 如果：
  - 你更熟悉或更喜欢 Python
  - 你想要一个更现代的呈现方式
  - 你需要立即应用所学知识到 Python 项目中

### 我是完全的初学者，可以从这里开始吗？

SICP 不是为完全没有编程经验的人设计的。如果你是零基础：

1. 先学习一门编程语言的基础（Python 或 JavaScript）
2. 完成一些小项目，理解基本的变量、函数、循环
3. 然后再回来学习 SICP

推荐初学者资源：[r/learnprogramming 指南](https://www.reddit.com/r/learnprogramming/wiki/faq)

## 学习笔记

[在学习过程中可以在此添加个人笔记和关键见解]

## 进度跟踪

- [ ] 完成核心教材阅读（SICP 第 1-3 章或同等内容）
- [ ] 观看主要视频课程系列
- [ ] 完成章节习题
- [ ] 完成补充练习题
- [ ] 复习和巩固

---

**下一步：** 完成本模块后，你可以继续学习 [计算机系统结构](../computer-architecture/README_CN.md) 或 [算法与数据结构](../algorithms-and-data-structures/README_CN.md)。
