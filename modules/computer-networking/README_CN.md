# 计算机网络

[English](README.md) | 简体中文

## 概述

互联网架构、协议和网络系统通信。本模块涵盖网络分层模型、TCP/IP 协议栈、路由、DNS 和网络应用。

## 为何要学？

互联网已然势不可挡：理解工作原理才能解锁全部潜力。

鉴于有那么多关于网络服务端和客户端的软件工程，计算机网络是计算机科学中价值最为「立竿见影」的领域之一。我们的学生，系统性地学习了计算机网络，最终能够理解那些曾困扰他们多年的术语、概念和协议。

> 你无法盯着水晶球预见未来，未来的互联网何去何从取决于社会。
>
> — Bob Kahn

## 前置要求

**推荐：**

- 编程 - 能够编写网络程序
- 操作系统 - 理解进程、并发等概念

## 编程语言

- **Python**（初级到中级）- 网络编程和协议实现
- **C**（中级）- 底层网络编程
- **任何语言** - 网络概念适用于所有语言

## 推荐资源

### 教材

#### 《计算机网络：自顶向下方法》

**作者：** James Kurose, Keith Ross

**中文版：** [《计算机网络：自顶向下方法》第7版](https://book.douban.com/subject/30280001/)

**英文版：** Computer Networking: A Top-Down Approach

**难度：** 初级到中级

**为什么选择这本书：**

这本书采用「自顶向下」的方法，从应用层开始，逐步深入到物理层。这种方法更符合现代软件工程师的需求，因为我们通常从编写网络应用开始。

**主要内容：**

- 应用层（HTTP、DNS、SMTP 等）
- 传输层（TCP、UDP）
- 网络层（IP、路由）
- 链路层和物理层
- 网络安全

**配套资源：**

- [Wireshark Labs](http://www-net.cs.umass.edu/wireshark-labs/) - 实践抓包分析
- 书籍配套网站的补充材料

### 视频课程

#### Stanford CS 144 - Introduction to Computer Networking

**学校：** Stanford University

**平台：** Lagunita (Stanford MOOC)

**链接：** [CS 144](https://lagunita.stanford.edu/courses/Engineering/Networking-SP/SelfPaced/about)

**描述：** 优秀的网络课程，配合教材学习效果很好

**主题：**

- 分层网络模型
- TCP/IP 协议栈
- 路由算法
- 网络应用设计

### 在线资源

- [Wireshark Labs](http://www-net.cs.umass.edu/wireshark-labs/) - 网络协议抓包实验
- [Beej's Guide to Network Programming](https://beej.us/guide/bgnet/) - Socket 编程指南
- [High Performance Browser Networking](https://hpbn.co/) - 免费在线书籍

## 练习

### Wireshark Labs

**来源：** [Wireshark Labs](http://www-net.cs.umass.edu/wireshark-labs/)

**难度：** 初级到中级

**主题：**

- HTTP 协议分析
- DNS 查询
- TCP 连接
- UDP 通信
- IP 数据包
- 以太网帧

**为什么重要：** 这些实验帮助你真正理解网络协议如何工作，而不仅仅是理论。

### 编程项目

对于计算机网络的学习，做项目比完成小的习题更有益。

**推荐项目：**

1. **HTTP 服务器**
   - 实现基本的 HTTP/1.1 服务器
   - 支持 GET、POST 请求
   - 处理静态文件

2. **基于 UDP 的聊天应用**
   - 实现可靠传输（确认、重传）
   - 理解 TCP 的设计动机

3. **迷你 TCP 栈**
   - 在用户空间实现简单的 TCP
   - 理解三次握手、流量控制等

4. **代理服务器**
   - HTTP 代理
   - 缓存功能
   - 负载均衡

5. **分布式哈希表（DHT）**
   - 实现简单的 P2P 网络
   - 理解分布式系统基础

## 学习方法

### 推荐学习路径

1. **阅读《计算机网络：自顶向下方法》**
   - 按章节顺序学习
   - 理解每一层的职责和协议

2. **完成 Wireshark Labs**
   - 边学边做实验
   - 亲手抓包分析协议
   - 这些实验对理解至关重要

3. **观看 Stanford CS 144**
   - 配合阅读观看
   - 关注设计原理和权衡

4. **编程实践**
   - 实现至少 2-3 个网络项目
   - 从简单的 Socket 编程开始
   - 逐步实现复杂的协议

5. **深入学习**（可选）
   - 研究网络安全（防火墙、VPN）
   - 学习高级主题（SDN、网络虚拟化）
   - 阅读 RFC 文档

### 时间分配建议

- **最少投入：** 100 小时（教材 + Wireshark Labs）
- **推荐投入：** 150-200 小时（包括编程项目）
- **深入学习：** 250+ 小时（高级主题 + 大型项目）

### 学习技巧

1. **抓包分析** - 使用 Wireshark 观察真实网络流量
2. **画图理解** - 网络拓扑、数据流向需要可视化
3. **动手编程** - 实现协议才能真正理解
4. **阅读 RFC** - 了解协议的官方规范
5. **调试网络** - 学会使用 ping、traceroute、netstat 等工具

## 补充资源

### Socket 编程

- [Beej's Guide to Network Programming](https://beej.us/guide/bgnet/) - Socket 编程经典指南
- 《Unix 网络编程》 - [卷1：套接字联网API](https://book.douban.com/subject/4859464/)

### 性能优化

- [High Performance Browser Networking](https://hpbn.co/) - Web 性能优化

### 网络安全

- 学习完基础网络后，可以探索网络安全主题
- 理解常见攻击（DDoS、中间人攻击等）

## 常见问题

### 需要学习 OSI 七层模型吗？

重点学习 TCP/IP 四层/五层模型：

- 应用层
- 传输层
- 网络层
- 链路层
- (物理层)

OSI 七层模型了解即可，实际应用中 TCP/IP 模型更重要。

### Wireshark Labs 真的有必要做吗？

**非常有必要！** 这些实验：

- 让你看到协议的真实运行
- 理解理论和实践的区别
- 培养网络调试能力

不做实验只看书，你不会真正理解网络。

### 需要了解物理层吗？

对于软件工程师：

- **不必深入** 物理层（电信号、调制等）
- **需要理解** 链路层基础（以太网、Wi-Fi）
- **重点掌握** 网络层及以上

除非你从事网络硬件或嵌入式开发，否则物理层的基本概念就足够了。

### 如何学习网络编程？

1. **从 Socket 开始** - 学习 TCP/UDP Socket 编程
2. **实现协议** - 自己实现简单的应用层协议
3. **使用框架** - 学习现代网络框架（如 Node.js、Flask）
4. **理解异步** - 掌握异步 I/O 和事件驱动编程

## 学习笔记

[在学习过程中可以在此添加个人笔记和关键见解]

## 进度跟踪

- [ ] 完成《计算机网络：自顶向下方法》核心章节
- [ ] 观看 Stanford CS 144 课程
- [ ] 完成所有 Wireshark Labs
- [ ] 实现至少 2 个网络编程项目
- [ ] 理解 TCP/IP 协议栈
- [ ] 掌握网络调试工具
- [ ] 复习和巩固

---

**下一步：** 学完计算机网络后，建议学习 [分布式系统](../distributed-systems/README_CN.md)，因为分布式系统建立在网络基础之上。
