# My aiTour

截至目前，这是我个人的 AI 学习路线，顺序为由上到下，连线为对应的部分先修关系，为美观起见，去除了一些先修关系的连线：

```mermaid
graph TD
    aiTour(aiTour)
    A(C++)
    B(Python)
    C1(数学分析Ⅰ)
    C2(数学分析Ⅱ)
    D1(线性代数)
    D2(高等代数)
    D3(矩阵论)
    E(离散数学)
    F(计算机系统基础)
    G(数据结构与算法)
    H1(概率论)
    H2(随机过程)
    I1(机器学习基础)
    J1(深度学习基础)
    J2(计算机视觉)
    J3(自然语言处理)
    K(凸优化)

    aiTour---D1
    aiTour---C1
    aiTour---E
    aiTour---B
    aiTour---A
    A---G
    B---I1
    C2---K
    C1---C2
    C1---H1
    D1---D3
    D1-.-D2
    D1---C2
    D2-.-D3
    D1---H1
    E---H1
    E---G
    G---I1
    G---F
    H1---H2
    H1---I1
    I1---J1
    J1---J2
    J1---J3
```

如果想要获取课程的简短介绍的话，可以参考[课程总览](./overview/course-overview.md)。

这份学习路线仅仅只是一个抛砖引玉——每个人都应该有自己独特的学习路线，而不是一味地照搬别人的。这里提供一个思路，以构建你自己的学习路线：

!!! note "aiTour 生成算法"
    1. 前往斯坦福大学的官网，搜索人工智能相关课程，这里以吴恩达教授的 [CS229](https://cs229.stanford.edu/) 为例；
    2. 进入对应课程的网址，查看课程介绍中的 [Prerequisites](https://docs.google.com/document/d/1P2s6xxcAT9VRwnEHApB3NHnIpcR8WWvyswHh3xDH_0E/edit#heading=h.u0en5qo62ffo)，就能得知修该门课所需要的先修课程（这里为 CS106A or CS106B, CS106X; CS 109, MATH151, or STATS 116; Math 51），并记录得到的先修关系；
    3. 对查询到的所有先修课程反复进行第2步，除非某个课程没有先修课程。

通过上述过程，就可以构建起一个斯坦福版本的学习路线了。当然，不一定必须学习相应的斯坦福课程，完全可以在网上查找推荐的替代课程。

或者，你也可以参考 [UCB](https://hkn.eecs.berkeley.edu/courseguides) 的课程地图。再或者，你也可以将上述思路运用到 [csdiy](https://csdiy.wiki) 中。

在确定好学习路线后，接着需要确定学习每门课程所用的资料。这个步骤只能按照你的个人喜好来实施。一般来说，所需的资料在网上应该是数不胜数的，你可以在各大网站平台上找到，例如 B 站、YouTube、GitHub、各大学的官方课程网站等。挑选时可以注意对应的先修要求、课程资料是否齐全（如课堂视频、notes、作业及解答、考试等）、哪个版本风评最好，以及是否有前人的踩坑经验等等。请按需挑选最符合你胃口的资料和课程。

如果你所寻找的课程不再开放，可以使用 [Web Archive](https://web.archive.org/) 来寻找是否有网页存档可以使用。
