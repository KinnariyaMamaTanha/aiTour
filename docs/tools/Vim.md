# Vim

我是从 csdiy 上的 [vim 介绍界面](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/Vim/)了解 vim 并进行学习的，相关教程可以在这个网页查询到。

个人使用感受：学习的路线实际上并不是非常陡峭（也有可能是因为我没有深入去学习）。我的学习路线是：

1. 跟着 vim 自带的 vimtutor 进行练习
2. 学习 vimrc 文件的配置，对一些常用键进行修改，参考了 [theCW 的视频讲解](https://www.bilibili.com/video/BV164411P7tw?vd_source=c9e11661823ca4062db1ef99f7e0eee1)
3. 参考 [theniceboy 的 vim 配置文件](https://github.com/theniceboy/.vim)对 vim 进行了其它的配置，使得可以使用 vim 直接进行一些简单的 C, C++, Python 程序的运行，并且配置好了 vim 的补全功能（使用 [coc.nvim](https://github.com/neoclide/coc.nvim) 插件实现）

我将自己的 vim 配置好了一些必要的功能，使得使用 vim 编写中小型项目、记录笔记、写有组织的日记等事情成为了可能，并且我在使用的 IDE 和其它文本编辑器（如 vscode）中都下载了 vim 插件，以便随时使用 vim 快捷操作（一部分原因是我已经习惯了 vim 的键位了，不太好改回来）。

另外，也可以尝试使用 [neovim](https://neovim.io/)，原因是：

1. 根据官网介绍，neovim "With 30% less source-code than Vim"，并且 neovim 使用 lua 而不是 vimscript 进行配置和脚本编写（意味着如果愿意的话，可以同时学习一下 lua 的语法），运行速度上比 vim 快了不少
2. vim 的原 vimrc 配置文件可以直接移植到 neovim 中，而无需重写配置文件
3. neovim 的插件更新更频繁，某些插件甚至只支持 neovim ，而一些 vim 的插件早已停止维护。

写在最后：

1. 如果确实希望将 vim 配置为自己的主力 IDE，而又不想过于折腾，可以考虑安装 vim 或 neovim 的发行版，例如 [LazyVim](https://www.lazyvim.org/) 、[LunarVim](https://github.com/lunarvim/lunarvim) 等(其它发行版我没有用过，因此不作列举)，然后在此基础上进行其它配置；
2. 如果想查找 vim 的插件的话，可以参考 [vimawesome](https://vimawesome.com/)，里面能查找到绝大部分 vim 插件；或者直接在 GitHub 上查询 “vim + 相关功能”；
3. 关于 vim 的详细教程，参考 [vim 从入门到精通](https://gitlab.com/wsdjeg/vim-galore-zh_cn#%E6%9B%B4%E5%8A%A0%E6%99%BA%E8%83%BD%E7%9A%84%E5%BD%93%E5%89%8D%E8%A1%8C%E9%AB%98%E4%BA%AE)；
4. 送给喜欢折腾的同学的话：完成一件事，重要的并非你所使用的工具，而是你最终是否完成它，以及你在完成这件事时的收获与感悟。vim 的确拥有一种独特的哲学，也可能在一些情况下是必需品，但是在拥有更好的替代工具时，例如其他的编辑器、IDE 或者什么软件的时候，如非必要，请不要过于迷恋 vim，请使用更好的、更专业的、更节省你自己的时间的工具——因为时间就是生命，对于我们这些自学的学生来讲，更应该是如此。至于其它软件，也是同理。
5. 世上本无编辑器的神，只有神的编辑器。
