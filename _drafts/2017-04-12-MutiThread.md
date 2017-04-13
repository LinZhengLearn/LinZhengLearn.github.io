---
layout: post
title: Java并发之Thread
categories: [Java, Multithreading]
description: Thread in java
keywords: Java, Multithreading, Thread
---



java中的多线程是同时执行多个线程的过程。

#  介绍

线程基本上是一个轻量级的子进程，是最小的处理单元。



## 线程的生命周期（状态）有哪些？

java 8中`Thread.State`内部枚举类有6种状态。分别如下图：

![](/images/posts/Multithreading/thread-state.png)

### New

线程实例化后还没执行start方法时的状态。

### Runnable

线程执行start方法，但线程调度器还没选择它作为running thread。

### **BLOCKED** 

线程在等待monitor 锁而被阻塞的状态。

### **WAITING** 

### **TIMED_WAITING** 

### **WAITING**



## 如何创建线程？



## 线程调度