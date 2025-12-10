# 操作系统

[English](README.md) | 简体中文

## 概述

操作系统如何管理资源、进程、内存和文件系统。本模块涵盖进程管理、内存管理、文件系统、I/O 和并发。

## 为何要学？

你所写的代码，基本上都由操作系统来运行，因此你应当了解其运作的原理。

理解操作系统将使你：

- 编写更高效的程序
- 理解并发和多线程
- 调试系统级问题
- 理解安全和权限管理
- 在系统编程和后端开发中更有竞争力

## 前置要求

**推荐：**

- 计算机系统结构 - 理解硬件工作原理
- C 语言编程 - 操作系统编程主要使用 C

## 编程语言

- **C**（中级到高级）- 操作系统实现和系统编程
- **Assembly**（初级）- 理解底层细节

## 推荐资源

### 教材

#### 《操作系统导论》（OSTEP）

**作者：** Remzi H. Arpaci-Dusseau, Andrea C. Arpaci-Dusseau

**中文版：** [《操作系统导论》](https://book.douban.com/subject/33463930/)

**英文在线版：** [免费阅读](http://pages.cs.wisc.edu/~remzi/OSTEP/)

**难度：** 初级到中级

**为什么选择这本书：**

这是一个不错的替代传统教材（如《操作系统概念》「恐龙书」和《现代操作系统》）的选择。这些传统教材因为写作风格和对学生不友好而招致了一些批评。

我们格外喜欢《操作系统导论》的结构，并且认为这本书的习题很值得一做。

**主要内容：**

- 虚拟化（CPU、内存）
- 并发（线程、锁）
- 持久化（文件系统、存储）

**配套资源：**

- [OSTEP 作业](http://pages.cs.wisc.edu/~remzi/OSTEP/Homework/homework.html)
- [xv6 实验项目](http://pages.cs.wisc.edu/~remzi/OSTEP/lab-projects-xv6.pdf)

#### 传统教材（供参考）

**《操作系统概念》（恐龙书）**

- 中文版：[第9版](https://book.douban.com/subject/30297919/)
- 全面但冗长

**《现代操作系统》**

- 中文版：[第4版](https://book.douban.com/subject/27096665/)
- Andrew Tanenbaum 著，理论性强

### 操作系统实现

在读完《操作系统导论》后，我们鼓励你探索特定操作系统的设计。

#### xv6 - MIT 教学操作系统

**描述：** MIT 维护的从 Unix V6 到 ANSI C 和 x86 的移植

**为什么推荐：** 阅读小型系统内核的代码并且为其增加特性是巩固对操作系统理解的很好方法

**资源：**

- [xv6 源代码和文档](https://pdos.csail.mit.edu/6.828/2016/xv6.html)
- [xv6 book](https://pdos.csail.mit.edu/6.828/2016/xv6/book-rev9.pdf)
- [xv6 实验想法](http://pages.cs.wisc.edu/~remzi/OSTEP/lab-projects-xv6.pdf)

#### 操作系统内部实现（进阶）

- [*Lion's Commentary on Unix*](https://www.amazon.com/Lions-Commentary-Unix-John/dp/1573980137/) - Unix 源代码注释
- [*The Design and Implementation of the FreeBSD Operating System*](https://www.amazon.com/Design-Implementation-FreeBSD-Operating-System/dp/0321968972/)
- [《Linux 内核设计与实现》](https://book.douban.com/subject/6097773/) by Robert Love
- [*Mac OS X Internals*](https://www.amazon.com/Mac-OS-Internals-Systems-Approach/dp/0321278542/)

### 视频课程

#### Berkeley CS 162 - 操作系统

**学校：** UC Berkeley

**平台：** Internet Archive

**链接：** [课程视频](https://archive.org/details/ucberkeley-webcast)

**描述：** 涵盖操作系统的核心概念

**主题：**

- 进程和线程
- 调度
- 同步和死锁
- 内存管理
- 文件系统
- I/O 和设备

### 在线资源

- [OSTEP 网站](http://pages.cs.wisc.edu/~remzi/OSTEP/) - 免费教材和作业
- [xv6 项目](https://pdos.csail.mit.edu/6.828/) - MIT 6.828 课程
- [Linux 内核文档](https://www.kernel.org/doc/html/latest/)

## 练习

### OSTEP 作业

**来源：** [OSTEP Homework](http://pages.cs.wisc.edu/~remzi/OSTEP/Homework/homework.html)

**难度：** 初级到中级

**主题：** 虚拟化、并发、持久化

**建议：** 这些模拟作业帮助理解操作系统概念

### xv6 实验

**来源：** [xv6 Labs](http://pages.cs.wisc.edu/~remzi/OSTEP/lab-projects-xv6.pdf)

**难度：** 中级到高级

**预计时间：** 每个实验 10-30 小时

**项目示例：**

- 实现系统调用
- 改进调度器
- 实现虚拟内存功能
- 文件系统扩展

**建议：** 这些项目对深入理解操作系统至关重要

### 其他实践

- 编写多线程程序理解并发
- 实现简单的 shell
- 研究 Linux 内核源代码
- 使用 strace、ltrace 等工具分析系统调用

## 学习方法

### 推荐学习路径

1. **阅读《操作系统导论》**
   - 三个部分都要学习（虚拟化、并发、持久化）
   - 完成章节思考题

2. **观看 Berkeley CS 162**
   - 配合阅读观看
   - 理解不同操作系统的设计权衡

3. **完成 OSTEP 作业**
   - 使用模拟器理解概念
   - 分析和实验

4. **深入 xv6**
   - 阅读 xv6 源代码
   - 完成至少 2-3 个 xv6 实验
   - 理解真实操作系统的实现

5. **探索现代操作系统**（可选）
   - 阅读 Linux 内核相关书籍
   - 研究特定子系统（如调度器、内存管理）

### 时间分配建议

- **最少投入：** 100 小时（OSTEP + 基础作业）
- **推荐投入：** 150-200 小时（包括 xv6 实验）
- **深入学习：** 250+ 小时（Linux 内核研究）

### 学习技巧

1. **动手实践** - 光看书不够，必须写代码
2. **画图理解** - 进程状态、内存布局等需要可视化
3. **调试技能** - 学会使用 GDB 调试系统程序
4. **阅读代码** - 读 xv6 或 Linux 源代码加深理解
5. **实验环境** - 建议使用虚拟机，避免破坏主系统

## 常见问题

### 先学计算机系统结构还是操作系统？

**强烈建议先学计算机系统结构**。理解硬件如何工作对学习操作系统至关重要。

### 需要深入学习 Linux 内核吗？

取决于职业方向：

- **系统程序员** - 是的，需要深入理解
- **后端开发** - 理解基本原理即可
- **应用开发** - OSTEP 的水平就足够

### xv6 过时了吗？

xv6 虽然基于老的 Unix，但它：

- 代码简洁易懂（约 10,000 行）
- 包含操作系统的核心概念
- 是学习的绝佳工具

学完 xv6 后，理解现代操作系统会容易很多。

### 如何选择学习哪个操作系统？

- **Linux** - 最广泛使用，资源丰富
- **FreeBSD** - 代码质量高，文档好
- **xv6** - 教学用，最适合初学者

建议：先学 xv6，再根据兴趣选择 Linux 或其他。

## 学习笔记

[在学习过程中可以在此添加个人笔记和关键见解]

## 进度跟踪

- [ ] 完成《操作系统导论》核心内容
- [ ] 观看主要视频课程
- [ ] 完成 OSTEP 作业
- [ ] 阅读 xv6 源代码
- [ ] 完成至少 2 个 xv6 实验项目
- [ ] 理解虚拟化、并发和持久化的核心概念
- [ ] 复习和巩固

---

**下一步：** 学完操作系统后，建议学习 [计算机网络](../computer-networking/README_CN.md) 或 [数据库](../databases/README_CN.md)。
