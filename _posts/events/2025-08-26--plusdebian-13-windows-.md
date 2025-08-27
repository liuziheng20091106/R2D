> id: https://sspai.com/post/102104

> link: https://sspai.com/post/102104

> title: PlusDebian 13 Windows

# PlusDebian 13 Windows
_Published on Tue, 26 Aug 2025 09:09:48 GMT_

![Article Cover Image](https://cdnfile.sspai.com/8/26/2025/article/e03c5ed7-52e1-631f-ad32-f241f77e74e0.jpeg)  

Debian 13 一些有趣的新特性
------------------

[@PlatyHsu](https://sspai.com/u/platyhsu)：一个新操作系统的发布，通常会带来一些肉眼可见的新东西：新的桌面壁纸、更漂亮的图标、某个你从来不用的应用推出了新功能。但作为支撑许多服务器运行、一向以稳定保守著称的关键发行版，Debian 的更新更像是一次无聊的但重要的建筑维护工程。最近，Debian 13（代号 Trexie）正式发布了，[完整的更新日志](https://www.debian.org/releases/trixie/releasenotes)很长，这里挑选三条或许不是最显著、但在我看来很有趣的更新点来聊聊。

### 提前化解「2038 年问题」

在类 Unix 系统（包括 Linux）中，`time_t` 是用于表示当前日期时间的类型，可以理解为计算机的「时间戳」。传统上，在 32 位系统中，`time_t` 用一个 32 位整数表示，存储自 1970 年 1 月 1 日以来的秒数。因此，它能覆盖的最大日期是 2038 年 1 月 19 日凌晨 03:14:07（UTC）。下一秒，这个整数就会「溢出」，从最大正数变成最小负数，使得计算机认为时间倒流回了 1901 年 12 月 13 日。——这就是「2038 年问题」，有点类似当年的「千年虫」（Y2K），只不过这次出问题的不是日历年份格式，而是系统计时器。

Debian 13 的一项关键任务就是未雨绸缪地解决这个隐患，在面向 32 位平台编译的版本上也改用 64 位的 `time_t` 类型。这样一来，时间计数器可以表示极其遥远的未来，不仅不会在 2038 年后「爆表」，地球恐怕还没等到下次计时溢出就已经不存在了。

这项工作听起来很简单，但实际上已经开展了很多年。难点在于 `time_t` 被用在了系统的角角落落。统计发现，在 Debian 维护的全部三万多个软件包里，有超过六千个都用到了 `time_t`。要解决 2038 年问题，不能只改其中一部分，因为软件包之间存在相互依赖关系：一个为 32 位时间标准编译的程序，没法和一个使用 64 位时间标准的系统库正常对话。所以，Debian 项目把整个软件仓库里几乎所有的软件包（超过 90%）都重新编译了一遍。

不过也有一项例外：老旧的 i386 架构（32 位 PC）由于主要用于运行遗留软件，经过一番（[不乏争议](https://lwn.net/Articles/938149/)的）讨论，并没有切换到 64 位 `time_t`，因为这会直接破坏旧版软件的兼容性，而那些软件几乎不可能再主动适配 64 位时间。事实上，Debian 13 已经不再提供完整的 i386 支持；官方干脆建议还在跑纯 i386 的用户别升级，用不了多久这架构也要退休了。

### 老牌包管理器新潮改版

十年前，有一位叫做 Joey Hess 的开发者给 Debian [提交](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=755088)了这样一个 bug：

> apt 很多时候是由用户主动使用 \[而不是通过脚本以编程方式使用\]，因此容易犯错。一个常见的错误似乎是，执行 apt-get dist-upgrade 时，没有注意到它准备移除你的备份系统、终端模拟器，或者 Steam。又或者没有注意到它准备安装大得出奇的软件或者 Steam。这种通知被埋藏在大量信息中，可能只是匆匆掠过，甚至转眼就被刷屏出终端窗口。\[…\] 所以，我建议将最重要的项目排序放在最后，以配合现在已经有的加粗强调。

这个 bug 一改就是……11 年。Debian 13 附带的 APT 是经过大版本更新的 3.0 版，其中最直观的改变就是提示信息的呈现：当你运行 apt install 或 apt remove 时，终端输出现在有颜色区分了。新安装的包是绿色的，要删除的包是红色的，并且根据 Hess 的提议放在最后以示强调。除此之外，各类提示之间也用空行更明确地区分开，并且软件包的名称之间分列对齐，而不是只用一个空格分开。这让你在按下 Y 之前，能更清楚地知道自己到底在干什么。

![](https://cdnfile.sspai.com/2025/08/26/f412073b7de2c9e6211af87fbc2f194a.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

与更清晰的信息呈现搭配，APT 3.0 还包含了新的依赖求解器 [solver3](https://blog.jak-linux.org/2024/05/14/solver3/)。简单来说，它在面对复杂的安装和升级操作时更容易给出「可行解」，在面对在大版本升级时，能产生更「干净」、更接近全新安装的系统状态。

最后，Debian 13 也转向了一种新的软件源格式。老用户应该对类似这样的两行字非常熟悉：

```
deb http://deb.debian.org/debian/ trixie main contrib non-free non-free-firmware
deb-src http://deb.debian.org/debian/ trixie main contrib non-free non-free-firmware
```

这是 `/etc/apt/sources.list` 文件定义软件源的语法。其中，第一行具体指的是从地址 `http://deb.debian.org/debian/` 加载 deb（预编译）类型、面向 Debian 13 (Trixie) 稳定版系统的软件包，并且包含所有四种[组件](https://wiki.debian.org/SourcesList#Components)下的包；第二行基本类似，但加载的是 `deb-src`（源代码）类型的包。

这种语法虽然结构简单，但既不易读也不易用程序解析（因为每行只有空格分割的值，无法提前通过列数或者字段名知道每一个值是哪项配置），软件源多了还会让 `sources.list` 变得非常混乱。

而从 Debian 13 开始，官方推荐的是这样一种称为 [Deb822](https://repolib.readthedocs.io/en/latest/deb822-format.html)（得名于其对 [RFC822](https://datatracker.ietf.org/doc/html/rfc822) 的借鉴）的语法：

```
Types: deb deb-src
URIs: https://deb.debian.org/debian
Suites: trixie
Components: main contrib non-free non-free-firmware
Architectures: amd64
Enabled: yes
Signed-By: /usr/share/keyrings/debian-archive-keyring.gpg
```

除了信息呈现更清晰外，可以注意到现在有更多的可配置项（如启用状态 `Enabled: yes/no`、处理器架构 `Architectures:`、签名密钥 `Signed-By:`）。特别是 `Signed-By:` 这项配置，避免了之前为了添加新的软件源，需要将其密钥加入全局钥匙串（`wget -qO - https://example.com/key.gpg | sudo apt-key add -`）的潜在不安全操作，改成了一个密钥只用于验证一个软件源。

不过，Debian 13 终究还是没有默认启用 Deb822 格式（尽管有过这样的主张）。如果想要手动切换，可以 root 身分运行

```
apt modernize-sources
```

即可自动备份并转换现有的 `sources.list`。

### 临时文件放进内存

`/tmp` 目录是 Linux 系统中供各程序存放临时文件的地方。传统上，这个目录位于硬盘上。但近年来，包括 Ubuntu 和 Fedora 在内的很多发行版早都默认采用 tmpfs 来挂载 `/tmp`。tmpfs 则是一种基于内存的临时文件系统，换言之，这些发行版把临时文件直接存放在内存里（必要时可交换到虚拟内存），不写入磁盘。这种做法的优点是显而易见的：在重启后所有临时文件都会自动消失，不会占据磁盘空间、也无需人工清理；而且读写操作直接在内存完成，比在磁盘上快得多，还有助于写入次数有限的 SSD 寿命。

（作为对比，macOS 通过一个每日运行的守护进程 `com.apple.tmp_cleaner` 调用位于 `/usr/libexec/tmp_cleaner` 的终端脚本，定期删除 `/tmp` 下所有创建时间、访问时间和修改时间均过去三天的临时文件。）
