# C++

## 课程简介

- **先修要求**：无（但最好先了解一些计算机基础内容）
- **参考材料**：
    - *C++ Primer Plus*，作者：Stephen Prata.
- **主要内容**：
    - 编程基础
    - C++数据类型
    - C++基础语法
    - C++函数
    - 指针与引用
    - 面向对象编程（类，类模板，友元，继承，函数重载）
    - 异常
    - 文件输入输出
    - 部分STL

## 个人心得

虽然大多数学校会以 C 语言作为讲授的第一门语言，但是我仍然选择了使用 C++ 作为编程的入门语言，主要原因是 C++ 支持 OOP，并且同 C 一样也支持指针。C++的知识浩如烟海，经过大一上的学习，我也仅仅只是窥得冰山一角而已，但其严谨而又细致的语法仍然给我留下了很深的印象。

我使用的教材是* C++ Primer Plus*，尽管网上对其争议颇多，但我仍然觉得使用这本书非常有帮助。该书细致入微，基本涵盖了 C++ 编程的方方面面（但有时会显得过于啰嗦），适合新手阅读或作为字典书使用。

在我看来，学习 C++ 最重要的是理解模块化开发的基本思想（封装、接口）、指针及引用，以及大致了解程序运行的过程和内存分配。新手往往会写出一长串包含在main函数中的代码，不仅难以阅读，而且不易移植到其它代码中。此时模块化开发就显得格外重要：将一种固定的程式抽象为一个函数或者一个类，将过程封装，并只提供接口来使用。既然模块化，那么就必然会涉及到变量的作用域和内存分配等内容，进而引出指针和引用以及变量的动态内存分配。按照这个思路，可以梳理出程序运行的基本框架。

此外，适当的练习也是必不可少的。对于新手，推荐使用[洛谷](https://www.luogu.com.cn/)中的入门题单进行练习；对于已经具有一定编程基础的同学，更推荐通过学习数据结构与算法分析来巩固代码能力，这样既能学习后续知识，又能提高自己的代码能力。**不推荐**新手使用[Leetcode](https://leetcode.cn/)刷题，因为涉及到了一些基础的面向对象编程，并且多数题目的题解使用 STL，题目难度对新手也不友好。等到具有一定的代码基础后，可以考虑在 Leetcode 上刷题。

鉴于上述刷题网站均没有较好的 OOP 训练，可以尝试自己编写一些类并保存为头文件，也便于日后使用。常见的可作为练习的类有：有理数类、复数类、向量类、矩阵类、链表类、栈类、队列类。或者直接学习[数据结构](../da-yi-han-jia/data-structure.md)，实现常用的数据结构类，搭建属于自己的 STL 库！

如果想对代码运行中的变量内存分配及作用域有一个图形化的展示，可以使用 [Python Tutor](https://pythontutor.com/) 网站进行可视化。

## 相关链接

1. [洛谷](https://www.luogu.com.cn/)：一个OI向的刷题网站。
2. [Leetcode](https://leetcode.cn/)：一个offer向的刷题网站。
3. [Python Tutor](https://pythontutor.com/):一个可以将 C++，Java，Python 等语言的代码可视化的网站。
