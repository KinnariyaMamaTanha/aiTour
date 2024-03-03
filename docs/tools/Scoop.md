# Scoop

在Linux和MacOS系统中，往往自带非常方便的软件包管理器来进行下载、更新、卸载等操作，比如apt, brew, yum等，只需要类似`apt install <app>`的指令就可以便捷地安装软件。但在Windows系统中，却没有这样的包管理器，在下载软件时往往需要前往官网选择版本、进行设置安装路径、配置环境变量等复杂的过程。如果你使用的是Windows系统，并且还是一个电脑小白的话，很有可能会迷茫于不同软件的软件安装过程。

这时，scoop就提供了类似上述软件的功能，可以使你在Windows上享受到“傻瓜式”软件管理。以neovim为例，只需要简单的一句指令：`scoop install neovim`，就可以直接安装neovim，并且省去了最烦人的环境变量设置的环节。另外，在下载某个软件的时候，scoop也实现了自动安装相关软件的功能，实在是非常便捷。

为了学习scoop的用法，可以：

1. 阅读[官网](https://scoop.sh/)的说明以获得功能的简要介绍；
2. 阅读[官方文档](https://github.com/ScoopInstaller/Scoop/wiki)来获得使用scoop的最好教程。
3. 开始在Windows上使用scoop管理软件包。

当然，scoop也不是万能的，例如：

1. 对于一些重型的软件，如Visual Studio、Matlab等，scoop也无能为力；
2. 使用scoop会跳过软件设置中的一些UI界面，所以你无法在安装时就进行customize。

但是，对于一些轻量级的软件，如vim、obidian、git等，scoop完全可以胜任安装任务，所以，具体取舍还是要看你自己了。
