> id: https://www.appinn.com/openai-gpt-oss/-full

> link: https://www.appinn.com/openai-gpt-oss/

> title: OpenAI gpt-oss 16GB

# OpenAI gpt-oss 16GB
_Published on Wed, 06 Aug 2025 08:30:16 +0000_

OpenAI 终于开源了自己的模型：**gpt-oss-120b** 和 **gpt-oss-20b**，并发布了中文内容：《[隆重推出 gpt-oss](https://openai.com/zh-Hans-CN/index/introducing-gpt-oss/)》。@[Appinn](https://www.appinn.com/openai-gpt-oss/)

![OpenAI 开源模型 gpt-oss，只需要 16GB 显存。目前可在线试用 1](https://do-cdn.appinn.com/static3/images/2025/08/Copy-of-appinn-homework-2025-08-06T162417.252.jpg "OpenAI 开源模型 gpt-oss，只需要 16GB 显存。目前可在线试用 1")

这是两款 Apache 2.0 许可证下的轻量级语言模型，可商用。均基于 Transformer 架构，采用专家混合（MoE）技术，gpt-oss-120b 约有 1170 亿参数，每个 token 激活约 51 亿参数；gpt-oss-20b 有 210 亿参数，激活约 36 亿参数。支持最长 128k 的上下文长度。

性能方面，gpt-oss-120b 在核心推理测试中几乎与 OpenAI 的闭源 o4-mini 模型持平，且能高效运行于单个 80GB GPU；gpt-oss-20b 性能接近 o3-mini 模型，仅需 16GB 内存，适合边缘设备和本地推理应用。

**模型**

**层数**

**总参数**

**每个令牌的活跃参数**

**总专家数**

**每个令牌的活跃专家数**

**上下文长度**

gpt-oss-120b

36

117b

5.1b

128

4

128k

gpt-oss-20b

24

21b

3.6b

32

4

128k

gpt-oss 使用了主要为英文的纯文本数据集对模型进行了训练，重点关注 STEM、编程和通用知识领域。并且使用了 OpenAI o4-mini 和 GPT‑4o 所用令牌化器的超集进行数据令牌化，即 ‘o200k\_harmony’，该令牌化器我们今日也一并开源。

如何部署
----

目前 **gpt-oss-120b** 和 **gpt-oss-20b** 两个模型已经可以在 huggingface 下载：

建议个人用户尝试 20b 模型，仅需16GB显存。毕竟不是几个人有 80G 显存来部署 120b 🐶

### **Ollama** 安装

\# gpt-oss-20b
ollama pull gpt-oss:20b
ollama run gpt-oss:20b

下载量大约 14GB，然后就可以使用 Ollama 对话了。

在线试用
----

目前可以直接在线试用这两个模型：

![OpenAI 开源模型 gpt-oss，只需要 16GB 显存。目前可在线试用 2](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201578%20995'%3E%3C/svg%3E "OpenAI 开源模型 gpt-oss，只需要 16GB 显存。目前可在线试用 2")

并且支持联网。

* * *

原文：https://www.appinn.com/openai-gpt-oss/
