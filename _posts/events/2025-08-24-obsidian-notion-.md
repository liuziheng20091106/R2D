> id: https://sspai.com/post/102002

> link: https://sspai.com/post/102002

> title: Obsidian Notion

# Obsidian Notion
_Published on Sun, 24 Aug 2025 09:06:31 GMT_

![Article Cover Image](https://cdnfile.sspai.com/2025/08/21/a75a4f6508a0e99c406c192efd208fb2.png)  

**Matrix 首页推荐** 

[Matrix](https://sspai.com/matrix) 是少数派的写作社区，我们主张分享真实的产品体验，有实用价值的经验与思考。我们会不定期挑选 Matrix 最优质的文章，展示来自用户的最真实的体验和观点。   
文章代表作者个人观点，少数派仅对标题和排版略作修改。

* * *

官方版 Dataview 插件
---------------

从 1.9.0 到 1.9.10，经过 10 个版本的迭代，Obsidian 终于公开发布了 Bases 功能，官方译名为「数据库」。有了「数据库」赋能，Obsidian 是否可以完全替代 Notion 了呢？

**先说结论：就目前发布的功能而言，Bases 倒不如说是官方推出的、升级版 Dataview 插件，提供了用户友好的操作界面，更高效的性能查询，但远远称不上「数据库」**。它更像是组织 pages 的视图容器，你可以使用不同的查询维度和排序方式，将仓库中的 pages 以表格或卡片的形式展示出来。

对比维度

Bases(1.9.10)

Dataview

**数据源**

笔记的属性

笔记的元数据**和**内联字段

**交互方式**

可视化操作

纯代码式

**数据编辑**

可编辑

只读

**实时性**

修改后实时同步

查询时重新渲染

**视图类型**

表格、卡片

表格、列表、任务

这样的 Bases 似乎让人略显失望，但从 Obsidian 的设计理念出发，这其实是一种必然。Obsidian 沿袭的是「文件优先」的哲学，采用去中心化、弱结构化的模式，数据模型是自下而上的：用户首先创建独立的 Markdown 笔记，然后通过 Bases 这一「视图」来聚合和组织这些笔记。

相比较而言，Notion 在官方文档中虽然也将 database 称作是「collections of pages」，但它本质上却是一种自上而下的数据结构，即用户首先创建数据库这个框架，然后向其中填充页面内容。因而 Notion 能够提供强大的原生关系（Relations）和汇总（Rollups）功能，支持跨数据库复杂关联。

就好像 Notion 的离线模式不那么「离线」，Obsidian 的数据库也不那么「数据库」，这是由软件自身的设计理念所决定的，享受了 Obsidian 卓越的离线能力和丰富的插件生态，也需接受它在数据库功能上的不足。

功能项

OB Bases

Notion

数据库模型

笔记集合（去中心化）

页面集合（中心化）

核心视图

表格、卡片

表格、列表、看板、日历、画廊、时间线等

关系/汇总

暂无

支持 Relations 和 Rollups

公式语法

面向对象式

函数式，与电子表格语法类似

模板功能

暂无

强大的内置和社区模板库

文件嵌入

支持

支持多种外部服务内容嵌入

Bases 使用实践
----------

话虽如此，Bases 功能仍然带来了很多全新的体验，以下是我推荐的两种实践方式：

### 电子书架

结合 Weread 插件和 Bases，我们可以轻易实现一个电子书架：将自己阅读过的、做过笔记的书，以卡片的形式展示出来。

![image.png|800](https://cdnfile.sspai.com/2025/08/21/article/976d8c5d0f65ff0f9c86b14f977c896a.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

整个过程非常简单：

#### **安装并设置 Weread 插件**

首先安装 Weread 插件，登录并同步笔记。这个插件可以将你在微信读书上的笔记同步到 Obsidian 仓库中。但是注意，如果一本书你从头到尾读完了，却没有留下任何笔记或是书评，是不会同步的。

我在仓库文件夹下创建了名为「WeRead」的文件夹来单独保存插件同步的笔记内容，这样不会影响现有的内容，也方便接下来在 Bases 中的设置。记得要在 Weread 插件中设置你要保存笔记的文件夹。

Weread 插件在同步笔记时，也会将书籍的元信息以 YAML 的形式插入到 page 中，比如作者、ISBN、阅读时长等等，同时也包括了书籍的封面图片链接，记录在 `cover` 属性中。

#### 创建并设置 Bases

接下来创建一个新的 Bases。你可以使用 `command + p` 打开命令面板，输入「创建新数据库」来查询并执行命令，或是在左侧文件列表的文件夹上右键，选择「创建新数据库」。

在 Bases 的左上方，打开视图配置，将「布局」切换为「卡片」，「图像属性」设置为「cover」，对应每本书籍的封面图片链接，「图像适配」可以设置为「完整包含」，这样可以完整展示图片的全貌。

![image.png|200](https://cdnfile.sspai.com/2025/08/21/article/5f2d91f329c844bfd7eba77fa5fc4238.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

打开 Bases 右上方的筛选功能，将过滤条件设置为：「文件夹」是微信读书同步笔记的文件夹。

![image.png|500](https://cdnfile.sspai.com/2025/08/21/article/94f7124d74bf83ff11c620ebc6cff648.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

这样就完成了全部的设置流程。你还可以手动调整卡片大小，或是添加其他的信息，比如最后阅读的时间等等。

### 稍后读列表

结合 Obsidian Web Clipper 浏览器插件 和 Bases，我们可以实现一个原生的 Obsidian 稍后读应用。

![screenshot-20250820-214812.png|800](https://cdnfile.sspai.com/2025/08/21/article/d4fdc4644d892d233281e80054da4b10.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

#### 使用 Obsidian Web Clipper 添加稍后读文章

Obsidian Web Clipper 是一个非常强大的浏览器插件，用于将网页内容保存到 Obsidian 仓库中。网上已经有非常多关于它的使用实践，此处不做赘述。

为了实现稍后读功能，我们需要在剪藏文章时添加一个新的属性，用于记录文章「已读/未读」的状态，我自己设置的属性名称是「isRead」，属性类型是「checkbox」。

同时，为了让添加的稍后读文章更加清晰明了，我还使用 Obsidian Web Clipper 的解释器功能，调用 Gemini 2.5 Flash 的 API，智能地为以下属性添加内容：

1.  **title**：{{"如果 title 为英文，则翻译为中文。如果为中文，则直接使用 title"}}
2.  **cover**：{{"使用页面中的第一个图片 URL，如果页面中没有图片 URL，则使用 \[\[../assets/文章剪藏.png\]\]"}}
3.  **description**：{{"使用中文，一句话总结当前 web page 的内容"}}
4.  **tags**：{{"从以下 6 个 tag 中选择最合适的一个：areas/ai,areas/swiftUI,areas/swift,areas/乐趣，areas/理财，areas/社会与文化"}}

在解释器中配置调用大模型 API 的 URL：

1.  [BigModel](https://open.bigmodel.cn/api/paas/v4/chat/completions)（智谱清言）：智谱的 `glm-4.5-flash` 模型是免费调用的，但是速度较慢
2.  [DeepSeek](https://api.deepseek.com/v1/chat/completions)
3.  [Gemini](https://generativelanguage.googleapis.com/v1beta/chat/completions)

Obsidian Web Clipper 模板中的属性设置可以参考下图：

![image.png|800](https://cdnfile.sspai.com/2025/08/21/article/c8e8d6a87d7037cafd77f70abedd4846.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

解释器根据文章内容处理属性的动态效果：

![20250820-214651.gif|300](https://cdnfile.sspai.com/2025/08/21/article/0f7e58e7de68d9227124e355da0691c4.gif)

#### 创建并设置 Bases

由于我们已经在 Obsidian Web Clipper 插件中设置好了属性，因此只需要创建一个新的 Bases，并将过滤条件指定为剪藏文章保存的文件夹，并在「属性」设置中，勾选想要展示的属性即可。

接下来，每当我们使用 Obsidian Web Clipper 剪藏文章，就会自动展示在这个 Bases 中。当我们阅读完一篇文章，只需要在 Bases 中勾选 checkbox，就能快速将其标记为已读。

一套简单的稍后读工作流就这样毫不费力地完成了。

不足之处
----

正如文章开头所说，Bases 是建立在 Obsidian「文件优先」设计理念的基础上，是对现有文章的聚合展示。因而它无法从结构上约束每一个插入数据库的数据（即笔记）都符合数据库规范。

这就对我们创建新笔记提出了更高的要求，需要为每篇新笔记在创建时就设置好属性以及属性对应的值，这样才能在现有的 Bases 中正常展示出来，正确融入工作流中。

除了通过 Obsidian Web Clipper 插件为剪藏的文章预设属性，我还推荐 Templator 这个插件。它可以针对不同的场景设置相应的模板，模板中支持通过脚本来为属性赋值，也可以将模板与文件夹关联，在文件夹中创建文件时自动应用模板。

此外，当前的 Bases 还缺少重要的分组功能，能够设置的视图类型也只有表格和卡片两种。不过在官网的 Roadmap 中，这些功能都已经在开发中，应该很快就会发布了，可以小小期待下。

总体来说，Bases 极大地提升了我们组织和查看非结构化笔记的交互体验，至少对我来说已经够好了，10 分的话我给 8 分🥳。

\> 关注 [少数派小红书](https://www.xiaohongshu.com/user/profile/63f5d65d000000001001d8d4)，感受精彩数字生活 🍃

\> 实用、好用的 [正版软件](https://sspai.com/mall)，少数派为你呈现 🚀
