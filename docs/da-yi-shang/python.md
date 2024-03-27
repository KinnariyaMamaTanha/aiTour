# Python

## 课程简介

- **先修要求**：无（但最好有另一种编程语言的基础，推荐C或[C++](./c++.md)）
- **参考材料**：
  - 《python基础教程》，作者：[挪] Magnus Lie Hetland
  - 《流畅的Python》，作者：Luciano Ramalho
  - [cs61a](https://inst.eecs.berkeley.edu/~cs61a/su20/)，伯克利神级网课
- **主要内容**：与[C++](./c++.md)中基本相同，只是没有指针，STL等内容

## 个人心得

首先，我不建议新手使用Python作为编程的入门语言，其原因如下：

1. Python**不够底层**。Python中没有指针的概念，学Python时可能会对Python中的引用、变量内存分配等没有深刻的认识；
2. Python**过于简单**。
    1. Python中的大部分函数及方法是直接提供的，但是实际上完全可以把这些函数及方法作为C或C++的编程练习来实现；
    2. Python中对类的继承的处理相当简单，一个`super()`函数就能解决一切，不利于对继承背后的原理的理解；
3. 学完C或C++，可以很快掌握Python，但反之不然。

因此，建议先学习C或C++之后，再来学习Python，那时，你就可以很快的掌握Python语言，并且理解Python每个函数或方法背后的原理。（另外，Python是基于C语言构建的；在机器学习中，有时会使用C++编写代码，Python提供接口来提高运行速度）

对于喜爱看书的同学，可以阅读《Python基础教程》来入门Python。此后，如果想要精通Python的话，可以继续阅读《流畅的Python》；如果想多积累代码实践的话，可以继续阅读*Python Cookbook*，此书有大量代码示例以供学习。但是请注意，书上往往会介绍Python的多个应用方向，建议不要全部看完，等到需要时再回来阅读效率更高。

对于喜欢看网课的同学，**强烈推荐**伯克利大学的cs61a课程。这门课的教材是计算机圣经SICP的Python版本，较有难度（不建议小白贸然上手）。其令人眼花缭乱的homework和project质量极高，可以有效的锻炼代码能力，也能让你在上千行的project中获得完成项目的快感（project的内容也相当有趣，在此不作剧透）。看完cs61a，我只能说，国内的本科教育，实在是任重而道远。

另外，cs61a中也会教授Scheme和SQL两门语言的基础部分，并且讲授了多种编程思维（这实际上才是这门课的精华），对于提高对程序的理解有很大的帮助。

最后，强烈感谢csdiy的作者，没有他，我是无法遇见cs61a这样优秀的一门网课，这也是我梦开始的地方。（详细可见[csdiy-梦开始的地方](https://csdiy.wiki/#cs61a)）

## 相关链接

1. [cs61a 2020summer](https://inst.eecs.berkeley.edu/~cs61a/su20/)：这是伯克利大学的cs61a课程2020夏季版官方网站。（当然也有许多不同年份的版本，请自行斟酌选择）
2. [csdiy](https://csdiy.wiki/#cs61a)：梦开始的地方。
3. [Python Tutor](https://pythontutor.com/)：一个可以将Python代码可视化的网站。
4. [COMPOSING PROGRAMS](https://composingprograms.netlify.app/)：教材的中译版。
5. [The Python Standard Library](https://docs.python.org/3/library/)：Python的官方文档，具有一定Python基础后可以查阅。
