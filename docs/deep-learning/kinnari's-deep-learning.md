# Kinnari 的个人学习路线

## 课程简介

- **先修要求**：线性代数、概率论，Python，算法，矩阵求导（可以参考[矩阵求导术](https://zhuanlan.zhihu.com/p/24709748)或者[这篇专栏](https://zhuanlan.zhihu.com/p/273729929)）
- **参考材料**：
    - *Neural Networks and Deep Learning*, by Michael Nielsen
    - [动手学深度学习](https://zh-v2.d2l.ai/)，作者：李沐等
    - 众多博客和 Pytorch 官方教程
    - [GPT 是什么？直观解释 Transformer | 深度学习第 5 章](https://www.bilibili.com/video/BV13z421U7cs?vd_source=c9e11661823ca4062db1ef99f7e0eee1)和[直观解释注意力机制，Transformer 的核心 | 深度学习第 6 章](https://www.bilibili.com/video/BV1TZ421j7Ke?vd_source=c9e11661823ca4062db1ef99f7e0eee1)，创作者 3Blue1Brown
- **主要内容**：
    - 多层感知机（MLP），反向传播算法（BP）
    - 卷积神经网络（CNN）
    - 循环神经网络（RNN），门控记忆单元（GRU），长短期递归神经网络（LSTM），注意力机制（Attention），Transformer，语言模型（language model）

## 个人心得

我首先使用 *Neural Networks and Deep Learning* 进行了深度学习的入门。这门课最大的优点就是通俗易懂、循序渐进。从感知机到一个简单的全连接层，再到一个不超过 5 行的多层感知机，让它去识别数字，竟然能够达到 90% 以上的准确度。在这个最简单的神经网络的基础上，Michael 又一个接一个地讲述改进它的若干方法，你会不知不觉中发现，这一切都是那么的自然且连贯——把元素计算转化为矩阵计算、损失函数的改进、regularition、超参数的选择……你会一次又一次的发现，识别数字的准确率越来越高，95%，96.4%，97.3%，一切似乎都那么鼓舞人心。最后一章引入卷积神经网络，再告诉你其实全部使用全连接层也有局限，而一些巧妙的结构可以进一步改进识别的准确率！从始至终，我们所做的不过只是一件事情——识别数字——但是，我们竟然走过了一个神经网络的完整搭建过程！！！另外，这门课还非常生动形象地向你展示了多层感知机中的反向传播算法是如何得来的、为什么神经网络可以拟合任意函数、为什么神经网络难以训练，以及在附录中讨论的是否有更简单的“智能”。这些内容同样让我受益匪浅。

接着，我使用 Pytorch 官网上的几篇教程以及其它的一些博客，学习了 Pytorch 的使用方法和 RNN、GRU、LSTM、Attention、Transformer、language model 等内容，顺序如下：

1. Pytorch 入门教程：[Deep Learning with PyTorch: A 60 Minute Blitz](https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html)。在后续的学习中，可以参考更详细的教程 [Learn Pytorch](https://www.learnpytorch.io/)。
2. RNN、GRU、LSTM 教程：
    1. [Written Memories: Understanding, Deriving and Extending the LSTM](https://r2rt.com/written-memories-understanding-deriving-and-extending-the-lstm.html)，这个教程是我看到过的关于 LSTM 的写得最好的教程，作者以人类阅读、翻译的例子作为类比，形象地展示出 LSTM 产生过程中的每一个动机——先从 RNN 入手，紧接着分析其缺陷，提出生活中的例子，从而进一步开发出 LSTM 的原型机；再指出原型机在实际中的表现，并分析其原因，在弥补缺陷的同时自然的引申出三种解决方案，其中就包括了 GRU 和 pseudo LSTM；最后将 pseudo LSTM 与原始的 LSTM 进行比较，并指出原始 LSTM 的缺陷与优点，接着提出一个能够利用原始 LSTM 优点的变体 "The LSTM with peepholes"。在博客的最后，作者还介绍了 LSTM 的基本思想在 residual network、highway network 以及 Neural Turing Machine 中的应用，作为对 LSTM 的扩展延伸。
    2. [Understanding LSTM Networks](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)，[现代神经循环网络（d2l）](https://zh-v2.d2l.ai/chapter_recurrent-modern/index.html)：包含一些结构的可视化以及代码实现，具体分析上并不如第一篇教程，不过可以加深印象。
    3. [LONG SHORT-TERM MEMORY](https://www.bioinf.jku.at/publications/older/2604.pdf)：LSTM 的原始论文，有兴趣的话可以看看
    4. [NLP From Scratch: Classifying Names with a Character-Level RNN](https://pytorch.org/tutorials/intermediate/char_rnn_classification_tutorial.html)，[NLP From Scratch: Generating Names with a Character-Level RNN](https://pytorch.org/tutorials/intermediate/char_rnn_generation_tutorial.html)：学习使用 Pytorch 写代码，了解基本框架。如果你需要有关 tensorflow 的代码教程的话，可以看看上面 2.a 中教程的作者笔下三篇有关 tensorflow 实现的博客。
3. Attention 教程：
    1. [Attention? Attention!](https://lilianweng.github.io/posts/2018-06-24-attention/)：一篇讲述 Attention 的博客，后半段介绍了 Transformer
    2. [Visualizing A Neural Machine Translation Model (Mechanics of Seq2seq Models With Attention)](https://jalammar.github.io/visualizing-neural-machine-translation-mechanics-of-seq2seq-models-with-attention/)：可视化地展示在 Neural Machine Translation 中 Attention 的使用，直观且形象。
    3. [d2l - 注意力机制](https://zh-v2.d2l.ai/chapter_attention-mechanisms/index.html)：动手学深度学习中关于注意力机制的讲解，可结合其代码进行实践
    4. [Illustrated: Self-Attention](https://colab.research.google.com/drive/1rPk3ohrmVclqhH7uQ7qys4oznDdAhpzF)：动图演示 self-attention，直观形象
    5. [NLP From Scratch: Translation with a Sequence to Sequence Network and Attention](https://pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html)：学习使用 Pytorch 写 Attention 机制。
4. Transformer 教程：
    1. [GPT 是什么？直观解释 Transformer | 深度学习第 5 章](https://www.bilibili.com/video/BV13z421U7cs?vd_source=c9e11661823ca4062db1ef99f7e0eee1)和[直观解释注意力机制，Transformer 的核心 | 深度学习第 6 章](https://www.bilibili.com/video/BV1TZ421j7Ke?vd_source=c9e11661823ca4062db1ef99f7e0eee1)：3Blue1Brown 的直观理解 GPT 视频，<del>使我注意力集中</del>。由于整个系列的视频还没有全部公布，我只放这两个链接在这里，后续续集请自行搜索。
    2. [How Transformers Work](https://towardsdatascience.com/transformers-141e32e69591)：在这篇博客的前半部分 RNN、LSTM 等框架进行了回顾，在后半部分介绍了 Transformer 的工作原理。另外，这篇博客引用了大量其它博客的内容，推荐都看一看。其中 [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) 这篇博客和 3.d 中的博客是同一个作者写的，都关于可视化，直观且易于理解。
    3. [Transformer 论文逐段精读](https://www.bilibili.com/video/BV1pu411o7BE?vd_source=c9e11661823ca4062db1ef99f7e0eee1)：李沐带你阅读一遍大名鼎鼎的 *Attention Is All You Need* 这篇论文，相信听完后你对 transformer 会更加熟悉。沐神专门有一系列视频带领阅读著名论文，感兴趣的话可以都看看。
    4. [Tutorial 6: Transformers and Multi-Head Attention](https://uvadlc-notebooks.readthedocs.io/en/latest/tutorial_notebooks/tutorial6/Transformers_and_MHAttention.html)：一篇结合了代码讲解 Transformer 的博客。
    5. [Build your own Transformer from scratch using Pytorch](https://towardsdatascience.com/build-your-own-transformer-from-scratch-using-pytorch-84c850470dcb)：带你从 0 开始构建一个 Transformer，和上一篇博客一样，很值得跟着写写代码。
    6. [A Mathematical Framework for Transformer Circuits](https://transformer-circuits.pub/2021/framework/index.html)：详细讲解了 Transformer 的数学框架。
    7. [The Transformer Family Version 2.0](https://lilianweng.github.io/posts/2023-01-27-the-transformer-family-v2/)：详细介绍了一些 Transformer 的改进与变体，适合用于扩展进阶。
5. Language model 教程：
    1. [A Comprehensive Guide to Build your own Language Model in Python!](https://medium.com/analytics-vidhya/a-comprehensive-guide-to-build-your-own-language-model-in-python-5141b3917d6d)：一篇详尽的 language model 教程。
    2. [Language Modeling with LSTMs in PyTorch](https://towardsdatascience.com/language-modeling-with-lstms-in-pytorch-381a26badcbf): 补充读物。
    3. [Word-level Language Modeling using RNN and Transformer](https://github.com/pytorch/examples/tree/main/word_language_model)：PyTorch 官方代码示例，可以作为参考来写一写。

在阅读这些教程的同时，我推荐同时阅读[《动手学深度学习》](./dive-into-deep-learning.md)这本书。因为上面列出的博客大多偏向理论，代码示例较少；而这本书更加注重代码实践，理论部分反而不是很详细。它们两个结合之后效果就比较不错了。

最后，由于我的这份课程具有非常强的个人性质，而且 CV 方向涉及内容较少（不过在计算机视觉部分中会有很详尽的讲解），而 NLP 方向内容较多，所以你可能更需要其它的一些更系统的课程，例如 [CS230](./CS230.md)，[李宏毅机器学习](./李宏毅机器学习.md)等。

## 相关链接

1. [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/)：一个简单易懂的深度学习教程，围绕着数字识别这一深度学习中的经典问题，带领你学会多层感知机、反向传播算法、卷积神经网络。
    1. <https://github.com/mnielsen/neural-networks-and-deep-learning>：作业和问题的代码实现，使用 Python2
    2. <https://github.com/MichalDanielDobrzanski/DeepLearningPython>：由于 Python2 已经过时，因此有人使用 Python3 实现了 2 中的代码。尽管如此，它使用的 Theano 库如今看来也显得过时了。
2. [《动手学深度学习》](./dive-into-deep-learning.md)：李沐大神出书，结合了深度学习理论与代码，不过侧重于代码实践。它的一个优点是书中的所有代码都可运行，正如书名所说，适合上手练习。不过个人认为不太适合小白学习，结合上述列出的博客一起学习效果更佳。

## 鸣谢

以上教程/博客中大多来源于我的师兄们[@cpdu](https://github.com/cpdu)[@cantabile-kwok](https://github.com/cantabile-kwok)[@JamesZhutheThird](https://github.com/JamesZhutheThird)，感谢师兄们对我的无私帮助！🙏🙏🙏
