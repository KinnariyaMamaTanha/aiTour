# aiTour

[![License](https://img.shields.io/github/license/KinnariyaMamaTanha/aiTour)](https://github.com/KinnariyaMamaTanha/aiTour/blob/main/LICENSE)
[![Issues](https://img.shields.io/github/issues/KinnariyaMamaTanha/aiTour)](https://github.com/KinnariyaMamaTanha/aiTour/issues)
[![Stars](https://img.shields.io/github/stars/KinnariyaMamaTanha/aiTour)](https://github.com/KinnariyaMamaTanha/aiTour)

2022年7月12日，MidJourney research lab 发布 Midjourney。

2022年11月30日，OpenAI 发布 ChatGPT。

2023年12月6日，Google 发布 Gemini。

2024年5月14日，OpenAI 发布 GPT-4o……

~~2024年10月8日，诺贝尔物理学奖颁发给 John J. Hopfield 和 Geoffrey E. Hinton，以表彰他们在人工神经网络方面作出的贡献。2024年10月9日，诺贝尔化学奖颁发给 David Baker 和 AlphaFold 开发者 Demis Hassabis、John M. Jumper~~

2025年1月20日，幻方旗下公司深度求索发布世界首个完全开源的推理模型 DeepSeek-R1，被称为当时最为先进的大语言推理模型。

2023 年可以说是人工智能爆火元年。从 ChatGPT 发布，到各地媒体广泛报道，世界各国 AI 公司奋起直追，众多国家将 AI 纳入国家重要战略，新的 AI 模型如雨后春笋般不断涌出。机器学习、深度学习、神经网络等专业词汇也似乎有渐渐走入公众的视野。

但是，究竟什么是 AI ？现有的 AI 真的如媒体报道所言那般“强大”了吗？现有的 AI 相关的技术背后又是什么原理在支撑？……怀着这些疑问，我报考了人工智能专业，以期在未来将这些问题一一解决，踏上了我的 AI 学习之旅。

可是我多希望这样美好的、怀揣着希望的出发，能够拥有一个明媚的旅途、一个至少令我满意的结局啊。现实一次又一次地无情地告诉我，我的愿望几乎不可能实现——老旧的教材、不合理的培养方案、一言难尽的授课质量、各式各样的杂乱活动，一个接一个的消磨我的内心，更别提学院之间一些本不该发生的糟心事……我无意对这些发表更多的评论，只是每每都会想起上海交通大学生存手册中[欢迎来到上海交通大学](https://survivesjtu.gitbook.io/survivesjtumanual/li-zhi-pian/huan-ying-lai-dao-shang-hai-jiao-tong-da-xue)一节的内容，如芒在背。

> 我只是看到了无数充满求知欲、激情、与年轻梦想的同学们，将要把自己的四年青春，充满希望与信任地交给大学来塑造。这使我心中非常不安。

所幸我能在刚入学的时候就遇到 [csdiy](https://csdiy.wiki) 这个宝藏网站，开始按照上面的课程介绍开始了我的自学生活。我感激所有无私做出分享的学长学姐，因为我无法想象，如果没有他们，接下来的本科四年，我将会在什么样的生活中度过。

时间流逝得飞快，转眼就到了一学期结束，按照学校的要求，学生需要写下自己一学期的回顾与总结。在这个时候，我突然有了一个大胆的想法——为什么不把自己的学习过程记录下来，做成一个 AI 相关的学习分享网站，像 csdiy 一样呢？我又搜索了国内是否有这样的网站，结果并未发现（不过现在发现了一些）。这更加激发了我建立一个学习分享网站的念头。另一方面，在阅读 csdiy 时，我也感受到了一些小小的问题：

- 目前无法仅靠 csdiy 构建出一个与 AI 相关成体系的课程网络，一些更深层次的 AI 课程、一些 AI 额外需要学习的数学课程还没有收录；并且，这些课程又几乎只有 AI 方向将会用到，单独划分到 AI 学习路线中会更为合理。我将在这个网站中进行补齐。
- csdiy 的作者并没有给出一个明确带有先修关系的 roadmap，这使我无法很快地安排出一条长期的学习路线，例如自学课程的先后关系，怎样安排能够顾及到大学本有的课程安排等等。因此我决定在我将建立的网站中添加一个 roadmap，不过由于每个人的情况不同，我没法给出一个适合所有人的学习路线，仅仅也只供参考。

于是当天下午我就基于 [materials for mkdocs](https://squidfunk.github.io/mkdocs-material/) 搭建起了这个学习网站，记录下我学习过程中所用到过的资料和心得体会，并整理出一条 AI 方向的学习路线，希望能给他人带去哪怕一点点帮助。我会竭尽我所能：

1. 寻找优质书籍、网课等资料并进行汇总；
2. 安排出一条尽可能合理的 AI 学习路线规划；
3. 在具体的课程中提供自己的尽可能多的有价值的心得体会。

对于前两点，我有信心做到令大多数人满意；对于最后一点，我所提供的心得也许并不适合每一个人，这是一件仁者见仁的事情，我会做到我能力范围内的最好。

如果能帮助到你，将会是我的万分荣幸。

## Contributing

我非常欢迎任何人做出贡献，接收不限于如下的几种贡献内容：

1. 对已有课程的补充，可以是心得体会、资料推荐等等。
2. 新的课程推荐。提交这种贡献时，请注意标注好与我的学习路线的先修关系，然后记得加入学习路线图（尽可能保持美观）。
3. 对于实用工具的补充。我也欢迎有关工具使用/学习教程的贡献，因为根据经验，这往往能给第一次使用这些工具的同学以极大的便利。

在提交贡献时，请尽可能做到以下几点：

1. 文件（夹）命名规范。文件夹名请使用英文小写，并用 `-` 进行单词的划分（例如 `linear-algebra`、`deep-learning`）；文件名使用课号（如果是课程推荐的话，如 `CS229`），或者书名的方式（如果是书籍推荐的话，如 `Introduction-to-Linear-Algebra`），或者工具英文名（如 `Docker`）
2. 排版规范。对于新增课程、书籍或原有课程、书籍的修改补充，请根据仓库中 template 文件夹下的格式进行排版。对于工具的增添，虽然没有具体的排版限制，但是请尽可能的优雅。
3. 中英文混合排版参考[这个仓库](https://github.com/sparanoid/chinese-copywriting-guidelines/tree/master)。专有名词的英文参照其原始写法（例如，是 `LaTeX` 而不是 `latex`）。英文书名请使用 *italics*。
4. 先修/后续关系。如果是新增课程/书籍的话，请务必将其添加进学习路线图中与根目录下的 `mkdocs.yml` 文件导航设置中；如果你对这个步骤不太明白的话，也可以在 issue 中提出。我将进行一定的校对后帮助你发布到网站上。
5. 为了保证界面风格一致性，一级标题请按照下述格式：
   1. 如果是课程推荐，使用 `所属大学 课程号: 课程名` 的方式（如 `Stanford CS229: Machine Learning`）
   2. 如果是书籍推荐，中文书名使用 `《书名》` 的方式（如 《概率导论》），英文书名使用 `斜体书名`（如 *Linear Algebra Done Right*）
   3. 如果是工具推荐，使用 `工具名` 的方式（如 `LaTeX`）
6. 如果在其它网站上有相关的课程介绍的话，可以在末尾进行补充。

另外，可以按照如下方式配置环境：

```bash
# fork aiTour to your repos
# remember to change user name
git clone https://github.com/KinnariyaMamaTanha/aiTour/

# install conda before this step
conda create -n aiTour python=3.10 -y
conda activate aiTour

# cd into the dir before this step
pip install -r requirements.txt

# begin serving
mkdocs serve

#### or you can use uv to get locked dependencies
# install uv first
curl -LsSf https://astral.sh/uv/install.sh | sh
# or pip install uv

# set up the environment
uv sync
```

## Issues

如果你发现本书的错误或者有改进意见，请尽情地提出 issue！我会尽可能快地修改（ddl 期间除外）。或者你也可以[向我发送邮件](mailto:jy_zhou@sjtu.edu.cn)！

## Discussions

本书已支持讨论功能，请在讨论区进行讨论，笔者创建了一个 QQ 交流群：793679786，你也可以自行成立 QQ / 微信等群聊进行交流。

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=KinnariyaMamaTanha/aiTour&type=Timeline)](https://star-history.com/#KinnariyaMamaTanha/aiTour&Timeline)

## License

项目贡献者编写的部分依照 [MIT LICENSE](https://www.tawesoft.co.uk/kb/article/mit-license-faq)。

其余部分（包括但不限于书中提到的课程资源、开源书籍以及视频内容）遵循原作者规定的许可。
