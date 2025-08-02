> id: https://www.appinn.com/annas-mcp/-full

> link: https://www.appinn.com/annas-mcp/

> title: annas-mcp MCP CLI

# annas-mcp MCP CLI
_Published on Thu, 31 Jul 2025 07:53:23 +0000_

**annas-mcp** 是一个从安娜的档案（Anna’s Archive）搜索和下载文档的 MCP 服务器和 CLI 工具。其中 CLI 提供了 Windows、macOS 与 Linux 版本。但注意需要拥有安娜的档案 API KEY 才可以使用。@Appinn

![annas-mcp - 安娜的档案 MCP 服务器与 CLI 工具 1](https://do-cdn.appinn.com/static3/images/2025/07/Copy-of-appinn-homework-2025-07-31T152520.670.jpg "annas-mcp - 安娜的档案 MCP 服务器与 CLI 工具 1")

上次介绍安娜的档案的时候，还是去年：

从目前的统计来看，现在的种子已经累计了 1.1PB 的数据！

annas-mcp
---------

annas-mcp 可以同时作为：

1.  mcp 服务器
2.  cli 命令行工具

当使用 mcp 继承到客户端的时候，先下载，然后：

"anna-mcp": {
    "command": "/Users/iosifache/Downloads/annas-mcp",
    "args": \["mcp"\],
    "env": {
        "ANNAS\_SECRET\_KEY": "feedfacecafebeef",
        "ANNAS\_DOWNLOAD\_PATH": "/Users/iosifache/Downloads"
    }
}

当作为 cli 命令的时候：

可以直接使用 `./annas-mcp search 名称` 进行搜索（不需要 API Key），然后使用 `download [hash] [filename]` 进行下载（需要 API Key）。

获取
--

* * *

原文：https://www.appinn.com/annas-mcp/
