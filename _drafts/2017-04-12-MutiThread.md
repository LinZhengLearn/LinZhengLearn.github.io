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

一个线程在给定时间点只可以处于一个状态。 这些状态是虚拟机中的状态，并不反映操作系统中的线程状态。

### New

线程实例化后还没执行start方法时的状态。

### Runnable

线程执行start方法，但线程调度器还没选择它作为running thread。

### **BLOCKED** 

线程在等待monitor 锁而被阻塞的状态。

### **WAITING** 

线程在等待另一个线程执行特定动作时的状态。

### **TIMED_WAITING** 

线程在等待另一个线程执行动作达到指定等待时间时的状态。

### **TERMINATED**

已退出的线程处于此状态。

## 如何创建线程？

创建线程有两种方式：

- 继承Thread类，覆盖run方法，这一方法new出来的线程之间内部属性不共享。
- 实现Runnable接口，重写其run方法，并将Runnable对象传给Thread对象。







## 线程调度