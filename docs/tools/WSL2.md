# WSL2

!!! info
     本文只建议使用 Windows 系统的同学参考

## 基本介绍

这是微软官方给出的关于WSL的介绍：

> 适用于 Linux 的 Windows 子系统 (WSL) 是 Windows 的一项功能，可用于在 Windows 计算机上运行 Linux 环境，而无需单独的虚拟机或双引导。 WSL 旨在为希望同时使用 Windows 和 Linux 的开发人员提供无缝高效的体验。

> - 使用 WSL 安装和运行各种 Linux 发行版，例如 Ubuntu、Debian、Kali 等。 安装 Linux 发行版并从 Microsoft Store 接收自动更新、导入 Microsoft Store 中不可用的 Linux 发行版，或构建你自己的客户 Linux 发行版。
> - 将文件存储在独立的 Linux 文件系统中，具体取决于安装的发行版。
> - 运行命令行工具，例如 BASH。
> - 运行常用的 BASH 命令行工具（例如 grep、sed、awk）或其他 ELF-64 二进制文件。
> - 运行 Bash 脚本和 GNU/Linux 命令行应用程序，包括：
> - 工具：vim、emacs、tmux
> - 语言：NodeJS、JavaScript、Python、Ruby、C/C++、C# 和 F#、Rust、Go 等。
> - 服务：SSHD、MySQL、Apache、lighttpd、MongoDB、PostgreSQL。
> - 使用自己的 GNU/Linux 分发包管理器安装其他软件。
> - 使用类似于 Unix 的命令行 shell 调用 Windows 应用程序。
> - 在 Windows 上调用 GNU/Linux 应用程序。
> - 运行直接集成到 Windows 桌面的 GNU/Linux 图形应用程序
> - 使用你的设备 GPU 加速 Linux 上运行的机器学习工作负载。

## 优点

在我看来，WSL2 的优点主要有：

1. 相较于虚拟机方案，WSL2 更轻便，内存占用更少，并且和 Windows 系统的文件互通性更好(在 Windows 的文件管理器中可以访问当前 Linux 权限下的所有文件；在 Linux 中 C 盘、D 盘等磁盘被默认挂载，可以通过 `/mnt/c/` 等路径直接访问，也可以选择配置不挂载 C 盘等)；
2. 相较于双系统方案，WSL2 安装、启动更方便快捷（因装双系统而导致原生 Windows 系统裂开的例子数不胜数），并且足以胜任日常学习；另外，Linux 子系统和 Windows 系统可以同时运行，不需要频繁地开关机来切换系统；
3. 可以同时安装多个 Linux 发行版，同时体验到多个版本的快乐（<del>折腾</del>）。

由于WSL2相较于原生 Linux 系统性能下降较小，故非常适合用于进行机器学习等任务（至少比 Windows 快，我的一个直观的感受是导入 Pytorch 包以及 xelatex 的编译等操作都是 WSL2 中显著地快于 Windows 中）。所以我在寒假中将原本部署在 Windows 上深度学习环境全部转移到了 WSL2 中，而 office 等其它应用则保留在了 Windows 系统中（我更愿意调侃此时的 Windows 为 Linux 的大号桌面）。这样做也能提前适应之后的科研等活动。如果你也使用 Windows 系统的话，不妨尝试一下 WSL2！

## 安装及使用

关于 WSL2 的安装教程，可以参考[官方文档](https://learn.microsoft.com/en-us/windows/wsl/install)。另外，官方文档也解决了使用中的一部分问题，建议按需阅读。关于 WSL2 的更进一步的使用方法，请自行 Google。

另外，在一份[texlive的安装教程](https://tug.ctan.org/info/install-latex-guide-zh-cn/install-latex-guide-zh-cn.pdf)的附录中，包含了一些 WSL 的教程（例如将 Linux 发行版迁移到非系统盘等），可以作为参考。

## 存在的问题

在我编辑这个页面时，WSL2 还存在如下问题：

1. 内存占用高（其实不止 WSL2，Windows11 本身内存占用就很高）。可以参考[官方配置文档](https://learn.microsoft.com/en-us/windows/wsl/wsl-config#wslconfig)进行配置，以减少内存占用（或者自行加装内存条dog.jpg）。也可以使用一个轻量的软件 [Mem Reduct](https://github.com/henrypp/memreduct) 进行定时的内存清理；
2. 对 GUI 应用支持不太友好。这点因个人电脑而异（例如在我的电脑上始终无法正常运行 xfce4 桌面，参考了多方教程仍没有解决方案），可以尝试使用微软推出的 [WSLg](https://learn.microsoft.com/zh-cn/windows/wsl/tutorials/gui-apps) ，以在 Windows 直接打开 Linux 的 GUI 应用；（2024-03-23补充：我通过 X server 成功配置好了 xfce4 桌面，但是很卡顿，体验不好，可能是电脑自身配置的原因，故放弃 WSL2 桌面）
3. 一旦开启 Hyper-V 后，就无法再使用 VMware 或者 VirtualBox 等虚拟机软件了，也就是说，WSL2 和它们不可兼得；（2024-03-19补充：VMware 已经支持 Hyper-V；VirtualBox 也行，但是还存在一些 bug）
4. 磁盘空间不会自动回收，需要手动压缩空间（并且最好转移到 D 盘中，不然 C 盘很容易就会炸开）。

## Linux使用教程

由于使用WSL2的初衷就是学习 Linux 的基本操作，因此也需要一些 Linux 教程：

1. [菜鸟教程](https://www.runoob.com/linux/linux-tutorial.html)
2. [Linux 101](https://101.lug.ustc.edu.cn/)（Ubuntu）
3. [鳥哥的Linux私房菜](https://linux.vbird.org/)（CentOS7）

个人使用的是后两者，可以帮助小白快速入门 Linux。

此外，MIT 的 [The-missing-semester](https://missing.csail.mit.edu/2020/) 课程也可以作为参考，中文翻译网址<https://missing-semester-cn.github.io/>

## 配置深度学习环境

在熟悉了 WSL2 的基本操作之后，就可以开始配置机器学习/深度学习的环境了，我的大致配置过程如下：

1. 在 Windows 中安装NVIDIA驱动程序
2. 在 WSL2 中安装 CUDA
3. 在 WSL2 中安装 cuDNN
4. 在 WSL2 中安装 anaconda（或 conda、miniconda）。当然不一定非要用 anaconda，使用 [docker](./Docker.md) 一样可以，但是 anaconda 的配置相对更简单一些
5. 在 WSL2 中安装 Pytorch 等 Python 包
6. 使用 VScode 或 Pycharm 专业版等远程连接 WSL2（或者直接在 WSL2 中安装 IDE/编辑器，不太推荐），开始 coding

由于不同的电脑情况不同，具体过程还请自行搜索安装教程。这里给出我参考的中文教程：<https://zhuanlan.zhihu.com/p/621142457>，以及<https://zhuanlan.zhihu.com/p/434239083>。其中，前者侧重于基于 docker 的配置方法，后者侧重于基于 anaconda 的配置方法（最后一部分安装 intelliJ Ultimate 的步骤可省略），参考时请关注年份是否合适，如果过于久远请查找最新版本的配置方法！

注意：我仅参考了教程中的大致配置步骤，具体命令则是通过阅读官方文档来获得，这样出错的概率会大大降低。并且由于此时我还没有学习 docker 的使用方法，故采用的是 anaconda 来进行环境配置。

## 一些调侃

正所谓“ Windows 是 Linux 的最大发行版”，[Microsoft 热爱 Linux](https://learn.microsoft.com/zh-cn/windows/wsl/about#microsoft-loves-linux)！！！
