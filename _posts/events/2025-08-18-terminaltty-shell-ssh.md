> id: https://www.appinn.com/terminal-tty-and-shell/-full

> link: https://www.appinn.com/terminal-tty-and-shell/

> title: TerminalTTY Shell SSH

# TerminalTTY Shell SSH
_Published on Mon, 18 Aug 2025 05:58:46 +0000_

**本文由 iShell Pro 赞助，这是一款带有AI功能的跨平台免费 SSH 工具**

[可以点击直接跳转至 iShell Pro 介绍](https://www.appinn.com/terminal-tty-and-shell/#ssh-%E5%AE%A2%E6%88%B7%E7%AB%AF%E4%BB%8B%E7%BB%8D%EF%BC%9Ai-shell-pro)

tty 到底是谁？
---------

如果你在 macOS、Linux 终端中，见过这个画面，并对 ttys 好奇过的话，那么就一起来研究下，这个 tty 到底是谁？ 😂

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 1](https://do-cdn.appinn.com/static3/images/2025/08/Copy-of-appinn-homework-2025-08-13T170203.597.jpg "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 1")

计算机中，有这样几个概念，青小蛙一直弄不清楚终端（Terminal）、TTY、Shell，甚至还有 SSH，就仔细研究了一下。

终端（Terminal）
------------

终端（Terminal）可以是物理设备，也可以是运行在计算机中的软件。

-   简单的说，终端就是人类操作计算机的那个界面，比如电传打印机。
-   终端的功能主要是**转录（打印或显示）数据**，同时负责**输入数据**给计算机。

### 上古时期：电传打字机

最早的终端是电传打字机（Teleprinter），它有一个键盘，可以自动将输入的字符转换为电信号发送出去，同时也能接收信号并打印到纸上。早在19世纪末就被用作电报业务使用。

随着 20 世纪 50 年代早期计算机的发展， 电传打字机被改装成计算机的输入设备，某些电传打字机型号还可以用于制作穿孔纸带以存储数据。

最著名的电传打字机是 Teletype Model 33，配有穿孔带读取器和打孔器，甚至可以用作计算机终端：

Teletype Model 33 是首批采用新标准化 ASCII 字符编码方法的产品之一，该方法于 1963 年首次发布。 由于价格低廉且兼容 ASCII，33 型电传打字机得到了广泛的应用，其大量销售强烈影响了 20 世纪 60 年代制定的几个事实上的标准。包括：

-   ASCII 码作为基础字符集的普及
-   XON/XOFF 软件流控的应用（被广泛采用为串行通信中的软件流控协议）
-   串行通信接口参数及波特率的统一（串口通信接口的标准化）
-   使用穿孔纸带作为数据介质的标准化

随着图形界面出现，物理终端被软件终端仿真器替代。

### tty：Teletype 的缩写

由于 Teletype 公司的产品太出名，以至于可以将 Teletype（或 Teletypewriter）直接翻译为电传打字机，缩写 tty。Unix 系统诞生时，电传打字机仍是主要的终端设备，从而沿用了“tty”。

随着计算机技术发展，尤其是显示器的出现，物理电传打字机逐渐被**虚拟终端**和**软件终端仿真器**所取代。“tty”这一名称和概念随着计算机终端硬件和软件的发展得到保留和扩展，成为 Unix/Linux 内核中所有终端接口的抽象名称，既致敬历史，也实用便捷。

在现代类 Unix 操作系统中，终端设备的输入输出通过 tty 传递给系统。tty 位于终端和 Shell 之间，负责处理字符流的传输和基本控制，使终端与 Shell 通信（关于 Shell 在后面解释）。

你可以看到 `/dev` 路径下有着一大堆的 tty\* 文件，这些文件就是 Unix/Linux 系统中所有“终端”的接口。

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 5](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201628%20882'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 5")

你还可以在终端中执行 tty 命令查看你当前 Shell 具体所对应的终端设备（文件）。

### 现代计算机：虚拟终端

虚拟终端（Virtual Terminal） 是为了实现多用户、多任务环境产生的，系统内核允许在一台物理机上模拟出多个独立的终端会话，它是物理终端的扩展，使有限的硬件资源得以高效利用，在没有图形界面的环境下管理多个任务。

回到最开头的截图中，Last login: Thu Aug 14 13:34:06 on ttys005 表示上一次登录的时间是8月14日13:34:06，ttys005 是那个登录会话所使用的终端设备名，而该终端设备对应的设备文件是 /dev/ttys005。

每打开一个新的终端窗口，系统会分配一个新的 ttys 设备编号。

### 现代计算机：软件终端仿真器

今天的终端仿真器可以简单的理解为 Linux、macOS 系统中的终端应用，也属于终端的一种：

而之前提到的 tty，也可以看作是终端与计算机之间沟通的桥梁：

用户输入/显示  
↓  

终端设备（Terminal）

  
↓  

tty（内核字符设备接口，传递输入输出和控制）

  
↓  

Shell（命令行解释器，解析执行命令）

  
↓  

操作系统内核（执行命令，管理资源）

参考连接：

Shell 是一个软件类别
-------------

Shell 是操作系统内核的外壳，负责解析由终端通过 TTY 传递来的命令并执行。Shell 接收用户输入的命令，将其转化成操作系统可以执行的动作，执行后把结果返回给终端显示。

就像有 Chrome、Firefox、Safari 等不同的浏览器一样，Shell 也有不同的软件，常见的有：

Shell名称

主要特点

**bash**

Bourne Again Shell，是Linux系统默认的Shell，兼容传统Bourne Shell，有命令行编辑、历史记录和自动补全等丰富功能，是最常用的Shell。

**sh**

Bourne Shell的简称，是Unix最初的Shell，在许多系统中常作为bash或其他Shell的符号链接，常用于脚本编写，移植性好。

**csh**

C Shell，语法类似C语言，有较多内部命令，特点是类似C语言的语法结构，但现代使用较少，已基本被tcsh替代。

**tcsh**

csh的增强版本，兼容csh，增加了命令行编辑、命令补全等功能，部分Linux发行版和Unix系统仍支持。

**ksh**

Korn Shell，兼容Bourne Shell，兼具csh的易用特性，脚本编写广泛使用，功能较强，是很多Unix系统的默认Shell之一。

**zsh**

功能最丰富的Shell之一，结合了bash、ksh、tcsh等多种Shell的特点，支持强大的脚本编写能力和交互式功能，macOS Catalina以后默认Shell是zsh。

**ash**

一个轻量级的Shell，功能相对简单，内存占用小，常用于资源受限的环境或嵌入式系统。

**fish**

现代交互式Shell，突出用户友好性和现代化脚本语法，支持自动建议和语法高亮，适合交互使用。

**nologin**

非交互式Shell，主要用于禁止用户登录。

SSH 协议：安全的连接到远程计算机
------------------

当我们需要远程访问计算机的时候（比如服务器机房、NAS 设备、虚拟机等），需要让远程计算机知道你是谁，又不能泄漏你和远程计算机的操作（比如密码），必须有一个**安全的方式**，这个方式就是 SSH 协议。

而这种通过 SSH 协议连接远程计算机的软件，一般叫做 SSH 客户端、SSH 工具，比如本文的赞助商 **iShell Pro**，就是一款带有 AI 功能的跨平台免费 SSH 工具。

iShell Pro – 高颜值跨平台 SSH 客户端
---------------------------

论颜值，iShell Pro 还是有的一拼：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 7](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201560%20975'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 7")

### 自定义主题配色

iShell Pro 支持自定义主题配色，先在设置中选择一个喜欢的颜色，再让 AI 生成一张二次元图片，设置一个合适的透明度，就成了独一无二的终端：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 8](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201558%20975'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 8")

### 漂亮的终端界面

先来看一下设置了背景图片，连接到远程服务器之后的样子：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 9](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201640%201029'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 9")

iShell Pro 比常见的 SSH 工具多了许多内容，包括：

-   显示系统信息的侧边栏
-   左下角的小工具栏
-   右下角的系统监控栏

在这里，不再是上古终端界面了，它突然变得有血有肉，有画面感，甚至有一种每天都要打开的期待。

（这张背景图有同学想要吗？）

### 管理多台服务器

iShellPro 非常适合同时管理多台服务器，你可以为每台远程设备添加**文字备注**、使用**分组管理**：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 10](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201550%20967'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 10")

如果你需要在办公室电脑、家用电脑、手机等不同的设备间管理这些服务器，那么还能通过**云同步**功能，将所有的远程服务器信息同步到云端之中，再也不会出现回家找不到某一台服务器的情况了 😂

而对于云同步的安全担心，iShellPro 需要一个**同步密码**，用来加密你的服务器信息，再上传云端。

这可以保证服务器信息本身不会在云端泄漏，保证安全：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 11](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%20856%20406'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 11")

### AI 助手 && 快捷命令输入提示

AI 时代的 SSH 客户端，最大特点就是有人帮你解释命令行了。

iShellPro 中有一个**快捷命令输入提示**功能，打开后，就能在输入**中文**的时候，出现AI菜单了：

iShellPro 会自动将中文指令转换为合适的命令行，回车输入。

而如果本身输入的是英文命令，则会出现另外的菜单，包括**自动补全**和**中文命令解释**：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 12](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201530%20800'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 12")

甚至你可以在输入一段命令之后，选择 AI 查询，它还会告诉你这段命令是什么意思，非常方便。

青小蛙觉得这个有点点方便，用**中文操作**这件事，似乎就这样曲线实现了。

而当你在终端中遇到问题，不知道该怎么办的时候，选中错误提示内容，右键选择**问问小i助手**：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 13](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201986%20871'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 13")

iShellPro 就会帮你查询这个错误的解决方案：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 14](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%20918%201110'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 14")

### 笔记（支持 markdown）

iShellPro 自带了笔记功能，可以方便的进行记录。目前支持富文本笔记和 markdown 笔记，还支持分组管理。

关于记录笔记，青小蛙有过体验，曾经折腾过某些软件的安装，时间久了以后…就不会装了，真不会了。

而这个时候群里的小伙伴就说：好记性不如烂笔头，你得记笔记…我以前，也不懂啊。

甚至还有一些小脚本，也不知道是什么时候折腾的，谁写的，反正一直能用。但如果碰到迁移服务器、搬家等操作，就很容易丢掉…

这个时候，如果你有笔记：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 15](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201086%20676'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 15")

听劝，把你平时常用的不常用的都记录下来…

### 录制功能

iShellPro 有一个录制功能，可以录制你输入的命令与屏幕反馈：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 16](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201572%20968'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 16")

并且，这个内容会保存为文本文件，如果你想要制作教程、分享所有的操作，比录屏方便、更节省资源。

### 快捷指令 && 命令市场

对于更常用的命令，可以使用 iShellPro 的快捷指令功能，随用随取：

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 17](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201578%20975'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 17")

而 iShellPro 的命令市场中，则有一些其他用户上传的命令，下载后也会出现在上图侧边栏**快捷命令**区域。

### 持续更新 && 新功能

iShellPro 自去年发布以来，已经经历了19个版本，有了不少新功能。

![终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 18](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201068%201506'%3E%3C/svg%3E "终端（Terminal）、TTY 和 Shell，还有 SSH，一次搞懂它们到底是什么？ 18")

今年 2.0 版本以来，就增加了 20 多项功能：

1.  增加串口功能
2.  增加SFTP权限编辑
3.  增加主题配色
4.  增加文件夹上传
5.  增加AI命令翻译
6.  增加跳板机
7.  增加流量监控网卡选择
8.  增加远端同步记录删除
9.  增加会话录制
10.  增加自定义背景及透明度
11.  增加智能提示历史命令
12.  增加断线提醒
13.  增加回车重连
14.  增加MFA二次验证功能
15.  增加MarkDown格式笔记
16.  增加空密码登录
17.  增加同步密码删除功能
18.  增加文件拖拽上传功能
19.  增加主机列表排序功能
20.  增加SFTP右键删除功能
21.  新增快捷命令发送到所有窗口

### 基础功能永久免费使用

iShellPro 基础功能永久免费使用，支持离线使用。

目前的 Pro 功能主要是云同步、AI 相关功能，还有上面提到的**快速命令输入提示**功能。

获取
--

如果你需要一款漂亮的、现代化的、带有AI功能的跨平台 SSH 客户端，不妨试试 iShellPro：

* * *

#[它们到底是什么](https://www.appinn.com/tag/%e5%ae%83%e4%bb%ac%e5%88%b0%e5%ba%95%e6%98%af%e4%bb%80%e4%b9%88/)
