> id: https://www.appinn.com/proxmox-ve-9-0-released/-full

> link: https://www.appinn.com/proxmox-ve-9-0-released/

> title: Proxmox VE 90 Debian 13

# Proxmox VE 90 Debian 13
_Published on Wed, 06 Aug 2025 06:27:20 +0000_

**Proxmox VE 9.0** 在昨天晚上正式发布（北京时间2025年8月5日晚9点），基于 Debian 13 Trixie 打造，使用很新的 Linux 内核 6.14.8-2 作为稳定默认版本。重要软件也都紧跟主流，QEMU 升级到 10.0.2、LXC 用上 6.0.4、ZFS 2.3.3，还有 Ceph Squid 19.2.3 等。@[Appinn](https://www.appinn.com/proxmox-ve-9-0-released/)

![Proxmox VE 9.0 正式发布：基于 Debian 13，内核更前沿，快来体验极客级虚拟化环境 1](https://do-cdn.appinn.com/static3/images/2025/08/Copy-of-appinn-homework-2025-08-06T140449.700.jpg "Proxmox VE 9.0 正式发布：基于 Debian 13，内核更前沿，快来体验极客级虚拟化环境 1")

Proxmox VE 是什么？
---------------

Proxmox VE 是一个开源的虚拟化平台，它能把一台（或多台）物理服务器虚拟成好多台小电脑，里面可以跑 Windows、Linux、甚至是轻量级的容器。

功能

PVE 能干什么？

**虚拟机（VM）**

在一台物理机器上，像在一块硬盘里再装一台完整的电脑（比如 Windows、Ubuntu 等）。

**容器（LXC）**

更轻量的“子系统”，只装需要的应用，启动快、资源占用小（类似于 Docker 但更简单）。

**集中管理**

有一个 **网页界面**，在浏览器里就能创建、启动、迁移、备份这些虚拟机和容器，完全不需要敲命令行。

**多台服务器一起管理（集群）**

把几台物理服务器连在一起，统一调度资源；即使某台机器挂了，别的机器还能接着跑。

**存储和网络**

内置支持 ZFS、Ceph、NFS、SMB 等多种存储方式，还能用 **Open‑vSwitch** 做高级网络（VXLAN、SR‑IOV 等）。

**免费 + 商业版**

社区版免费、开源，想要官方技术支持可以购买企业版的订阅。

Proxmox VE 9.0 具体更新了什么
----------------------

组件名称

版本号

说明

Debian

13 “Trixie”

底层操作系统，提供稳定现代基础环境

Linux 内核

6.14.8-2

提升硬件支持和安全性

QEMU

10.0.2

虚拟机管理器，支持更多新特性和性能优化

LXC

6.0.4

Linux 容器组件，功能和兼容性增强

Ceph

Squid 19.2.3

分布式存储系统，适合企业级存储需求

ZFS

2.3.3

开源文件系统，支持快照和动态扩容

-   快照新玩法，卷链式支持，任何支持块存储的存储系统都能搞快照，告别阵营壁垒，无论 iSCSI/Fibre Channel 都通吃。
-   高可用（HA）配置规则升级，资源与节点/资源间亲和度自定义，对应你的实际需求，集群再大也能玩转。
-   SDN Fabric 上线，软件定义网络体验升级。
-   移动端带来了用 Rust 的 Yew 框架重构的现代化 Web UI，手机管理也能赏心悦目了。
-   ZFS 支持 RAIDZ 池动态添加新硬盘，再加再扩无需停机，真香属性爆表。
-   官方还给你全程升级指南，无论 PVE 8.x 还是 Beta 9.0 用户，都能 apt 一把直升，妥妥的。
-   **增强的移动界面**：PVE 9.0 重新设计了移动页面，让移动浏览器访问更容易。

升级和兼容性
------

社区关心的问题，Proxmox 都专门 FAQ 了一遍：

-   PVE 8.4 官方保证安全和漏洞修复支持到 2026 年 8 月，给你缓冲期慢慢迁移。
-   Beta 升 Stable，稳得很，只要 apt 就能安排；甚至能在 Debian 13 “Trixie” 上直接装 9.0。
-   Ceph 的升级是“双跳”：要先从 Reef 升到 Squid，再进 PVE 9.0，官方文档详细指导，照做就行。

获取
--

* * *

原文：https://www.appinn.com/proxmox-ve-9-0-released/

小众软件的青小蛙觉得，如果你还在使用 **VMware ESXi**，不妨考虑下 **Proxmox VE 9.0**。
