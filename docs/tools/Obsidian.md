---
hide:
    - footer
---
# Obsidian - 一款强大的笔记工具

Obsidian是我主要使用的记笔记软件，我使用它记录一些计算机相关的笔记，便于需要时查询。

Obsidian使用Markdown语法（但不是GFM, [GitHub Favored Markdown](https://github.github.com/gfm/)，中文介绍可参考[这个网址](https://gfm.docschina.org/zh-hans/)，这是Obsidian美中不足的一点）。它集成了记笔记所需的所有基础功能，包括模板、笔记双链、笔记漫游、各种格式导出等，更重要的是，Obsidian还拥有一个强大的插件市场，你可以按需从中获取插件以方便自己做笔记。区别于收费的Typora，Obsidian是免费的，包括其插件，这也是我使用Obsidian而不是Typora的原因之一。

**关于使用教程**：最好的Obsidian教程是安装后自带的沙盒(Sandbox)仓库以及[官方教程](https://help.obsidian.md/Home)，其中也包含了Obsidian使用的Markdown语法。

**关于插件**：网络上往往会推荐很多Obsidian的插件，但是大多数都违背了使用Obsidian的做笔记的初衷。诚然，可以将Obsidian配置为待办事务管理工具，思维导图制作工具，甚至是日程管理工具，但是为什么不使用相关的专门工具，而要费心思把笔记软件配置出其它用途呢？我也尝试过若干插件，但是最终使用的也只有寥寥几个：Excute Code, Advanced Tables, Completr, Minimal Theme Settings, Style Settings, Recent Files以及Vimrc Support（其中主题设置的插件Minimal Theme Settings和Style Settings并非必须，如果不使用vim模式的话，Vimrc Support插件也不需要，这样算来，一共也就使用了4个插件）。我的个人配置可见于我的[Notes仓库](https://github.com/KinnariyaMamaTanha/Notes)中的.obsidian文件，直接克隆至本地即可使用。

**关于主题配置**：赏心悦目的UI固然怡人，但是也不应该花费太多时间在界面配置上。如果你有折腾的习惯，请注意控制好自己的双手和大脑，把重心放在记笔记这件事本身上吧！（对于其它软件的配置也是同样）

**关于同步**：网上有多种同步Obsidian方式，我选择使用Obsidian + Git + Github模式，由于Obsidian中的笔记库(vault)和Git中的仓库(repository)有相似之处，因此我直接将一个Obsidian库作为Git的repository进行存储。只需要定期向Github中递交最新版本的笔记，就可以在别处通过克隆仓库的方式下载完整笔记库了。（注：Obsidian有用于自动同步GitHub的插件，但是我没有使用，故在此不作介绍。另外，也可以尝试Obsidian + OneDrive的方式进行笔记同步，通过学生优惠能够获得4T的云存储空间以及实时同步的功能，缺点是本地误删会导致云端文件也被删除）

**关于缺陷**：不可避免地，Obsidian也存在一些缺点。例如：
1. 只能编辑存在于某一个仓库(vault)中的Markdown文件，而不能编辑仓库以外的文件，因此不能像Typora一样作为Markdown文件编辑器使用。
2. 功能较为多了些（也有人说是臃肿），对于仅仅想编辑Markdown文件而不想构建成体系的笔记仓库的同学，可以考虑使用Typora而不是Obsidian。

更进一步地，如果你想将Obsidian融入自己的日常学习工作流中，可以参考csdiy中[关于Obsidian的介绍](https://csdiy.wiki/%E5%BF%85%E5%AD%A6%E5%B7%A5%E5%85%B7/workflow/)。
