# Obsidian

Obsidian 是我主要使用的笔记软件，我使用它记录一些计算机相关的笔记，便于需要时查询。

Obsidian 使用 Markdown 语法（但不是 [GitHub Favored Markdown](https://github.github.com/gfm/)，中文介绍可参考[这个网址](https://gfm.docschina.org/zh-hans/)，这是 Obsidian 美中不足的一点）。它集成了记笔记所需的所有基础功能，包括模板、笔记双链、笔记漫游、各种格式导出等，更重要的是，Obsidian 还拥有一个强大的插件市场，你可以按需从中获取插件以方便自己做笔记。区别于收费的 Typora，Obsidian 几乎所有功能都是免费的（收费的功能也有免费的替代方案），包括其插件，这也是我使用 Obsidian 而不是 Typora 的原因之一。

## 关于使用教程

最好的 Obsidian 教程是安装后自带的沙盒(Sandbox)仓库以及[官方教程](https://help.obsidian.md/Home)，其中也包含了 Obsidian 使用的 Markdown 语法。

## 关于插件

网络上的博客往往会推荐很多 Obsidian 的插件，但是大多数都违背了使用 Obsidian 的做笔记的初衷。诚然，可以将 Obsidian 配置为待办事务管理工具，思维导图制作工具，甚至是日程管理工具，但是为什么不使用专门的相关工具，而要费心思把笔记软件配置出其它用途呢？

我也尝试过若干插件，但是最终使用的也只有寥寥几个：Advanced Tables, Completr, Minimal Theme Settings, Style Settings, Recent Files 以及 Vimrc Support（其中主题设置的插件 Minimal Theme Settings 和 Style Settings 并非必须，如果不使用 vim 模式的话，Vimrc Support 插件也不需要，这样算来，一共也就使用了4个插件）。可见为了满足记笔记这一项功能，安装很多插件是完全没有必要的。

## 关于主题配置

赏心悦目的 UI 固然怡人，但是也不应该花费太多时间在界面配置上。如果你有折腾的习惯，请注意控制好自己的双手和大脑，把重心放在记笔记这件事本身上吧！（对于其它软件的配置也是同样）

## 关于同步与备份

实际上有多种同步 Obsidian 方式，我选择使用 *Obsidian + Git + Github* 的方法，只需要定期向 Github 中递交最新版本的笔记，就可以在别处通过克隆仓库的方式下载完整笔记库了。（注：Obsidian 有用于自动同步 GitHub 的插件，但是我没有使用，故在此不作介绍。另外，也可以尝试 Obsidian + OneDrive 的方式进行笔记同步，通过学生优惠能够获得 4T 的云存储空间以及实时同步的功能，缺点是本地误删会导致云端文件也被删除，并且无法在 OneDrive 中直接预览 .md 文件）

## 关于缺陷

不可避免地，Obsidian 也存在一些缺点。例如：

1. 只能编辑存在于某一个仓库(vault)中的 Markdown 文件，而不能编辑仓库以外的文件，因此不能像 Typora 一样作为 Markdown 文件编辑器使用。（此时 vim 或者 vscode 就可以派上用场了）
2. 功能较为多了些（也有人说是臃肿），对于仅仅想编辑 Markdown 文件而不想构建成体系的笔记仓库的同学，可以考虑使用 Typora、vim、VS Code等，而不是 Obsidian。

更进一步地，如果你想将 Obsidian 融入自己的日常学习工作流中，可以参考 csdiy 中[关于 Obsidian 的介绍](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/workflow/)。
