> id: https://www.appinn.com/synocommunity-synocli-packages/-full

> link: https://www.appinn.com/synocommunity-synocli-packages/

> title: SynoCli SynoCommunity NAS 110

# SynoCli SynoCommunity NAS 110
_Published on Mon, 11 Aug 2025 04:45:03 +0000_

**SynoCommunity** 是一个开源社区，维护了大约 131+ 套群晖 DSM 系统第三方开源套件，只需要将源添加至套件中心即可，即开即用。而 **SynoCli** 则是 **SynoCommunity** 自己提供的 7 个套件，用来方便的为群晖 DSM 系统安装如 tmux、screen、mtr、rsync、nano 等命令，总计超过 110 款小工具。主要为开发者使用。@[Appinn](https://www.appinn.com/synocommunity-synocli-packages/)

![SynoCli - 来自 SynoCommunity，为群晖 NAS 安装 110+ 款开发者工具 1](https://do-cdn.appinn.com/static3/images/2025/08/Copy-of-appinn-homework-2025-08-11T124025.406.jpg "SynoCli - 来自 SynoCommunity，为群晖 NAS 安装 110+ 款开发者工具 1")

第一步：安装 SynoCommunity
--------------------

首先需要在群晖套件中心添加套件来源：

-   名称：**SynoCommunity**
-   位置：**https://packages.synocommunity.com/**

具体教程可以参考这篇文章：[https://www.appinn.com/synocommunity/](https://www.appinn.com/synocommunity/)

第二步：选择安装 SynoCli 套件
-------------------

添加好 **SynoCommunity** 之后，就可以在套件中心搜索 **SynoCli** 来选择性安装了：

![SynoCli - 来自 SynoCommunity，为群晖 NAS 安装 110+ 款开发者工具 2](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%202172%201472'%3E%3C/svg%3E "SynoCli - 来自 SynoCommunity，为群晖 NAS 安装 110+ 款开发者工具 2")

具体套件内容如下：

### 1\. SynoCliNet（网络工具）

-   nmap（含ncat, ndiff, nping）
-   netcat
-   tmux
-   screen
-   sshfs
-   socat
-   fritzctl（已移除）
-   ser2net
-   arp-scan
-   links（文本浏览器）
-   imapfilter（邮件过滤）
-   mtr（网络诊断）
-   etherwake（WOL唤醒）
-   telnet & whois（来自inetutils）
-   dig, mdig, delv, arpaname（来自ISC BIND）
-   rsync
-   xxHash（高速哈希算法）

### 2\. SynoCliFile（文件工具）

-   less
-   tree
-   jdupes
-   fdupes
-   rhash
-   mc（Midnight Commander）
-   nano
-   micro
-   rnm
-   file
-   fzf（fuzzy finder）
-   detox
-   rmlint
-   ripgrep（rg）
-   zstd
-   lzip/plzip
-   pixz
-   fd（fd-file）
-   mg（Micro GNU emacs）
-   bat
-   eza（替代exa）
-   lsd（LSDeluxe）
-   jupp
-   nnn
-   iconv
-   dos2unix
-   xstow
-   patch

### 3\. SynoCliDevel（开发工具）

-   automake
-   autoconf
-   binutils（含ld, as, gold）
-   gdb
-   libtree
-   LLVM
-   m4
-   make
-   pkg-config
-   strace

### 4\. SynoCliDisk（磁盘工具）

-   e2fsprogs
-   fuse
-   TestDisk
-   ncdu
-   davfs2
-   lsscsi
-   dar
-   ddrescue
-   duf
-   gdu
-   dua
-   dutree
-   tdu
-   s3backer
-   smartmontools（含smartctl7, smartd）
-   mergerfs
-   disktype
-   gpart

### 5\. SynoCliKernel（内核工具）

-   usbserial
-   linuxtv
-   cdrom.ko
-   sr\_mod.ko

### 6\. SynoCliMonitor（监控工具）

-   busybox（含iostat, pgrep, pmap, watch, pstree）
-   ionice
-   lsof
-   nmon & njmon
-   iperf2
-   iperf3
-   htop
-   cpulimit
-   bandwhich
-   btm（bottom）
-   procs
-   net-snmp（命令行工具）
-   lm-sensors

### 7\. SynoCliMisc（杂项工具）

-   bc
-   expect
-   uhubctl
-   errno（来自moreutils）
-   ifdata
-   ifne
-   isutf8
-   lckdo
-   mispipe
-   parallel
-   pee
-   sponge
-   ts
-   cal（来自util-linux）
-   col
-   colcrt
-   colrm
-   column
-   findmnt
-   hardlink
-   hexdump
-   lsblk
-   lscpu
-   lsipc
-   lsirq
-   rev
-   wall
-   whereis
-   zramctl

通过 SynoCli 套件安装这些开发工具的好处是不需要自己直接折腾 DSM 系统，减少风险。

获取
--

* * *

原文：https://www.appinn.com/synocommunity-synocli-packages/
