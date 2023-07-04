# 第6章 goroutine
## 6.1 进程、线程与协程
### 6.1.1 进程
![](https://img.github.mailjob.net/book-go-runtime/6.1.1.mp4)
### 6.1.2 线程
![](https://img.github.mailjob.net/book-go-runtime/6.1.2.mp4)
### 6.1.3 协程
![](https://img.github.mailjob.net/book-go-runtime/6.1.3.mp4)
## 6.2 IO 多路复用
### 6.2.1 三种网络 IO 模型
### 6.2.2 示例对比
## 6.3 巧妙结合
## 6.4 GMP 模型
### 6.4.1 基本概念
### 6.4.2 从 GM 到 GMP
## 6.5 GMP 主要数据结构
![](https://img.github.mailjob.net/book-go-runtime/6.5.mp4)
### 6.5.1 runtime.g
### 6.5.2 runtime.m
### 6.5.3 runtime.p
### 6.5.4 schedt
## 6.6 调度器初始化
![](https://img.github.mailjob.net/book-go-runtime/6.6.mp4)
### 6.6.1 调度器初始化过程
### 6.6.2 runtime.schedinit
## 6.7 G 的创建与退出
![](https://img.github.mailjob.net/book-go-runtime/6.7.mp4)
### 6.7.1 相关汇编函数
### 6.7.2 runtime.newproc
## 6.8 调度循环
## 6.9 抢占式调度

![](https://img.github.mailjob.net/book-go-runtime/6.9.mp4)

### 6.9.1 Go1.13 的抢占式调度

![](https://img.github.mailjob.net/book-go-runtime/6.9.1.mp4)

### 6.9.2 Go1.14 的抢占式调度

![](https://img.github.mailjob.net/book-go-runtime/6.9.2.mp4)

## 6.10 timer
### 6.10.1 一个示例
### 6.10.2 数据结构
### 6.10.3 操作函数
## 6.11 netpoller
### 6.11.1 跨平台的 netpoller
### 6.11.2 TCP 连接的 Read 方法
## 6.12 监控线程
### 6.12.1 保障 timer 顺利执行
### 6.12.2 按需执行 netpoll
### 6.12.3 抢占运行时间过长的 P
### 6.12.4 抢占系统调用中的 P
### 6.12.5 强制执行 GC
## 6.13 本章小结