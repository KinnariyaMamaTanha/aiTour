# Scoop

在Linux和MacOS系统中，往往自带非常方便的软件包管理器来进行下载、更新、卸载等操作，比如apt, brew, yum等，只需要类似`apt install <app>`的指令就可以便捷地安装软件。但在Windows系统中，却没有这样的包管理器，在下载软件时往往需要前往官网选择版本、进行设置安装路径、配置环境变量等复杂的过程。

这时，scoop就提供了类似上述软件的功能，可以使你在Windows上享受到“傻瓜式”软件管理。以neovim为例，只需要简单的一句指令：`scoop install neovim`，就可以直接安装neovim，并且省去了最烦人的环境变量设置的环节。另外，在下载某个软件的时候，scoop也实现了自动安装相关软件的功能，实在是非常便捷。

为了学习scoop，可以：

1. 阅读[官网](https://scoop.sh/)的说明以获得功能的简要介绍；
2. 阅读[官方文档](https://github.com/ScoopInstaller/Scoop/wiki)来获得使用scoop的最好教程。