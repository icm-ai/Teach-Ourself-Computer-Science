# 数据库

[English](README.md) | 简体中文

## 概述

数据库系统、SQL、事务处理和数据建模。本模块涵盖关系型数据库、查询优化、事务和分布式数据库基础。

## 为何要学？

对于多数重要程序，数据是其核心，然而很少人理解数据库系统的工作原理。

比起其他主题，自学数据库系统需要更多的付出。这是一个相对年轻的研究领域，并且出于很强的商业动机，研究者把想法藏在紧闭的门后。此外，许多原本有潜力写出优秀教材的作者反而选择了加入或创立公司。

鉴于如上情况，我们鼓励自学者大体上抛弃教材，而是从课程开始，然后前往阅读论文。

## 前置要求

**推荐：**

- 编程 - 能够编写数据库应用
- 数据结构 - 理解树、哈希表等
- 操作系统 - 理解文件系统、并发

## 编程语言

- **SQL** - 数据库查询语言（必须）
- **任何编程语言** - 用于实现数据库或编写应用

## 推荐资源

### 核心资源

#### Readings in Database Systems（红书）

**编者：** Peter Bailis, Joe Hellerstein, Michael Stonebraker

**在线版：** [redbook.io](http://www.redbook.io/)

**英文原版：** [Readings in Database Systems](https://book.douban.com/subject/2256069/)（暂无中文版）

**难度：** 中级到高级

**为什么选择：**

这是由顶级数据库研究者编纂的论文合集。对于想要在基础课程水平更进一步的学习者，「红书」应当是首选。

**主要内容：**

- 传统 RDBMS 系统
- 新SQL数据库
- NoSQL 系统
- 大规模数据处理
- 一致性模型

#### Architecture of a Database System

**作者：** Joe Hellerstein, Michael Stonebraker, James Hamilton

**在线阅读：** [免费PDF](http://db.cs.berkeley.edu/papers/fntdb07-architecture.pdf)

**难度：** 中级

**为什么重要：**

这篇论文提供了独特的对关系型数据库管理系统（RDBMS）如何工作的高层次观点，是后续学习的实用梗概。

**建议：** 在学习数据库之初就读这篇论文，建立整体认识。

### 教材（可选）

#### 《数据库管理系统：原理与设计》

**作者：** Raghu Ramakrishnan, Johannes Gehrke

**中文版：** [《数据库管理系统：原理与设计》](https://book.douban.com/subject/1155934/)

**难度：** 中级

**何时使用：** 如果你坚持一定要一本导论教材

### 视频课程

#### Berkeley CS 186 - 数据库系统导论

**学校：** UC Berkeley

**讲师：** Joe Hellerstein

**平台：** Internet Archive

**链接：** [2015年春季课程](https://archive.org/details/UCBerkeley_Course_Computer_Science_186)

**描述：** 优秀的数据库课程，我们建议从这门课开始

**主题：**

- 关系模型和 SQL
- 索引（B+ 树、哈希）
- 查询优化
- 事务和并发控制
- 恢复
- 分布式数据库

### 进阶资源

#### 事务处理

**书籍：** [*Transaction Processing: Concepts and Techniques*](https://book.douban.com/subject/2586390/) by Jim Gray

**难度：** 高级

**何时阅读：** 深入学习事务处理的经典著作

#### 数据建模

**书籍：** [*Data and Reality*](https://book.douban.com/subject/17915870/)

**为什么推荐：**

数据模型往往是数据库中一个被忽视的、教学不充分的方面。这本书提供了永恒的关于感知和管理数据的视角。

## 练习

### CS 186 项目

**来源：** Berkeley CS 186 课程

**难度：** 中级到高级

**典型项目：**

- 为 Spark 添加特性
- 实现 B+ 树索引
- 查询优化器
- 并发控制

**建议：** CS 186 课程的学生给 Spark 添加特性，这是不错的项目。

### 自己实现数据库

**项目：** 从零实现一个简单的关系型数据库管理系统

**难度：** 高级

**预计时间：** 100+ 小时

**为什么要做：**

如果没有编写足够数量的代码，很难巩固数据库理论。自然，它将不会有太多的特性，但是即便只实现典型的关系型数据库管理系统每个方面最基础的功能，也是相当有启发的。

**核心组件：**

1. **存储管理** - 页面、缓冲池
2. **索引** - B+ 树或哈希索引
3. **查询处理** - 解析、执行
4. **事务** - 简单的锁机制
5. **恢复** - 日志和检查点

### SQL 练习

**平台：**

- [LeetCode Database](https://leetcode.com/problemset/database/) - SQL 练习题
- [HackerRank SQL](https://www.hackerrank.com/domains/sql) - 从基础到高级
- [SQL Zoo](https://sqlzoo.net/) - 交互式 SQL 教程

## 学习方法

### 推荐学习路径

1. **观看 Berkeley CS 186**
   - 从课程开始建立系统性认识
   - 做课程笔记
   - 理解关键概念

2. **阅读 Architecture of a Database System**
   - 在学习初期阅读
   - 理解 DBMS 的整体架构
   - 为深入学习做准备

3. **学习 SQL**
   - 熟练掌握 SQL 查询
   - 理解查询优化
   - 练习复杂查询

4. **阅读红书论文**
   - 选择感兴趣的章节
   - 理解数据库系统的演进
   - 了解现代数据库系统

5. **编程实践**
   - 完成 CS 186 项目（如果可以）
   - 或者从零实现简单数据库
   - 理解实现细节

6. **深入专题**（可选）
   - 分布式数据库
   - 列式数据库
   - NoSQL 系统
   - 时序数据库

### 时间分配建议

- **最少投入：** 100 小时（CS 186 + SQL）
- **推荐投入：** 150-200 小时（包括论文阅读和项目）
- **深入学习：** 250+ 小时（实现数据库 + 高级主题）

### 学习技巧

1. **理解架构** - 从整体到局部理解数据库系统
2. **动手实践** - SQL 和实现都需要大量练习
3. **读论文** - 数据库领域论文质量高，值得细读
4. **性能分析** - 理解查询计划和性能优化
5. **实际应用** - 在项目中应用所学知识

## 学习资源

### 经典论文

从红书和以下资源选择：

- [Papers We Love - Databases](https://github.com/papers-we-love/papers-we-love/tree/master/databases)
- [MIT 6.824 阅读清单](https://pdos.csail.mit.edu/6.824/schedule.html)

### 在线教程

- [SQL Tutorial](https://www.sqltutorial.org/) - SQL 基础教程
- [Use The Index, Luke](https://use-the-index-luke.com/) - SQL 索引优化

### 数据库系统

**学习用：**

- SQLite - 简单，适合学习源码
- PostgreSQL - 功能强大，文档完善

**生产环境：**

- PostgreSQL
- MySQL/MariaDB
- 云数据库（AWS RDS、Google Cloud SQL）

## 常见问题

### 需要深入学习 SQL 吗？

是的，非常重要！

- **基础 SQL** - SELECT、JOIN、子查询（必须掌握）
- **高级 SQL** - 窗口函数、CTE、性能优化（推荐掌握）
- **数据库管理** - 索引、事务、权限（了解即可）

### NoSQL 数据库怎么样？

先学好关系型数据库：

1. 关系型数据库的概念是基础
2. 许多 NoSQL 系统的设计是对关系型的反思
3. 理解关系型后，NoSQL 更容易理解

之后可以学习：

- 文档数据库（MongoDB）
- 键值存储（Redis）
- 列族数据库（Cassandra）
- 图数据库（Neo4j）

### 需要实现一个数据库吗？

不是必须，但强烈推荐：

- **好处：** 深入理解内部机制
- **时间：** 需要大量时间投入
- **替代：** 可以通过 CS 186 项目或研究现有数据库源码

### 数据建模重要吗？

非常重要但经常被忽视：

- 好的数据模型是成功的一半
- 糟糕的设计会导致性能问题
- 需要理论和实践结合

推荐阅读 *Data and Reality* 培养数据建模思维。

## 学习笔记

[在学习过程中可以在此添加个人笔记和关键见解]

## 进度跟踪

- [ ] 观看 Berkeley CS 186 课程
- [ ] 阅读 Architecture of a Database System
- [ ] 掌握 SQL 查询和优化
- [ ] 阅读红书中的精选论文
- [ ] 完成至少一个数据库实现项目
- [ ] 理解事务、并发控制和恢复
- [ ] 复习和巩固

---

**下一步：** 学完数据库后，可以学习 [分布式系统](../distributed-systems/README_CN.md)，其中包括分布式数据库的内容。
