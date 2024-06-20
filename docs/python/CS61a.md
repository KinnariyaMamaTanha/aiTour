# CS61a: Structure and Interpretation of Computer Programs

## 课程简介

- **先修要求**：无（但最好有另一种编程语言的基础，推荐 C 或 C++）
- **参考材料**：
    - CS61a 课程
    - 《python 基础教程》，作者：[挪] Magnus Lie Hetland
    - 《流畅的 Python》，作者：Luciano Ramalho
- **主要内容**：与 C++ 中基本相同，只是没有指针，STL等内容

## 个人心得

首先，我不建议新手使用 Python 作为编程的入门语言，其原因如下：

1. Python 不够底层。Python 中没有指针的具体体现，学 Python 时可能会对 Python 中的引用、变量内存分配等没有深刻的认识；
2. Python 偏简单。
    1. Python 中的大部分函数及方法是直接提供的，但是实际上完全可以把这些函数及方法作为 C 或 C++ 的编程练习来实现；
    2. Python 中对类的继承的处理相当简单，一个 `super()` 函数就能解决一切，不利于对继承背后的原理的理解；
    3. 学完 C 或 C++，可以很快掌握 Python，但反之不然。

因此，建议先学习 C 或 C++ 之后，再来学习 Python，那时，你就可以很快的掌握 Python 语言，并且理解 Python 每个函数或方法背后的原理。（另外，Python 是基于 C 语言构建的；在机器学习中，有时会使用 C++ 编写代码，Python 提供接口来提高运行速度）

当然，以上也仅仅是我个人的理解，如果和你的理解不同，请忽视以上内容。事实上，不管从哪门语言入门，最终都是殊途同归的。

对于喜欢看网课的同学，强烈推荐伯克利大学的 CS61a 课程。这门课的教材是计算机圣经 [SICP](https://mitp-content-server.mit.edu/books/content/sectbyfn/books_pres_0/6515/sicp.zip/index.html) 的 Python 版本，较有难度（不建议小白贸然上手）。其令人眼花缭乱的 homework 和 project 质量极高，可以有效的锻炼代码能力，也能让你在上千行的 project 中获得完成项目的快感（project 的内容也相当有趣，在此不作剧透）。看完 CS61a，我只能说，国内的本科教育，实在是任重而道远。

另外，CS61a 中也会教授 Scheme 和 SQL 两门语言的基础部分，并且讲授了多种编程思维（我认为这实际上才是这门课的精华），对于提高对程序的理解有很大的帮助。

最后，强烈感谢 csdiy 的作者，没有他，我是无法遇见 CS61a 这样优秀的一门网课，这也是我[梦开始的地方](https://csdiy.wiki/#cs61a)。

## 相关链接

1. 课程网站：[2020 summer](https://inst.eecs.berkeley.edu/~cs61a/su20/)
2. [csdiy](https://csdiy.wiki/#cs61a)：梦开始的地方。
3. [Python Tutor](https://pythontutor.com/)：一个可以将Python代码可视化的网站。
4. [COMPOSING PROGRAMS](https://composingprograms.netlify.app/)：教材的中译版。
5. [The Python Standard Library](https://docs.python.org/3/library/)：Python的官方文档，具有一定Python基础后可以查阅。
