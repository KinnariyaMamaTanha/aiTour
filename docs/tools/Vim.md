# Vim

我是从 csdiy 上的 [vim 介绍界面](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/Vim/)了解 vim 并进行学习的，相关教程可以在这个网页查询到。

个人使用感受：学习的路线实际上并不是非常陡峭（也有可能是因为我没有深入去学习）。我的学习路线是：

1. 跟着 vim 自带的 vimtutor 进行练习
2. 学习 vimrc 文件的配置，对一些常用键进行修改
3. 参考 [theniceboy 的 vim 配置文件](https://github.com/theniceboy/.vim)对 vim 进行了其它的配置，使得可以使用 vim 直接进行一些简单的 C, C++, Python 程序的运行，并且配置好了 vim 的补全功能（使用 [coc.nvim](https://github.com/neoclide/coc.nvim) 插件实现）

由于我并不打算将 vim 配置为主力 IDE，仅会在编辑单个文件时使用 vim，因此我并未进行过多的配置。但是我在使用的 IDE 和其它文本编辑器(如 vscode)中都下载了 vim 插件，以便随时使用 vim 快捷键进行编程。

另外，也推荐使用 [neovim](https://neovim.io/)，原因是：

1. 根据官网介绍，neovim "With 30% less source-code than Vim"，并且 neovim 使用 lua 而不是 vimscript 进行配置和脚本编写（意味着如果愿意的话，可以同时学习一下 lua 的语法），运行速度上比 vim 快了不少
2. vim 的原 vimrc 配置文件可以直接移植到 neovim 中，而无需重写配置文件
3. neovim 的插件更新更频繁，某些插件甚至只支持 neovim ，而一些 vim 的插件早已停止维护

写在最后：

1. 如果确实希望将 vim 配置为自己的主力 IDE，而又不想过于折腾，可以考虑下载 vim 或 neovim 的发行版，例如 [lazyvim](https://www.lazyvim.org/) 等(其它发行版我没有用过，因此不作列举)，然后修改为自己常用的按键；
2. 如果想查找vim的插件的话，可以参考 [vimawesome](https://vimawesome.com/)，里面能查找到绝大大部分vim插件；或者直接在GitHub上查询“vim + 相关功能”；
3. 关于 vim 的详细教程，参考 [vim 从入门到精通](https://gitlab.com/wsdjeg/vim-galore-zh_cn#%E6%9B%B4%E5%8A%A0%E6%99%BA%E8%83%BD%E7%9A%84%E5%BD%93%E5%89%8D%E8%A1%8C%E9%AB%98%E4%BA%AE)；
4. 世上本无编辑器的神，只有神的编辑器。
