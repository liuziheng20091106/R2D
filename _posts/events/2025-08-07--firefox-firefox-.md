> id: https://www.appinn.com/run-firefox-sync-server/-full

> link: https://www.appinn.com/run-firefox-sync-server/

> title: Firefox Firefox

# Firefox Firefox
_Published on Thu, 07 Aug 2025 07:10:02 +0000_

![运行你自己的 Firefox 同步服务器，替代 Firefox 中国 1](https://do-cdn.appinn.com/static3/images/2025/08/Copy-of-appinn-homework-2025-08-07T150150.097.jpg "运行你自己的 Firefox 同步服务器，替代 Firefox 中国 1")

今天早上 @huaingabc 同学在 [Firefox 中国关闭，如何备份数据](https://mp.weixin.qq.com/s/_VToK1oJ5d_4ZWu-bHFDrQ)一文中说：

> 昨天亲测，把国内账号改为国际账号就行了；退出登录，（退出前最好备份一下数据，且退出的时候不要清除数据）然后地址栏输入 about:config → 搜索并修改以下参数identity.fxaccounts.autoconfig.uri → “https://accounts.firefox.com/, 重启就行了。国际账号为新账号，简单设置下就好了。

青小蛙表示很好奇，就搜索了下，没想到发现了新大陆：

![运行你自己的 Firefox 同步服务器，替代 Firefox 中国 2](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201076%201090'%3E%3C/svg%3E "运行你自己的 Firefox 同步服务器，替代 Firefox 中国 2")

这是 Mozilla 官方发布的全套 Firefox 同步服务器教程文档（[Mozilla Services Documentation](https://github.com/mozilla-services/docs)）啊。

包括两个部分：

-   Sync-1.5 Server
-   Firefox Accounts Server

Sync-1.5 Server（自托管同步服务器）
-------------------------

-   **主要功能**：确实是用于同步书签、历史记录、密码等浏览器数据。这是一个为用户提供数据同步功能的服务器。
-   **存储与同步接口**：它为用户提供了一个存储后端和同步接口，让数据同步到自己搭建的服务器，从而替代 Mozilla 的官方服务。这对于希望完全掌控自己数据的用户非常有吸引力。
-   **技术栈与数据库**：该服务基于 Python (特别是 Python 2.7)，并可以通过配置支持多种数据库，如 SQLite, MySQL (使用 `pymysql` 驱动) 和 Postgres (通过配置 `sqluri` 连接字符串)。
-   **客户端配置**：用户需要在 Firefox 浏览器的 `about:config` 页面中，将 `identity.sync.tokenserver.uri` 指向自建服务器的地址，以完成同步配置。
-   **服务器配置**：在服务器的 `syncserver.ini` 配置文件中，必须指定一个 `public_url`，这是客户端能访问到的服务器公共 URL。
-   **目标用户**：完全符合您的描述，适合那些希望掌控个人数据存储和同步流程的用户。

Firefox Accounts Server（Firefox 账户服务器）
--------------------------------------

-   **与 Sync Server 的关系**：官方文档指出，由于安全和认证机制，如果您选择自托管 Firefox 账户服务器，那么您也**必须**同时自托管 Sync-1.5 服务器。
-   **独立账户系统**：这是一个完全独立的账户管理系统，负责用户的身份验证（登录、注册、密码重置等）。
-   **核心组件**：它包含两个核心部分：
-   **认证服务器 (auth-server)**：管理账户数据库和用户凭证。
-   **内容服务器 (content-server)**：提供用户在浏览器上看到的账户管理网页界面。
-   **技术栈**：该服务主要基于 Node.js 构建。
-   **自托管替代方案**：它的主要目的就是替代 Mozilla 官方的 Firefox 账户服务，实现完全自托管的账户管理。
-   **客户端配置**：配置方法与 Sync Server 类似，需要在 Firefox 的 `about:config` 中设置多个 URL，将 `identity.fxaccounts.autoconfig.uri` 或其他相关 `fxaccounts` 地址指向您自建的账户服务器。

也就是说，根据这个教程最终可以实现：

一个完整的自托管 Firefox 数据同步服务，与 Firefox 官方一模一样…除了自己用，你还可以为别人提供服务，只需要在 `about:config` 里面修改服务器地址就好了。

甚至，你都能通过 Firefox 的源码，直接自定义同步服务器地址，重新编译后，发给自己的用户，默认就使用了你的同步服务器，就像之前 Firefox 中国做的那样…

**或者可以这样说**：Firefox 官方的同步功能，就是这个东西。

就…正经的开源项目，还挺酷的。

* * *

原文：https://www.appinn.com/run-firefox-sync-server/
