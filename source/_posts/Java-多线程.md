---
title: Java-多线程
date: 2019-05-27 11:19:38
tags:
---
# Java多线程编程

## 概念
- 进程：每个进程有自己独立的代码段和数据空间（进程上下文），进程间切换会有较大的开销，每个进程会有1-n个线程，进程是资源分配的最小单位；
- 线程： 同一类线程共享代码段和数据空间，每个线程有独立的运行栈和程序计数器，线程切换开销小（线程是CPU调度的最小单位）
- 线程和进程均可分为五阶段：创建、就绪、运行、阻塞、终止
- 多进程：操作系统可以同时运行多进程（多个任务）
- 多线程：同一个程序可以同时有多个顺序流执行

Java中实现多线程的三种方式：
- 继承Thread类；
- 实现Runable接口；
- 实现Callable接口，并与Future、线程池结合使用

