# Anaconda

在学习中，不同的任务往往会要求不同的 Python 环境，比如某个项目可能只能在 Python3.10 以上运行，另一个项目又会要求 Python 版本必须为 3.9，并且还要求 CUDA 版本为 12.1，Pytorch 版本为 2.1.2 等等等等。这时为了避免繁琐的环境配置以及解决多版本 Python 共存的问题，可以使用 Anaconda 来管理不同的 Python 环境。

Anaconda 是一种用于科学计算的 Python 发行版，官网网址为 <https://www.anaconda.com/>，支持Linux、MacOS，以及 Windows 系统。Anaconda 使用预装好的 conda 软件进行 Python 包和环境的管理，在其自带的 base 环境中，已经预装好一系列 Python 工具。如果对电脑空间有较高要求，可以选择安装 Miniconda，它只包含最基本的 conda 和 Python 软件。

另外如果想详尽地了解 conda 的使用方法，可以参考[官方说明文档](https://docs.conda.io/projects/conda/en/stable/index.html)，阅读完后基本就可以使用 conda 顺利地搭建 Python 虚拟环境了。
