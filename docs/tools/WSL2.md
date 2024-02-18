---
hide:
    - footer
---

# WSL2

WSL，全称"Windows Subsystem for Linux"，用于在Windows系统中运行Linux系统，而WSL2为WSL的第二个版本。WSL2是基于完整的Linux内核构建的，因此能提供更好的性能和更好的兼容性，使得在 Windows 系统上运行 Linux 应用程序更加流畅和稳定。

相较于虚拟机方案，WSL2更轻便，并且和Windows系统的文件互通性更好(在Windows的文件管理器中可以访问当前Linux权限下的所有文件；在Linux中C盘、D盘等磁盘被默认挂载，可以直接访问)；相较于双系统方案，WSL2安装、启动更方便、快捷，并且足以胜任日常学习。

由于WSL2相较于原生Linux系统性能下降很小，故非常适合用于进行机器学习等任务。所以我在寒假中将原本部署在Windows上深度学习环境全部转移到了WSL2中。这样一来，我的学习环境就转移到了Linux中，而office等其它应用则保留在了Windows系统中(我更愿意调侃此时的Windows为Linux的大号桌面)。这样做也能提前适应之后的科研等活动。

关于WSL2的安装教程，可以参考[官方文档](https://learn.microsoft.com/en-us/windows/wsl/install)。

在我编辑这个页面时，WSL2还存在如下问题：

1. 内存占用高（其实不止WSL2，Windows11本身内存占用就很高）。可以参考[官方配置文档](https://learn.microsoft.com/en-us/windows/wsl/wsl-config#wslconfig)进行配置，以减少内存占用（或者自行加装内存条dog.jpg）。也可以使用一个轻量的软件[Mem Reduct](https://github.com/henrypp/memreduct)进行定时的内存清理。
2. 对GUI应用支持不太友好。这点因个人电脑而异（例如在我的电脑上始终无法正常运行xfce4桌面，参考了多方教程仍没有解决方案），可以尝试使用微软推出的[WSLg](https://learn.microsoft.com/zh-cn/windows/wsl/tutorials/gui-apps)，以在Windows直接打开Linux的GUI应用。

关于WSL2的更进一步的使用方法，可以自行Google。

由于使用WSL2的初衷就是学习Linux，因此也需要一些Linux教程：
1. [菜鸟教程](https://www.runoob.com/linux/linux-tutorial.html)
2. [Linux 101](https://101.lug.ustc.edu.cn/)
