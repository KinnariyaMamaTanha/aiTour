# WSL2

## 基本介绍

这是微软官方给出的关于WSL的介绍：

> 适用于 Linux 的 Windows 子系统 (WSL) 是 Windows 的一项功能，可用于在 Windows 计算机上运行 Linux 环境，而无需单独的虚拟机或双引导。 WSL 旨在为希望同时使用 Windows 和 Linux 的开发人员提供无缝高效的体验。

>  - 使用 WSL 安装和运行各种 Linux 发行版，例如 Ubuntu、Debian、Kali 等。 安装 Linux 发行版并从 Microsoft Store 接收自动更新、导入 Microsoft Store 中不可用的 Linux 发行版，或构建你自己的客户 Linux 发行版。
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

在我看来，WSL2的优点主要有：

1. 相较于虚拟机方案，WSL2更轻便，内存占用更少，并且和Windows系统的文件互通性更好(在Windows的文件管理器中可以访问当前Linux权限下的所有文件；在Linux中C盘、D盘等磁盘被默认挂载，可以通过`/mnt/c/`等路径直接访问，也可以选择配置不挂载C盘等)；
2. 相较于双系统方案，WSL2安装、启动更方便快捷（因装双系统而导致原生Windows系统裂开的例子数不胜数），并且足以胜任日常学习；另外，Linux子系统和Windows系统可以同时运行，不需要频繁地开关机；
3. 可以同时安装多个Linux发行版，同时体验到多个版本的快乐（<del>折腾</del>）。

由于WSL2相较于原生Linux系统性能下降较小，故非常适合用于进行机器学习等任务（至少比Windows快，我的一个直观的感受是在Windows中）。所以我在寒假中将原本部署在Windows上深度学习环境全部转移到了WSL2中，而office等其它应用则保留在了Windows系统中(我更愿意调侃此时的Windows为Linux的大号桌面)。这样做也能提前适应之后的科研等活动。

## 安装及使用

关于WSL2的安装教程，可以参考[官方文档](https://learn.microsoft.com/en-us/windows/wsl/install)。另外，官方文档也解决了使用中的一部分问题，建议按需阅读。关于WSL2的更进一步的使用方法，请自行Google。

## 存在的问题

在我编辑这个页面时，WSL2还存在如下问题：

1. 内存占用高（其实不止WSL2，Windows11本身内存占用就很高）。可以参考[官方配置文档](https://learn.microsoft.com/en-us/windows/wsl/wsl-config#wslconfig)进行配置，以减少内存占用（或者自行加装内存条dog.jpg）。也可以使用一个轻量的软件[Mem Reduct](https://github.com/henrypp/memreduct)进行定时的内存清理；
2. 对GUI应用支持不太友好。这点因个人电脑而异（例如在我的电脑上始终无法正常运行xfce4桌面，参考了多方教程仍没有解决方案），可以尝试使用微软推出的[WSLg](https://learn.microsoft.com/zh-cn/windows/wsl/tutorials/gui-apps)，以在Windows直接打开Linux的GUI应用；
3. 一旦开启Hyper-V后，就无法再使用VMware或者VirtualBox等虚拟机软件了，也就是说，WSL2和它们不可兼得；
4. 磁盘空间不会自动回收，需要手动压缩空间（并且最好转移到D盘中，不然C盘很容易就会炸开）。


## Linux使用教程

由于使用WSL2的初衷就是学习Linux的基本操作，因此也需要一些Linux教程：

1. [菜鸟教程](https://www.runoob.com/linux/linux-tutorial.html)
2. [Linux 101](https://101.lug.ustc.edu.cn/)

个人使用的是后者，可以帮助小白快速入门Linux。

## 配置深度学习环境

在熟悉了WSL2的基本使用之后，就可以开始配置机器学习/深度学习的环境了，大致过程如下：

1. 在Windows中安装NVIDIA驱动程序；
2. 在WSL2中安装CUDA；
3. 在WSL2中安装cuDNN；
4. 在WSL2中安装anaconda（或conda、miniconda）；
5. 在WSL2中安装Pytorch等Python包；
6. 使用VScode或Pycharm专业版等远程连接WSL2（或者直接在WSL2中安装IDE/编辑器），开始coding。

由于不同的电脑情况不同，具体过程还请自行搜索安装教程。

## 一些调侃

正所谓“Windows是Linux的最大发行版”，[Microsoft 热爱 Linux](https://learn.microsoft.com/zh-cn/windows/wsl/about#microsoft-loves-linux)！！！
