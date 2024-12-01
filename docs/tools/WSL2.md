# WSL2

!!! info
     本节关于 WSL2 的部分只建议使用 Windows 系统的同学参考。

## 基本介绍

这是微软官方给出的关于 WSL 的介绍：

!!! note "Introduction"
     适用于 Linux 的 Windows 子系统 (WSL) 是 Windows 的一项功能，可用于在 Windows 计算机上运行 Linux 环境，而无需单独的虚拟机或双引导。 WSL 旨在为希望同时使用 Windows 和 Linux 的开发人员提供无缝高效的体验。

     - 使用 WSL 安装和运行各种 Linux 发行版，例如 Ubuntu、Debian、Kali 等。 安装 Linux 发行版并从 Microsoft Store 接收自动更新、导入 Microsoft Store 中不可用的 Linux 发行版，或构建你自己的客户 Linux 发行版。
     - 将文件存储在独立的 Linux 文件系统中，具体取决于安装的发行版。
     - 运行命令行工具，例如 BASH。
     - 运行常用的 BASH 命令行工具（例如 grep、sed、awk）或其他 ELF-64 二进制文件。
     - 运行 Bash 脚本和 GNU/Linux 命令行应用程序，包括：
     - 工具：vim、emacs、tmux
     - 语言：NodeJS、JavaScript、Python、Ruby、C/C++、C# 和 F#、Rust、Go 等。
     - 服务：SSHD、MySQL、Apache、lighttpd、MongoDB、PostgreSQL。
     - 使用自己的 GNU/Linux 分发包管理器安装其他软件。
     - 使用类似于 Unix 的命令行 shell 调用 Windows 应用程序。
     - 在 Windows 上调用 GNU/Linux 应用程序。
     - 运行直接集成到 Windows 桌面的 GNU/Linux 图形应用程序
     - 使用你的设备 GPU 加速 Linux 上运行的机器学习工作负载。

而 WSL2 则是微软推出的第二个版本的 WSL，在文件 IO 性能、systemd 支持、系统调用兼容性等方面做得比 WSL1 更好。关于 WSL1 和 WSL2 的区别，可以阅读[官方文档](https://learn.microsoft.com/zh-cn/windows/wsl/compare-versions)。

## 优点及缺陷

在我看来，WSL2 的优点主要有：

1. 在 WSL2 中可以直接使用 Windows 中的 GPU、NVIDIA 驱动，在传统的虚拟机中则无法享受到这一便利；
2. WSL2 中的 Linux 发行版和宿主 Windows 系统几乎无缝集成，不用像双系统一样来回切换，资源占用也少于传统的虚拟机。
3. WSL2 在完成机器学习、深度学习任务中性能优于 Windows 系统，在某些情况下甚至和原生 Linux 系统接近；
4. WSL2 安装更为快捷、简单。只需要根据官方步骤执行几步命令就能完成安装，相较于双系统更加简便。
5. Windows 系统下的 Docker 使用体验很差，只有依托 WSL 才能享受到类似于 Linux 中的效果。
6. WSL2 中进行 LaTeX 编译的速度明显快于 Windows 中的速度，能有效减少等待编译的时间。

当然，WSL2 也不可避免地有一些缺陷：

1. 内存占用高。有些时候，进程 VmmemWSL 不会自动结束，导致内存占用过高；并且由于默认会分配给 WSL 最高达总内存一半的内存，使得 Windows 主机的内存可能会不太够用（Windows 本身内存占用就偏高）。可以通过参考 [WSL 的高级设置](https://learn.microsoft.com/en-us/windows/wsl/wsl-config)来进行内存分配等功能的配置。也可以使用一个轻量的软件 [Mem Reduct](https://github.com/henrypp/memreduct) 进行定时的内存清理；
2. 跨系统的文件交互有性能瓶颈。如果需要大量跨系统文件交互的话，速度会非常慢。因此建议将项目文件全部置于 WSL2 中以避免这种情况。
3. 磁盘空间不会自动回收，在 WSL2 中删除文件后，Windows 中并不会释放磁盘空间，需要手动压缩释放（并且最好转移到 D 盘中，以避免 C 盘空间占用过高）。
4. 涉及到硬件层面的支持不友好，例如对 USB 设备的支持不太理想，目前只能使用 [usbipd-win](https://github.com/dorssel/usbipd-win) 来实现对宿主机的 USB 设备的访问。
5. 启用 Hyper-V 之后， VMware 等虚拟机软件性能有所下降。

## 安装及使用

关于 WSL2 的安装教程，可以参考[官方文档](https://learn.microsoft.com/en-us/windows/wsl/install)。之后可以按照 [WSL 的高级设置](https://learn.microsoft.com/en-us/windows/wsl/wsl-config)来进行进一步配置。官方文档中也解决了使用中的一部分问题，建议按需阅读。关于 WSL2 的更进一步的使用方法，请自行 Google。

另外，在一份 [texlive 的安装教程](https://tug.ctan.org/info/install-latex-guide-zh-cn/install-latex-guide-zh-cn.pdf)的附录中，包含了一些 WSL 的教程（例如将 Linux 发行版迁移到非系统盘等），可以作为参考。

## Linux 使用教程

由于使用 WSL2 的初衷也有学习 Linux 的基本操作，因此也需要一些 Linux 教程：

1. [菜鸟教程](https://www.runoob.com/linux/linux-tutorial.html)
2. [Linux 101](https://101.lug.ustc.edu.cn/)（Ubuntu）
3. [鳥哥的 Linux 私房菜](https://linux.vbird.org/)（CentOS7）

个人使用的是后两者，可以帮助小白快速入门 Linux。

此外，MIT 的 [The-Missing-Semester](https://missing.csail.mit.edu/2020/) 课程也可以作为参考，中文翻译网址 <https://missing-semester-cn.github.io/>；以及[《快乐的 Linux 命令行》中文翻译](https://billie66.github.io/TLCL/)。

## 配置深度学习环境

在熟悉了 WSL2 的基本操作之后，就可以开始配置机器学习/深度学习的环境了，我的大致配置过程如下：

1. 在 Windows 中安装 NVIDIA 驱动程序
2. 在 WSL2 中安装 Anaconda / Miniconda，或使用 [Docker](./Docker.md)，但是 [conda](./Conda.md) 的上手相对更简单一些
3. 在 WSL2 中利用 conda 创建虚拟环境，并安装 Pytorch 等需要的包
4. 按需安装 cuda-toolkit 和 cudnn。根据根据需求，决定是使用 conda 在特定深度学习环境中局部安装，还是为 WSL2 进行全局安装。
5. 使用 VS Code 或 Pycharm 专业版等远程连接 WSL2（或者直接在 WSL2 中安装 IDE/编辑器，不太推荐），开始 coding。

由于电脑情况各不相同，还请自行搜索安装教程。这里给出我参考的中文教程：<https://zhuanlan.zhihu.com/p/621142457>，以及 <https://zhuanlan.zhihu.com/p/434239083>。其中，前者侧重于基于 Docker 的配置方法，后者侧重于基于 Anaconda 的配置方法（个人并不推荐其中安装 intelliJ Ultimate 的步骤），参考时请关注年份是否合适，如果过于久远请查找最新版本的配置方法！当然，前往官网搜索一定能保证时效性，故更推荐自行查找 NVIDIA 以及 Pytorch 官网教程。我仅参考了这两个教程中的大致配置步骤，具体命令则是通过阅读官方文档来获得，这样安装出错的概率会大大降低。

## 一些调侃

正所谓“ Windows 是 Linux 的最大发行版”，[Microsoft 热爱 Linux](https://learn.microsoft.com/zh-cn/windows/wsl/about#microsoft-loves-linux)！！！
