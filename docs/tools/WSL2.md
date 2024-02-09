---
hide:
    - footer
---

# WSL2

WSL，全称"Windows Subsystem for Linux"，用于在Windows系统中运行Linux系统，而WSL2为WSL的第二个版本。WSL2是基于完整的Linux内核构建的，因此能提供更好的性能和更好的兼容性，使得在 Windows 系统上运行 Linux 应用程序更加流畅和稳定。

相较于虚拟机方案，WSL2更轻便，并且和Windows系统的文件互通性更好(在Windows的文件管理器中可以访问当前Linux权限下的所有文件；在Linux中C盘、D盘等磁盘被默认挂载，可以直接访问)；相较于双系统方案，WSL2安装、启动更方便、快捷，并且Linux系统崩溃基本不会影响Windows系统。

由于WSL2相较于原生Linux系统性能下降并不大，故非常适合用于进行机器学习等任务。所以我在寒假中将原本部署在Windows上深度学习环境全部转移到了WSL2中，这样学习环境就转移到了Linux中，而office等其它应用则保留在了Windows系统中(我更愿意称此时的Windows系统为Linux系统的大号桌面)。这样做也能为之后的科研等活动进行准备。

关于WSL2的安装教程，可以参考[官方文档](https://learn.microsoft.com/en-us/windows/wsl/install)。更进一步的使用方法，可以自行Google。