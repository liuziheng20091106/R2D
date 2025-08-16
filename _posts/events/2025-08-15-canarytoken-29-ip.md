> id: https://www.appinn.com/canarytoken/-full

> link: https://www.appinn.com/canarytoken/

> title: CanaryToken 29 IP

# CanaryToken 29 IP
_Published on Fri, 15 Aug 2025 09:35:00 +0000_

**CanaryToken** 是一个非常有趣的服务，它提供了 29 种常见的蜜罐陷阱，包括 Windows 文件夹、运行指定程序、打开 PDF 文档、Word/Excel 文件、图片、二维码，以及网络蜜罐：MySQL、邮箱、AWS 证书、Log4shell 等，只要有人使用了这些陷阱，你就会收到通知，支持邮件与 WebHook。@[Appinn](https://www.appinn.com/canarytoken/)

![CanaryToken - 29 种蜜罐陷阱！同事偷看我文件后，他的IP就自动'投案'到我邮箱了 1](https://do-cdn.appinn.com/static3/images/2025/08/Copy-of-appinn-homework-2025-08-15T170900.787.jpg "CanaryToken - 29 种蜜罐陷阱！同事偷看我文件后，他的IP就自动'投案'到我邮箱了 1")

来自[**发现频道**](https://meta.appinn.net/c/faxian/10)，@艾尔赛高 同学的推荐：[https://meta.appinn.net/t/topic/73994](https://meta.appinn.net/t/topic/73994)

偶然发现的一个有趣服务。提前生成无害的蜜罐密钥，放在容易被攻击者接触的位置（例如 ~/.aws/credentials ），如果被攻击/泄露了，当攻击者尝试使用密钥的时候，会受到通知（可选邮件/webhook）

### 示例场景：

-   监控开发环境是否被入侵
-   监控私有代码仓库是否被意外拉取
-   监控密钥是否意外泄漏

一个例子：监控 Windows 文件夹
-------------------

在 [CanaryToken](https://canarytokens.org/nest/?utm_source=appinn.com) 官网找到 **Windows Folder**，打开后输入邮箱、说明（用来让你区分哪个文件夹的，比如输入：我的小姐姐的家），以及可选设置 Webhook 通知：

![CanaryToken - 29 种蜜罐陷阱！同事偷看我文件后，他的IP就自动'投案'到我邮箱了 2](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%202526%201688'%3E%3C/svg%3E "CanaryToken - 29 种蜜罐陷阱！同事偷看我文件后，他的IP就自动'投案'到我邮箱了 2")

然后点击下方的 Create Canarytoken 按钮，从新的页面下载 zip 文件：

![CanaryToken - 29 种蜜罐陷阱！同事偷看我文件后，他的IP就自动'投案'到我邮箱了 3](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201080%201193'%3E%3C/svg%3E "CanaryToken - 29 种蜜罐陷阱！同事偷看我文件后，他的IP就自动'投案'到我邮箱了 3")

注意由于系统限制，这个蜜罐仅支持 Windows 10 以下版本。

在这个 zip 文件夹中，有一个 desktop.ini 文件，复制到你要监控的文件夹里就行了。

desktop.ini 内容很简，打开就能触发里面的 URL 的意思：

\[.ShellClassInfo\]
IconResource=\\\\%USERNAME%.%COMPUTERNAME%.%USERDOMAIN%.INI.xxxxxxxx.canarytokens.com\\resource.dll

就好了。一旦有人打开了你的文件夹，就会收到邮件，包括时间、IP地址、描述：

![CanaryToken - 29 种蜜罐陷阱！同事偷看我文件后，他的IP就自动'投案'到我邮箱了 4](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201336%201468'%3E%3C/svg%3E "CanaryToken - 29 种蜜罐陷阱！同事偷看我文件后，他的IP就自动'投案'到我邮箱了 4")

而从邮件点进去还能看到历史记录、删除警报灯功能。

总之，给青小蛙一种：这是我能用的吗？的强烈感觉。

快去玩玩吧 😂

**CanaryToken** 的29 种蜜罐陷阱
-------------------------

**CanaryToken** 能设置的蜜罐一共 29 种，非常丰富，你总能用到

蜜罐名称 (英文)

简要说明

Web bug

攻击者访问特定URL时发送告警

DNS

攻击者解析特定DNS名称时告警

Credit Card

攻击者尝试使用你的信用卡信息时告警

QR code

攻击者扫描你的二维码时触发告警

MySQL

攻击者加载你的MySQL数据库转储文件时告警

AWS keys

攻击者使用伪造的AWS API密钥时告警

Fake App

攻击者运行伪造应用程序时发送告警

Log4shell

当检测到Log4j漏洞（CVE-2021-44228）日志时告警

Fast redirect

当攻击者访问URL时快速重定向并告警

Slow redirect

当攻击者访问URL时慢速重定向并收集更多信息

Sensitive command

当检测到可疑Windows命令执行时告警

Windows Fake File System

伪造文件系统中访问文件时触发告警

Web image

上传的图片被查看时触发告警

Azure login certificate

Azure服务主身份登录时触发告警

Microsoft Excel

伪造的Excel文档被打开时告警

Microsoft Word

伪造的Word文档被打开时告警

SVN

访问SVN仓库时触发告警

Unique email address

发送邮件到该唯一邮箱地址时触发告警

Microsoft SQL Server

访问MS SQL数据库时触发告警

Custom EXE / binary

执行伪造EXE或DLL文件时触发告警

Acrobat Reader PDF

伪造的PDF文档被打开时告警

Windows Folder

在Windows资源管理器中浏览伪造文件夹时触发告警

JS cloned website

通过JavaScript检测网站被克隆时触发告警

CSS cloned website

通过CSS监测网站克隆时触发告警

Kubeconfig

使用你的Kubernetes配置时触发告警

WireGuard VPN

使用你的WireGuard VPN客户端配置时触发告警

Azure Entra ID login

钓鱼Azure Entra ID登录时触发告警

Network Folder

访问映射的WebDAV网络文件夹时触发告警

SAML IdP App

从身份提供者仪表板打开伪造应用时触发告警

原文：https://www.appinn.com/canarytoken/
