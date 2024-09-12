# 序

## 关于这本书

> 2024年1月11日 19 点 18 分，那时的我创建了这本书。

2023 年可以说是人工智能爆火元年。从 ChatGPT 发布，到各地媒体广泛报道，世界各国 AI 公司奋起直追，众多国家将 AI 纳入国家重要战略，新的 AI 模型如雨后春笋般不断涌出。机器学习、深度学习、神经网络等专业词汇也似乎有渐渐走入公众的视野。

但是，究竟什么是 AI ？现有的 AI 真的如媒体报道所言那般“强大”了吗？现有的 AI 相关的技术背后又是什么原理在支撑？……怀着这些疑问，我报考了人工智能专业，以期在未来将这些问题一一解决，踏上了我的 AI 学习之旅。

可是我多希望这样美好的、怀揣着希望的出发，能够拥有一个明媚的旅途、一个至少令我满意的结局啊。现实一次又一次地无情地告诉我，我的愿望几乎不可能实现——老旧的教材、不合理的培养方案、一言难尽的授课质量、各式各样的杂乱活动，一个接一个的消磨我的内心，接着又遇到了一系列学院之间本不该发生的糟心事……

我无意对这些发表更多的评论，只是每每都会想起上海交通大学生存手册中[欢迎来到上海交通大学](https://survivesjtu.gitbook.io/survivesjtumanual/li-zhi-pian/huan-ying-lai-dao-shang-hai-jiao-tong-da-xue)一节的内容，如芒在背。

> 我只是看到了无数充满求知欲、激情、与年轻梦想的同学们，将要把自己的四年青春，充满希望与信任地交给大学来塑造。这使我心中非常不安。

所幸我在刚入学时能遇到 [csdiy](https://csdiy.wiki) 这个宝藏网站，开始按照上面的课程介绍开始了我的自学生活。我感激所有无私做出分享的学长学姐，因为我无法想象，如果没有他们，接下来的本科四年，我将会在什么样的生活中度过。

时间流逝得飞快，转眼就到了一学期结束，按照学校的要求，学生需要写下自己一学期的回顾与总结。在这个时候，我突然有了一个大胆的想法——为什么不把自己的学习过程记录下来做成一个 AI 相关的学习分享网站，像 csdiy 一样呢？我又搜索了国内是否有类似目标的网站，结果并未发现（不过现在发现了一些）。这更加激发了我建立一个 AI 相关的学习分享网站的念头。另一方面，在阅读 csdiy 时，我也感受到了一些小小的问题：

- 目前无法仅靠 csdiy 构建出一个与 AI 相关成体系的课程网络，一些更深层次的 AI 课程、一些 AI 额外需要学习的数学课程、一些 AI 相关的工具还没有收录。我将在这个网站中进行补齐。
- csdiy 的作者并没有给出一个明确带有先修关系的 roadmap，这使我无法很快地安排出一条长期的学习路线，例如自学课程的先后关系，怎样安排能够顾及到大学本有的课程安排。因此我决定在我将建立的网站中添加一个 roadmap，不过由于每个人的情况不同，我没法给出一个适合所有人的学习路线，仅仅也只供参考。
- csdiy 中推荐了很多高质量的网课，但是并没有涉及到书籍的推荐。我认为阅读经典书籍同样是学习的重要环节，所以我也添加了书籍推荐，与课程推荐并行。

于是当天下午我就基于 [materials for mkdocs](https://squidfunk.github.io/mkdocs-material/) 搭建起了这个学习网站，记录下我学习过程中所用到过的一些资料和心得体会，并整理出一条 AI 方向的学习路线，希望能给他人带去哪怕一点点帮助、哪怕一点点微不足道的启发。

我会如实地记录下自己在人工智能的学习过程中所使用过的书籍、参考过的资料，以及自己的一些小小的学习体会（大多是自己思考过后得出的结论），当然，也正因为大多数观点都是我个人的，避免不了与他人的观点相冲突，所以如果我的一些观点与你的相左的话，希望能够得到你的谅解，更希望你能提出宝贵的建议！

尽管我会提供一份可能的学习路线，但是我更提倡每个人都构建自己的学习路线，毕竟 "It's best only when it fits you"。

特别地，我希望这本书能够给我 SJTU 的学弟学妹们带来一些帮助，算是我送给他们的一份小礼物吧。

### 这本书是/不是什么

这本书是我的人工智能学习旅途上的记录，是我对一些精彩课程的分享，是我推荐使用的工具介绍。

这本书不是详细的工具教程，更不是详细的课业辅导。

### 这本书适合哪些人

如果你和我一样，也是人工智能专业或计算机科学与技术专业的本科学生，那么这本书应该非常适合你来读；如果你已经是研究生，那么这本书的后半部分内容（目前暂未写到）或许值得你看看；如果你已经工作，那么你或许可以从这本书中找到一些你所需要的内容。总而言之，由于本书的编排顺序，本书应该最适合那些立志于学习人工智能的学生，尤其是本科大一的学生。

### TODO-List

??? "TODO list"
    - 优化理论
    - 语音处理
    - 强化学习

## 建立交流群

本书支持讨论功能，请在页面末尾的讨论区进行讨论，也可以选择自行组建群交流群。如果你想与作者联系，欢迎向作者[发送邮件](mailto:jy_zhou@sjtu.edu.cn)！

## 贡献者请看这里

我非常欢迎任何人做出贡献。更详细的说明，请参考仓库的 [README 文件](https://github.com/KinnariyaMamaTanha/aiTour)。感谢您的贡献！

## 特别鸣谢

在此特别感谢 csdiy 的作者（[@PKUFlyingPig](https://github.com/PKUFlyingPig)）以及贡献者们，是 csdiy 这本书让我真正意识到自学的巨大威力，也是它让我产生了写下自己的一本书的想法，并提供了我无穷的动力。推荐所有学习计算机的人都去阅读 csdiy 这本书！

我也要向所有学习资料和课程的创建者，向所有无私公开课程资源的教授们献上我最崇高的敬意！是他们的辛勤的付出和无私的品格，才让我们所有学生能够方便快捷地接触到世界上数不胜数优秀学习资源。再次感谢！

## 请作者喝杯奶茶

这本书完全开源，如果你觉得我写得还行，或者这本书真真正正地帮助到了你，不妨为这个仓库点一个 star 或者请作者喝杯奶茶。

<figure markdown>
  ![Image title](./images/payment.png){ width="400" }
</figure>