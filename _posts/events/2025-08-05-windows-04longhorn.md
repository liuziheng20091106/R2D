> id: https://sspai.com/post/89445

> link: https://sspai.com/post/89445

> title: Windows 04Longhorn

# Windows 04Longhorn
_Published on Tue, 05 Aug 2025 07:00:00 GMT_

![Article Cover Image](https://cdnfile.sspai.com/2025/07/15/14b5425c4f1dac39c661c97cdf2b4c5f.png)  

> **也许这是我第一次不知道从哪里开始。**
> 
> ——科技记者 Paul Thurrott，其「通往黄金之路：通往 Windows Vista 的漫漫长路」系列文章，详细记述了 Windows Longhorn & Vista 的开发历程。

前言
--

[上一期文章](https://sspai.com/post/88722)回顾了 Windows 95 - XP 时期 Windows 设计风格的演变历程，提到了当时微软内部出现的扁平化设计趋向，一直到最后 Windows XP 的主要设计风格 Luna 的定型。 对于 Windows XP 在改进设计风格上做出的努力，当时的用户体验团队成员 Hillel Cooperman 曾这样评价 ：

> 从 Windows XP 开始，我们终于看到了微软在美学上的投入。

而 Windows XP 发布后，微软并没有停止对新设计风格的探索，这些都体现在 Windows 的下一版本中——这一代 Windows 的开发堪称传奇：它的开发很艰难，经历了六年的磕磕绊绊，开发到一半还不得不推倒重来；它对 Windows 的意义重大，期间引入了许多创新功能，影响一直延续至今，也是介绍 Windows 历史绕不开的一个版本；它的设计风格则是一变再变，默认主题接连换了好几套；历经了约六年的打磨，最终发布后面对的却是一系列失败……

这些特征交织在一起，让 Windows 的这一段历史尤为复杂，对我来说也是最难写的一期。写得太少则意犹未尽，写得太多又容易散乱失焦。就连本文原定是一直写到 Vista 发布的，但最终还是决定以 Longhorn 重置前/后为界，分成两期写。

那么从哪里开始说起呢？不妨就从一座雪山脚下的小酒廊开始……

> 如未特殊说明，本文所指的「Longhorn 版本」均为重置前版本。

「小酒廊」的蜕变
--------

Windows XP（代号 Whistler）的开发尚未完成，微软便已开始了下一版本 Windows 的规划。

2000 年，微软在 PDC 2000 中展示了 Windows 后续的发展路线图，其中代号为 Whistler 的版本（也就是后来的 Windows XP）计划于 2001 年下半年发布，之后则是代号为 Blackcomb 的、计划于 2002 年下半年发布的新版本。

按照计划，新版本的 Windows 将基于微软新推出的 .NET 框架构建。

![](https://cdnfile.sspai.com/2025/06/10/a394f83b99dd91f6c11007140e7ba77d.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

PDC 2000 中展示的 Windows 路线图

不过在 2001 年 1 月微软的一份内部规划文件中，却出现了名为「Whistler+1」的项目名称，这被认为是 Whistler 后继操作系统版本的临时命名1。原定的 Whistler 和 Blackcomb 之间，又多出了至少一个 Windows 版本。

2001 年 5 月，微软开始规划名为「Longhorn」的 Windows 项目，计划于 2003 年左右推出。在微软最初的设想中，Longhorn 只是 Whistler 与下一代操作系统 Blackcomb 之间的一个过渡版本，就连它的名称也暗示了这一点：Whistler 和 Blackcomb 是加拿大的两座山名（也是加拿大有名的滑雪圣地，微软员工经常前往此处滑雪），而 Longhorn 则是两座山之间一个小酒廊。

![](https://cdnfile.sspai.com/2025/02/11/68d0b186298a0f92ffb8cb15b8229214.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/02/11/8d19df7757a10a2f8d6ba1aea6d30523.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/02/11/45cd81e1ac3fed599e80f0e9b7fde22b.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/02/11/5f0627180750461a81814eb6629acf20.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

按照计划，Longhorn 将基于 Windows Server 2003 的代码库，并且同时有客户端和服务器端两个版本。下图展示了 Longhorn 的开发路线图。

![](https://cdnfile.sspai.com/2025/07/23/64cfa1a615edf9abd37efce79249dabd.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/07/24/6db695ce2697a57255f688e369d2c2f0.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

2002 年 4 月，微软集团副总裁 Jim Allchin 透露 Longhorn 不会在 2004 年之前发布，「我们将有一个合理的开发周期，」他说，「以前我们经常操之过急，把所有时间都花在收集测试版反馈上，而没有像我期望的那样带来足够的创新。」

这是 Longhorn 的首次延期。

4 月的 WinHEC 2002 过后，微软透露 Longhorn 将会包含新的托管接口、图形结构、网络技术以及存储架构等。这意味着 Longhorn 的定位将发生变化，从过渡版本变为了主要版本。而随着 Longhorn 项目的逐渐推进，许多原本规划在 Blackcomb 项目中的功能也被纳入到了 Longhorn 中，致使 Longhorn 项目变得越来越复杂。

2002 年 6 月，微软董事长比尔·盖茨在《财富》杂志的封面文章中称，他将把大约一半的时间投入到 Longhorn 的开发中，并将 Longhorn 的开发形容为「相当于多次登月计划」和对 Windows 的一次「全面检修」，而不只是一次「升级版本」。他向《财富》杂志描述了 Longhorn 的 10 个主要场景，包括人员、注释、实时通信、存储、身份验证和安全，以及新外观等。

![website/blog/editor/media-nofol4k4.jpg](https://cdnfile.sspai.com/2025/07/31/article/30ed8029ee6d2498170a04c9a274821a.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

《财富》杂志封面上的比尔·盖茨

根据规划，Longhorn 的三大支柱计划如下：

-   基于数据库的文件系统 WinFS，当时被称为「安全存储结构化和非结构化数据的下一代数据存储」，实际上是微软 [Cairo](https://betawiki.net/wiki/Microsoft_Cairo) 项目中「对象文件系统」（OFS）的继承；
-   一个基于矢量的全新应用程序界面框架 Avalon（后来更名为 Windows Presentation Foundation，即 WPF），它依赖于 .NET Framework 和 .NET Core ；
-   通讯服务 Indigo（后来更名为 Windows Communication Foundation）。

后两者均属于 WinFX 的范畴，WinFX 是一系列基于 .NET Framework 构建的新类库。除了技术上的改进之外，Longhorn 在 UI 设计上也做出了很大变化。

但最初，我们所熟悉的「Aero」还未上场。

Plex：改变的一小步
-----------

2002 年 11 月 19 日，测试小组 xBetas 公开了 Longhorn 版本 Build 3683，这是目前最早公开有完整镜像的 Longhorn 版本。它采用了一款名为「Plex」的新主题，其窗口边框与 Windows XP 的类似（上方圆角下方直角），但配色有所改变，与 Windows XP 的 Luna 相比色调更为偏暗，样式有点类似于 Windows XP 曾经测试过的「水彩」（Watercolor）主题（可参见[上一期](https://sspai.com/post/88506)），并且采用了居中标题栏。

![](https://cdnfile.sspai.com/2025/07/19/6dca4a3d41f1a980671815304294a1e9.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Build 3683 采用的 Plex 主题

除了桌面外，登录界面也进行了一定的更新，整体布局仍与 Windows XP 相似，只是更换了背景。值得注意的是，登录界面的右上角显示了当前时间（Paul Thurrott 称其为「期待已久」），而这在近十年后才以锁屏时钟的形式重新回归。

![](https://cdnfile.sspai.com/2025/07/31/af50724dd70085db9db96581f53d400c.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/07/24/8e8a8f4e4631bdfe84186b43fdb464d5.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

而在一个 Longhorn 概念演示（见下面视频）里展示了这样的登录界面，它采用了上面提到的 Plex 风格，与 Windows XP 相比已有了很大变化。这个视频还展示了一款经过全新设计的音乐库程序。

![](https://cdnfile.sspai.com/2025/07/31/5ded691bba87d661d64a8590f1792ba9.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/07/31/5fece7e13119953c3d8badcc0b17104c.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

![](https://cdnfile.sspai.com/2025/08/01/29b811263427be0ccd7b3c6d4b04cbd7.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Longhorn 音乐库

 

该版本也包含 Avalon 的初步版本，下图展示了采用 Avalon 编写的显示设置。

![](https://cdnfile.sspai.com/2025/07/31/9056ae802d015a8bbc63c44929e19752.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

采用 Avalon 编写的显示设置

直到下一阶段的 Longhorn 开始开发，大家熟悉的「Aero」才真正露面。

「Aero」初登场
---------

在 Longhorn 项目的开发中，微软引入了一套新的设计风格，名为「Aero」。「Aero」实际上是四个词的缩写：**Authentic（真实）、Energy（能量）、Reflective（反射）和 Open（开放）**。据微软介绍，Aero 的目标是为了释放 Windows 软件的强大功能，以及提供更清晰、更一致的 Windows 界面。

严格来说，Aero 并不单单指设计风格，而是一整套设计语言的总称，包含视觉风格、向导设计、用户通知，甚至包括针对应用程序中指令和其他文本的措辞和语气设计等。

Aero 设计从 Build 4015 开始便有所体现，经过一些设置便可以在该版本中启用带有透明度的窗口边框。据 Aero 团队的首席项目经理 Kam Vedbrat 介绍，采用半透明的窗口边框可以让窗口变得更加轻盈，且富有层次感。

![带玻璃框架的桌面合成发动机](https://cdnfile.sspai.com/2025/07/18/article/8f200ae06f557a007c30d73050c65a40.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Build 4015 中带有透明度的窗口边框

而为了渲染 Aero 的玻璃效果，微软引入了一个窗口管理器：**DCE（Desktop Compositing Engine，桌面合成引擎），**其利用 Direct3D 图形驱动程序进行渲染和着色。一段时间之后，DCE 更名为 DWM（Desktop Window Manager，桌面窗口管理器），至今该程序仍负责 Windows 的窗口渲染。

### Slate 和 Jade

实际上，Longhorn 的重置前版本均不包含名为「Aero」的主题。因为这个时候 Aero 还属于私有主题。但由于系统中留有 Aero 相关的代码，所以仍能通过[特殊方式](https://betawiki.net/wiki/Windows_Aero)启用 Aero 效果。

而那个时期真正作为 Windows 默认主题公开展示的，是 Slate 和 Jade。

Slate 主题于 Build 4042 首次引入，意为「石板」，顾名思义，它的整体风格为黑灰色（如下左图），而右图则是启用 Aero 之后的效果。

![](https://cdnfile.sspai.com/2025/08/01/1c360cdcd434de0e10c4ca7eab94dddc.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/01/2beeee7ef9ac43cca4eb551a5b218199.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Jade 主题于 Build 4066 引入，意为「玉」，从名称中也可以看出，它的风格会更接近 Aero 主题，事实上它也的确基于私有的 Aero 主题。而这个版本可以启用两种 Aero 效果：一种是绿色半透明（如左图），一种是几乎全透明（如右图）。

![](https://cdnfile.sspai.com/2025/08/01/73851f76d80d6cc46d3af95db841d721.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Jade 主题

![](https://cdnfile.sspai.com/2025/08/01/7edada7b2a18f25bb4aa08e59967ff0c.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/01/fe3fc9c411a9dd264f2a3d49322be3f7.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

而 Build 4074 的 Aero 也有其他变化，比如引入了 Flip 3D 窗口切换效果，按下 Win+Tab 后窗口就会以 3D 形式排列。

![Aero done right | Microsoft Longhorn](https://cdnfile.sspai.com/2025/08/01/article/9afac4e16609ced5d7c1f1f5567910bb.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Flip 3D

除此之外，Build 4074 也引入了一套新图标（与正式版较为接近）和 Segoe UI 字体，整体与 Windows XP 和之前的 Longhorn 版本已有很大区别。又由于它是当时为数不多的由微软官方公开的 Longhorn 版本，该版本的知名度也较高，也被一些人认为是「最美的 Longhorn 版本」，也是许多人在体验 Longhorn 项目时选择的初始版本。

> 一个细节：上面两个 Longhorn 版本一个采用了干草地，一个采用了叶丛作为壁纸，其实这也是微软为更好展示 Aero 而精心设计的。据 Windows 团队的设计师 Jenny Lam 解释，这些壁纸「能真正展现玻璃质感。这样，当你用玻璃摩擦叶片时，就能看到折射，还能感受到维度和深度。」微软也希望借此真正反映 Aero**（真实、能量、反射、开放）**哲学。

### Aurora：极光美如画

除了 Aero 之外，Longhorn 还有其他一些独具魅力的设计，比如一个名为「Aurora」的功能，它可以在桌面上显示动态的极光效果。

下图展示了 Longhorn 的极光效果：

![](https://cdnfile.sspai.com/2025/07/15/5cfadfa1b4fb0b9a9a4d17c1305a87fc.gif)

Longhorn 极光效果

![](https://cdnfile.sspai.com/2025/08/01/44b2c7aaa79b399b45b5811487c37611.gif)

Build 4074 上的 Aurora 桌面

这一设计将在之后的版本中进一步拓展，我们下期再讲。

除了 Aero 和 Aurora 之外，Longhorn 还有许多让人眼前一亮的新设计，比如旋转图标，资源管理器的轮播视图等。这些设计在现在看来可能有些花哨，但与当年设计较为简陋的 Windows XP 相比也令人耳目一新，展现出当年 Longhorn 的独特魅力，令人神往。

![](https://cdnfile.sspai.com/2025/07/31/3bf216b13fd2f15e6b408cc210766556.gif)

Longhorn 的旋转图标和轮播视图

### Aero 与 Aqua：真的像吗？

从微软推出 Aero 一直到现在，一个很常见的争论就是它与 Mac OS X 中曾经引入的 Aqua 风格的相似度。我曾翻看过当年的一些讨论帖，但发现其中两极分化比较严重，无法得出真正客观的结论。

而在我眼中，Aero 与 Aqua 确实有一定相似的地方，比如窗口边框和其他一些控件都有一定的透明度，拟物化效果较强等等。但两者确实有一些明显的区别，比如 Aero 的玻璃效果更强，而 Aqua 的按钮等一些控件更接近凝胶风格。

所以对于这个问题，你可以保留自己的看法，而如果你问我这个问题，我的回答是：Aqua 确实与它的名字一样更像「水滴」，但如果问谁更像「玻璃」，我会选 Aero。

![Desktop with applications in Mac OS 10.0.4](https://cdnfile.sspai.com/2025/07/18/article/954a87f442cb03de51d7971e1a5b61f4.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Mac OS X 中的 Aqua

边栏：任务栏的扩展
---------

除了视觉效果外，Longhorn 的桌面环境还引入了一项重大变化，那就是边栏（Sidebar）。在边栏中包含一些部件，用户能在此查看时间、天气等信息或执行一些简单操作。

实际上，在桌面上放置侧边栏这一概念在当时并不新鲜。在 Longhorn 开发的那几年，包含类似功能的程序已是遍地开花，如 Stardock 的 DesktopX、雨滴桌面（Rainmeter）、Konfabulator（之后更名为 Yahoo! Widgets）等。而 Apple 也抢先于微软在 2005 年正式推出了仪表板（Dashboard）小部件。

![](https://cdnfile.sspai.com/2025/07/15/581efc4608bb6bb3e07ffd24f6a97cf9.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/07/15/4fb1fb3e13c31e41d264a82138dbd4f3.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

而微软自己，在 Longhorn 之前也进行过类似侧边栏功能的开发。IE4 的 Windows 桌面更新引入的频道栏（Channel Bar，活动桌面的一部分）可以看作是 Windows 侧边栏的前身。也有人将 Office 和 WinXP 的资源管理器中的任务窗格、MSN 6 中的「我的资料」栏和 MSN 8 中的仪表板视为边栏的早期实现。

![](https://cdnfile.sspai.com/2025/07/15/e599ad418f85faf33044903ed17455bf.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/07/15/4b454f48e6232138cd3a0f7fcbde11a2.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

自 2000 年起，微软研究院便开发了一款名为 Sideshow 的侧边栏程序2，并在微软内部进行测试。这个程序在 PDC 2001 上得到了公开演示。这一时期，微软研究院分别于 2001 年 9 月和 2002 月 8 月撰写了两篇研究报告《[Sideshow：提供对重要信息的外围感知](http://www.microsoft.com/en-us/research/publication/sideshow-providing-peripheral-awareness-of-important-information/?from=https%3A%2F%2Fresearch.microsoft.com%2Fapps%2Fpubs%2Fdefault.aspx%3Fid%3D69878)》《[设计和部署信息感知界面](http://www.microsoft.com/en-us/research/publication/designing-and-deploying-an-information-awareness-interface/)》，其中明确了 Sideshow 的理念是「利用用户的外围感知，帮助人们实时了解信息的同时不过度分散注意力」。

> 用户界面的一个基本问题是如何帮助用户了解信息而不过度打扰或分散注意力。在本文中，我们介绍了 Sideshow，这是一个外围感知界面，旨在帮助用户保持对人和信息的了解。我们提供了 Sideshow 现场试验的数据，其中我们公司的数百名员工在七个月的时间内使用了 Sideshow。数据表明，Sideshow 的设计实现了提供对重要信息的感知而又不会过度分散注意力的目标。
> 
> ——《Sideshow：提供对重要信息的外围感知》

Sideshow 的一个版本于 2002 年被 [WinBeta.org](http://winbeta.org/) 泄露。其中的小部件被称为「小票」（Tickets），自带有邮件，股市，交通等多个部件。当鼠标悬停在这些小票上时，会显示更多详细信息。小部件也可合并形成组。

![](https://cdnfile.sspai.com/2025/07/15/92ea0a4823b40d012f710e7124f70092.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/07/15/1469c5e4e779f4e84c1af17a38ebdbfb.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

在 Longhorn 项目期间，Sideshow 更名为「Sidebar」（边栏），微软将边栏视为「任务栏通知区域的进化」，也可以理解为是任务栏的扩展。而实际上边栏可以与任务栏合并，并且有两种方式，一种是以任务栏为主体，边栏部件最小化为任务栏上的图标（如左图）；另一种是以边栏为主体，任务栏成为边栏中的一个部件（如右图）。

![](https://cdnfile.sspai.com/2025/07/22/2b684d3f433ed3711bcb03d68937594b.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/07/22/7d52257ad549db5526bdd8235b60663f.gif)

边栏中的部件被称为「瓷块（Tile）」3，以 Build 3718 为例，它包含如下部件：

> 时钟、多桌面管理器、应用列表、快速启动栏、搜索、幻灯片、通知中心、用户图块、媒体播放器。

![](https://cdnfile.sspai.com/2025/07/22/article/0b266f527331e899e517c6c2ae9b1b9d.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Build 3718 中包含的部件

随着时间的推移，边栏中包含的部件也越来越多，在微软后来的设想中，用户可以利用侧边栏完成管理联系人，处理电子邮件，进行音量控制等复杂操作，而不仅仅局限于查看信息。

![](https://cdnfile.sspai.com/2025/07/22/face5ffc0288cc5bf6452883818d8c5c.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/07/22/29ee1111eba76ea13742e74037b6422c.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

与此同时，微软也设想对任务栏本身进行重新设计。Build 4015 的任务栏将任务图标（不包括开始按钮）居中，并在右键菜单中新增了「kill」（结束任务）按钮，允许用户在任务栏右键直接结束相关任务（顺便一提，该功能直到 Windows 11 Build 25300（2023 年 2 月 15 日发布）才重新出现）。

![](https://cdnfile.sspai.com/2025/07/31/76009e5197e6d21732fdd14091e63cf2.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Build 4015 的任务栏

![](https://cdnfile.sspai.com/2025/07/31/de165896e4d1d8f705ea2ae4d971df8f.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Build 4015 的任务栏右键菜单中的「kill」按钮

> 花絮：实际上，微软也考虑过对任务栏本身的功能进行扩展。2003 年 1 月起，微软研究院开发了一款名为「GroupBar」的应用程序，其采用的理念类似于现在的浏览器标签页分组，可以将任务分组并进行批量操作。微软将其形容为「任务栏的演进（The TaskBar Evolved）」。该程序现在仍可以在[微软网站](http://www.microsoft.com/en-us/download/details.aspx?id=52453)上下载到，并仍然可以在新版 Windows 上运行。
> 
> ![](https://cdnfile.sspai.com/2025/07/17/article/4cef636da4e74cf4b9cbbccb0b73a8fd.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)
> 
> GroupBar 示例

一鸣惊人
----

2003 年 5 月，在 WinHEC 2003 上，微软首次提及了「Aero」，之后，在 PDC 2003 上，Hillel Cooperman 展示了 Aero 界面，在场的人都惊叹不已，Paul Thurrott 称：

> 这是我见过的最令人印象深刻的技术演示之一，也是唯一一场能与史蒂夫·乔布斯主题演讲媲美的微软活动。

![](https://cdnfile.sspai.com/2025/08/01/5b171803a5ec8c840a7479c5ea0035c8.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

PDC 2003 上演示的 Longhorn

至今我们仍然可以通过视频感受当年让人惊艳的 Aero 界面演示：

 

这也让当时的许多人都期待着一个经过重新设计的 Windows 系统。在 PDC 2003 后，Paul Thurrott 直言：

> 当时我们并没有意识到，PDC 2003 之后，一切都会走下坡路。如果你当时告诉我，在那之后，我们将经历承诺被违背、功能被取消以及毫无进展的境地，我绝对不会相信。在 PDC 2003 上，我们来了，我们见识了，我们坚信不疑。我们畅饮酷爱饮料（Kool-Aid），凝视着温暖而模糊的未来，并为之着迷。然而，这一切最终都未能实现。

难以为继
----

然而，在 PDC 2003 之后，Longhorn 开始逐渐走向下坡路。

随着开发的缓慢进展，以及越来越多的技术或功能的不断加入，Longhorn 项目最终变成了一个臃肿且不稳定的空头支票，开发计划的完成变得遥遥无期，开发团队迷失了方向。团队成员和高层管理人员将该项目描述为一个彻头彻尾的「猪」（pig），发布日期也一再被推迟。

![](https://cdnfile.sspai.com/2025/07/20/369780cbba6d2f59717a15a2c49f4da9.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

2004 年 2 月 Longhorn 内部性能和可靠性演示的幻灯片强调了该项目的迅速恶化，其中将 Longhorn 称为「猪」

而 Longhorn 也面临着内存泄漏和系统崩溃等稳定性问题，以及功能膨胀、新技术完成度不高等开发问题，这些问题随着开发的进展而日益严重，项目最终进入了**开发地狱**。作为最后的手段，微软开始着手将操作系统进行组件化重构，希望能够控制功能膨胀。然而，组件化工作却进一步拖累了项目。Longhorn 项目已很难再推进。

而 Apple 也利用这个机会，在 WWDC 等活动中对 Longhorn 极尽讽刺之能事（更多信息可参阅我之前的[文章](https://sspai.com/post/89448)）。2004 年，Apple 推出的 Mac OS X Tiger，其中确实包括许多 Longhorn 正在开发的功能（比如仪表板小部件等），这对微软来说是不小的挑战。

![](https://cdnfile.sspai.com/2025/07/02/7acb4c00d180b9a87b86c22cc355b28a.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

WWDC04 会场展板《Introducing Longhorn》

微软无意间重走了 Apple 的老路：Longhorn 渐渐变成了微软版的 [「Pink」项目](https://sspai.com/post/60696)。

> 人类唯一从历史中吸取的教训就是人类从来不会吸取教训——黑格尔

与此同时外部环境也不轻松。2003 年 8 月，随着冲击波和震荡波病毒的全球爆发，以及 Windows XP 经常出现安全漏洞以及易受恶意软件、电脑病毒、缓存溢出等问题，微软陷入严重信任危机。在 2004 年的 TechEd 上，鲍尔默表示，「为了解决 Windows XP 的安全性问题，我们不得不将 Longhorn 的优先级降低。」最终，Windows XP SP2 于 2004 年 8 月顺利推出，然而 Windows XP SP2 的开发也使得 Longhorn 的开发计划被严重延误。

2004 年 4 月中旬，有传言称微软力不从心，将缩减 Longhorn 的功能集。《商业周刊》在 2004 年 4 月 19 日报道称，微软将「放弃一些最雄心勃勃的功能，以便在 2006 年之前推出已经推迟的 Windows XP 后续版本」；WinFS 的功能将被缩减，使其仅在本地系统上提供文档索引而不是通过网络；此外下一个 Office 版本（Office 2007，当时称为 Office 12）将设计为兼容 Longhorn 和之前的 Windows 版本，而不仅仅是 Longhorn。

当时微软首席产品经理格雷格·沙利文 (Greg Sullivan) 表示，Longhorn 功能的削减是为了「在不牺牲产品核心功能的情况下实现 Longhorn 的愿景」。

2004 年 5 月，在 WinHEC 2004 大会上，微软公开展示了上文提到的 Build 4074。Build 4093 则新增了基于 Avalon 的 Windows Movie Maker，这是重启计划前的最后一个版本。

![](https://cdnfile.sspai.com/2025/08/01/e922c4e996566dfea863717de18573dd.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

按下「重置」键
-------

2004 年 8 月，在解决了 Windows XP 安全问题之后，微软决定重启 Longhorn 开发进程，并计划在 2006 年正式发布 Longhorn 客户端操作系统，新代码库将基于 Windows Server 2003 SP1。Jim Allchin 也大刀阔斧地进行了改革，力求使开发计划更快完成。

按照新计划，WinFS 将脱离 Windows，作为可下载的数据框架发布。（最终，WinFS 于 2006 年取消，多年之后，比尔•盖茨称 WinFS 是他「**对微软产品最大的遗憾**」）。而其他一些 Longhorn 开发者功能将被移植到之前的 Windows 版本。「微软还宣布，WinFX 开发者技术，包括代号为 Avalon 的新演示子系统和代号为 Indigo 的新通信子系统，将于 2006 年在 Windows XP 和 Windows Server 2003 中推出。至于 Longhorn 服务器版本，预计仍将在 2007 年推出。」

Longhorn 项目，重新开始了。

如果……
----

看完上文，你是否对 Longhorn 项目的重置感到惋惜？事实上有这种想法的不止你一个人。在 Longhorn 重置之后，仍有一些个人和组织试图恢复重置前的 Longhorn 项目。比如，2007 年，Joejoe 论坛上的一个团队发起了一个名为「Longhorn Reloaded」的项目，它基于 Windows Longhorn 4074 版本，但稳定性比 Build 4074 有了一定提升。但微软最终发现了这个项目，并发出了一封勒令停止的信函以将其下架。与之类似的 Longhorn 修改项目还有 [SigmaOS](https://crustywindo.ws/Sigma_OS) 等。

![Winver](https://cdnfile.sspai.com/2025/08/01/article/573c46b41bff279c67d014bb106ab85e.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Longhorn Reloaded

如果 Longhorn 项目没有被重置，而是按照计划顺利进行下去，现在的 Windows，乃至个人电脑，又会是什么样的呢？时光自然无法倒流，但我们可以通过当时的一些相关资料来一探当年微软对 Longhorn 的设想。

据用户体验企业家 Long Zheng 介绍，一家位于旧金山的工业设计公司 [Ammunition](http://www.ammunitiongroup.com/) 4曾经负责为微软提供计算机设计图，在此之后这些设计图在其网站上公开。我们能透过这些设计图看看微软对 Longhorn PC 的理解。

![微软氧气](https://cdnfile.sspai.com/2025/08/01/article/a0646b4f9033930c88ebc70f1e46417f.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

微软 Oxygen 概念桌面系统，可从常规使用模式切换至媒体观看模式，也支持手写笔输入

![微软锌](https://cdnfile.sspai.com/2025/08/01/article/53ee9f441edd4d33309dc5cbe6bb7d3a.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

用于工作台的 Microsoft Zinc 概念

![微软 Carbon](https://cdnfile.sspai.com/2025/08/01/article/890668b79d533c2106f1af3f949645a4.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

微软 Carbon 概念微型电脑

![微软 Argon](https://cdnfile.sspai.com/2025/08/01/article/8c939915b186797fe6c2c0131a8bc34b.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

微软 Argon 概念，偏向娱乐功能的一体机

![微软钴](https://cdnfile.sspai.com/2025/08/01/article/b6336eb68c5d43345c1f06a3832a6b85.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Microsoft Cobalt 可转换笔记本/平板电脑

除了设计图之外，当年微软还做了一些视频演示，感兴趣的朋友可以到文章末尾进行观看，管窥当年 Longhorn 的设计理念。

写在最后……
------

对我来说，Longhorn 对 Windows 来说是个非同一般的存在。我之前就是被 Longhorn 吸引才真正对 Windows 的测试版本感兴趣的。因为 Longhorn 除了让我了解到了一个系统的开发历程，还让我感受到了，这其中蕴含了太多的希望，也有太多的遗憾。

当你真正了解了 Longhorn 的开发历程并体验过其中几个版本后，你会不禁感叹，「原来 Windows 还有这样一段不寻常的历史」，而如果没有 Longhorn，Windows 的开发史也将会无趣很多。

正如 Long Zheng 所说，

> 有时候我觉得微软就像电影《夺宝奇兵》里那样，维护着一个仓库，把所有被抛弃的想法都堆放在里面。这很遗憾，因为外人永远无法理解最终产品的诞生过程。据我所知，Longhorn 诞生时，就有成千上万个类似的概念被提出，最终才有了 Vista。

而最初的 Longhorn 虽然折戟沉沙，但它当初放弃的一些设计也出现在了后面的 Windows 中，比如登录界面的时钟、任务栏上的虚拟桌面5、通知中心等。Longhorn 也确实如 Long Zheng 所说，如同一个宝库，源源不断地如今的 Windows 提供着灵感。

下一期：新生
------

关于 Longhorn 可讲的还有很多，但受限于篇幅本文只能到此为止了，而 Longhorn 在重置之后也将迎来新的开始。

当 Longhorn 摆脱了「开发地狱」之后，她又会以怎样的姿态呈现呢？而面对这一「新」项目，微软为她起了一个足以体现当年 Longhorn 雄心和远见的名字：**Vista（远景）**。

到下期，我将继续向大家讲述关于 Longhorn & Vista 的后半生。

更多 Longhorn 概念演示
----------------

  

参考资料（主要）
--------

1.  [Windows Vista - 维基百科（英文）](https://en.wikipedia.org/wiki/Windows_Vista)
2.  [Windows Vista - betawiki](https://betawiki.net/wiki/Windows_Vista)
3.  [Windows Longhorn - betaarchive](https://www.betaarchive.com/wiki/index.php?title=Windows_Longhorn)
4.  [传奇诞生 – Windows Vista 开发历程 - 一维天地](https://www.iwstech.com/blog/24)
5.  [Paul Thurrott - 通往黄金之路：Windows Vista 的漫漫长路（第一部分：2001-2002 年）](https://www.itprotoday.com/windows-server/road-to-gold-the-long-road-to-windows-vista-part-1-2001-2002)
6.  [微软 Longhorn 项目（longhorn.ms）](https://longhorn.ms/)
7.  [istartedsomething | Long Zheng 的博客](https://istartedsomething.com/)
8.  [Windows Aero - 维基百科（英文）](https://en.wikipedia.org/wiki/Windows_Vista)
9.  [Windows Aero - betawiki](https://betawiki.net/wiki/Aero)
10.  [Slate 主题 - betawiki](https://betawiki.net/wiki/Slate)
11.  [Jade 主题 - betawiki](https://betawiki.net/wiki/Jade)
12.  [Lucas Brooks 的推文](https://x.com/mswin_bat/status/1406130295523315717)
13.  [您觉得 Windows Vista Aero 看起来像 Mac OS X Aqua 吗？- neowi](https://www.neowin.net/forum/topic/540441-does-windows-vista-aero-look-like-mac-os-x-aqua-to-you/)n
14.  [Windows Sidebar - betawiki](https://betawiki.net/wiki/Windows_Sidebar)
15.  [比尔·盖茨对微软产品最大的遗憾：WinFS - ZDNet](https://www.zdnet.com/article/bill-gates-biggest-microsoft-product-regret-winfs/)
16.  [Windows Longhorn Reloaded 项目介绍](https://crustywindo.ws/Windows_Longhorn_Reloaded)

\> 关注 [少数派公众号](https://sspai.com/s/J71e)，解锁全新阅读体验 📰

\> 实用、好用的 [正版软件](https://sspai.com/mall)，少数派为你呈现 🚀
