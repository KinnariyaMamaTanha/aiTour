# Vim

我是从csdiy上的[vim介绍界面](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/Vim/)了解vim并进行学习的，相关教程可以在这个网页查询到。

个人使用感受：学习的路线实际上并不是非常陡峭。我的学习路线是：

1. 跟着vim自带的vimtutor进行练习
2. 学习vimrc文件的配置，对一些常用键进行修改
3. 参考[theniceboy的vim配置文件](https://github.com/theniceboy/.vim)对vim进行了其它的配置，使得可以使用vim直接进行一些简单的C, C++, Python程序的运行，并且配置好了vim的补全功能

由于我并不打算将vim配置为主力IDE，仅会在编辑单个文件时使用vim，因此我并未进行过多的配置。但是我在使用的IDE和其它文本编辑器(如vscode)中都下载了vim插件，以便随时使用vim快捷键进行编程。

另外，也推荐使用[neovim](https://neovim.io/)，原因是：

1. 根据官网介绍，neovim "With 30% less source-code than Vim"，并且neovim使用lua而不是vimscript进行配置和脚本编写（意味着如果愿意的话，可以同时学习lua的语法），运行速度上比vim快了不少
2. vim的原 vimrc 配置文件可以直接移植到neovim中，而无需重写配置文件
3. neovim的插件更新更频繁，某些插件甚至只支持neovim

写在最后：

1. 如果确实希望将vim配置为自己的主力IDE，而又不想过于折腾，可以考虑下载vim或neovim的发行版，例如[lazyvim](https://www.lazyvim.org/)等(其它发行版我没有用过，因此不作列举)，然后修改为自己常用的按键；
2. 如果想查找vim的插件的话，可以参考[vimawesome](https://vimawesome.com/)，里面能查找到大部分vim插件；或者直接在GitHub上查询“vim + 相关功能”；
3. 世上本无编辑器的神，只有神的编辑器。
