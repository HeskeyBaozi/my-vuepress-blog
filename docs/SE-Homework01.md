---
title: Software Engineering - HomeWork1
date: 2018-03-15 19:44:02
tags:
- 课程作业
- 系统分析与设计
---

> Software engineering is “(1) the application of a systematic, disciplined, quantifiable approach to the development, operation, and maintenance of software, that is, the application of engineering to software,” and “(2) the study of approaches as in (1).” – IEEE Standard 610.12

<!-- more -->

![焦油坑](./images/SE-homework/jiaoyoukeng.jpg)

## 1、简单题

### 软件工程的定义

软件工程是将系统化的、规范的、可度量的方法应用于软件的开发、运行和维护，即将工程化方法应用于软件。

### 阅读经典名著“人月神话”等资料，解释 software crisis、COCOMO 模型。

`software crisis`，即软件危机。软件危机是指落后的软件生产方式无法满足迅速增长的计算机软件需求，从而导致软件开发与维护过程中出现一系列严重问题的现象。

`COCOMO`，即`constructive cost model`，构造性成本模型。是由巴里·勃姆（Barry Boehm）提出的一种软件成本估算方法。这种模型使用一种基本的回归分析公式，使用从项目历史和现状中的某些特征作为参数来进行计算。

### 软件生命周期

 软件生命周期是指软件的产生直到成熟的全部过程。并且衍生出了软件开发模型，常见的有瀑布模型，即：

1. 需求定义（Requirements）
2. 设计（Design）
3. 实作（Implementation）
4. 整合与测试（Verification）
5. 移交与维护（Maintenance）

### 按照 SWEBok 的 KA 划分，本课程关注哪些 KA 或 知识领域？

1. Software requirements 需求
2. Software design 设计
3. Software construction 构建
4. Software testing 测试
5. Software maintenance 管理
6. Software configuration management 配置管理
7. Software engineering management 工程管理
8. Software engineering process 工程进程
9. Software engineering models and methods 工程模型与方法

### 解释 CMMI 的五个级别。例如：Level 1 - Initial：无序，自发生产模式。

1. Level 1 - initial 无序，自发的生产模式。
2. Level 2 - Managed 有基本管理程序，能完成任务的生产模式。
3. Level 3 - Defined 项目流程制度化，能实现持续生产和模式复制的生产模式。
4. Level 4 - Quantitatively Managed 定量精准管理，能把控产品性能和生产流程的生产模式。
5. Level 5 - Optimizing 优化管理，能持续更新和改善流程的生产模式。

### 用自己语言简述 SWEBok 或 CMMI

`SWEBok`，即`Software Engineering Body of Knowledge`， 是国际标准`ISO / IEC TR 19759：2005`指定的并且普遍接受的软件工程知识体系标准。主要是为我们整理好了软件工程思想上必要的知识架构和知识路线图。

`CMMI`，即`Capability Maturity Model Integration`，即能力成熟度模型集成。是一种用于改进软件开发团队对于一个软件项目的掌握和开发的熟练度的评估和改善用的方法。

## 2、解释 PSP 各项指标及技能要求：

- 阅读《现代软件工程》的 [PSP: Personal Software Process](http://www.cnblogs.com/xinz/archive/2011/11/27/2265425.html) 章节。 

### 按表格 PSP 2.1， 了解一个软件工程师在接到一个任务之后要做什么，需要哪些技能，解释你打算如何统计每项数据？ （期末考核，每人按开发阶段提交这个表）

```txt
Planning（计划）
  Estimate（评估构建成本）

Development（开发）
  Analysis（分析需求）
  Design Spec（设计文档）
  Design Review （设计审核）
  Coding Standard（代码规范）
  Design（设计）
  Coding（编程）
  Code Review（代码审核）
  Test（测试）
```

要求技能：
- 知识：对具体技术的掌握, 动手能力
- 经验：对问题领域的知识和经验的积累 (例如: 对于医疗行业的了解, 对于金融行业的了解)。
- 通用的软件设计思想
- 职业技能包括：自我管理的能力、表达和交流的能力、与人合作的能力、把任务按质按量完成的执行力

如何统计每项数据？

- 分治思想
- 评估统计过程中不断迭代。