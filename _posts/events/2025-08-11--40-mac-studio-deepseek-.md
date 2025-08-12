> id: https://www.36kr.com/p/3415442855857538

> link: https://www.36kr.com/p/3415442855857538

> title: 40 Mac Studio DeepSeek

# 40 Mac Studio DeepSeek
_Published on Mon, 11 Aug 2025 04:04:07 GMT_

几个月前，爱范儿在一台 M3 Ultra 的 Mac Studio 上，成功部署了 671B 的 DeepSeek 的本地大模型（4-bit 量化版）。

**而如果我们搞来 4 台顶配 Mac Studio……**

-   每一台都是 M3 Ultra
-   512GB 统一内存
-   819GB/s 内存带宽
-   80 核 GPU
-   80Gbps 雷雳 5 双向传输……

把这四头猛兽，通过开源工具串联成一个「桌面级 AI 集群」——能否把本地推理的天花板再抬高一个维度？

**这也是来自英国创业公司 Exo Labs 正尝试解决的问题。而爱范儿成为了首批见到这个全新解决方案的中国媒体之一。**

![](https://img.36krcdn.com/hsossms/20250809/v2_72e6d6177edf4486be3398cf3e09fde6@000000_oswg116097oswg1080oswg810_img_000?x-oss-process=image/format,jpg/interlace,1)

**「地主家也没有余粮」**
--------------

你可能会以为，像牛津这样的顶级大学肯定 GPU 多得用不完，但其实完全不是这样。

Exo Labs 创始人 Alex 和 Seth 毕业于牛津大学——即使在这样的顶尖高校做研究，想要使用 GPU 集群也需要提前数月排队，一次只能申请一张卡，流程漫长而低效。

（ 别说牛津大学了，就连美国的国家实验室系统，拥有的超算集群算力也同样需要预约排队。 ）

**Alex 和 Seth 发现了一个现象：当前 AI 基础设施的高度集中化，使得个人研究者和小型团队被边缘化。**

为了解决问题，他们在去年 7 月启动了第一次实验，串联了手头上的两台 MacBook Pro，然后跑通了 LLaMA 模型。虽然性能有限，每秒只能输出 3 个 token，但已经足以验证 Apple Silicon 架构用于 AI 分布式推理的可行性。

更重要的是，尽管 LMStudio 等本地跑大模型的基础设施解决方案已经比较普遍了，但串联多台消费级电脑——组成集群——相关方案在当时仍然属于「未知水域」。

**而这个小团队的工作，也被苹果注意到了。**

![](https://img.36krcdn.com/hsossms/20250809/v2_b84bc2a3b9b74a7f8c02cfc021b8e1e7@000000_oswg112080oswg1080oswg1134_img_000?x-oss-process=image/format,jpg/interlace,1)

MacBook Pro 的算力终究是有限的，而二人集群化 Mac 电脑的工作，在今年 3 月迎来了一个关键的转折点：苹果发布了 M3 Ultra 顶配处理器版本的 Mac Studio。

512GB 统一内存、819GB/s 的内存带宽、80 核 GPU，再加上 Thunderbolt 5 的 80Gbps 双向传输能力——真正强有力的，足以运行 2025 上半年满血版大模型的本地 AI 集群，终于从理想变成了现实。

**同时跑两个 670 亿参数大模型是什么体验？**
--------------------------

4 台顶配 M3 Ultra 的 Mac Studio 通过 Thunderbolt 5 串联后，账面数据相当惊人：

-   128 核 CPU（32×4）
-   240 个 GPU 核心（80×4）
-   2TB 统一内存（512GB×4）
-   总内存带宽超过 3TB/s

**这样的组合，性能已经称得上是一台小型超算了，但从体积上仍然（勉强）可归到「家用级」。**

但硬件只是基础，真正发挥效能的关键是 Exo Labs 开发的分布式模型调度平台 Exo V2。Exo V2 会根据内存与带宽状态将模型自动拆分，部署在最合适的节点上。

Exo Labs 和苹果在现场提供了 Exo V2 的 demo，向爱范儿展示了以下核心能力：

**大模型加载：**8-bit 量化后的 DeepSeek，完整载入需要高达 700GB 内存，单台 Mac Studio 无力承担。而 Exo 的软件会将模型拆分部署到 2 台 Mac Studio 上完成加载。激活后，它的流式输出「打字速度」基本上超过了人的阅读速度。

![](https://img.36krcdn.com/hsossms/20250809/v2_c5c19647f41e413e8687b2e6298fe42b@000000_img_000?x-oss-process=image/format,jpg/interlace,1)

**并行推理：**在 DeepSeek V3 仍在两台顶配 Mac Studio 上跑着的同时，又加载了同样 670 亿参数的 DeepSeek R1。系统立即将 R1 分配到剩余的两台 Mac Studio，实现两个大模型并行推理，支持多用户同时提问。

![](https://img.36krcdn.com/hsossms/20250809/v2_836f195882494c3f92e7e123a81c1451@000000_img_000?x-oss-process=image/format,jpg/interlace,1)

**私有文档 RAG 问答：**拖入公司财报 PDF，模型在本地完成知识嵌入与问答，不依赖任何云端资源，数据完全私有可控。

![](https://img.36krcdn.com/hsossms/20250809/v2_e18597deffbd45e286e13f9260bd066a@000000_oswg103478oswg1080oswg1581_img_000?x-oss-process=image/format,jpg/interlace,1)

**轻量微调：**若企业有数千份内部资料，可通过 QLoRA + LoRA 技术进行本地微调。如果只用单台 Mac Studio，微调的耗时仍然长达数日，但 Exo 的集群调度能力，使得训练任务可线性加速，大幅缩短时间成本。

**巨大的成本差异**
-----------

爱范儿在现场后台观察拓扑图发现：即使 4 台机器同时处于高负载状态，整套系统功耗始终控制在 400W 以内，运行几乎无风扇噪音。

要在传统服务器方案中实现同等性能，至少需要部署 20 张 A100 显卡，服务器加网络设备成本超 200 万人民币，功耗达数千瓦，还需独立机房与制冷系统。

**——就这样，苹果 M 芯片在 AI 大模型的浪潮中，意外地找到了一个新的定位。确实令人没想到。**

![](https://img.36krcdn.com/hsossms/20250809/v2_cd38d2eb9e0f48e48d686b071c225eac@000000_oswg48949oswg1080oswg608_img_000?x-oss-process=image/format,jpg/interlace,1)

Exo Labs 基于 M3 Ultra Mac Studio 开发的这个套组，起售价 32999 元，配备 96GB 统一内存。而 512GB 的顶配版本，更是价格不菲。

但从技术角度来看，统一内存架构带来的优势是革命性的。

在设计 M 芯片之初，苹果更多是为节能、高效的个人创作而生。但统一内存、高带宽 GPU、Thunderbolt 多路径聚合等特性，反而非常适合 AI 本地推理这件事，虽然意料之外，却又在情理之中。

传统 GPU，即使是最高端的工作站卡，显存通常也只有 96GB。**而苹果的统一内存让 CPU 和 GPU 共享同一块高带宽内存，避免了数据在不同存储层级之间的频繁搬运，这对大模型推理来说意义重大。**

当然，EXO 这套方案也有明显的定位差异。它不是为了与 H100 正面对抗，不是为了训练下一代 GPT，而是为了解决实际的应用问题：运行自己的模型，保护自己的数据，进行必要的微调优化。

**如果说 H100 是金字塔顶的王者，而 Mac Studio 正在成为中小团队手中的瑞士军刀。**

本文来自微信公众号[“爱范儿”（ID：ifanr）](https://mp.weixin.qq.com/s?__biz=MjgzMTAwODI0MA==&mid=2652422107&idx=1&sn=280b39f7c7c4190b63088e3dfae73589&chksm=9a33b3c85de6d1081f68caa3e2078d346f54889ab699f7e1a1d450584d3279b0e2374fa107ac&scene=0&xtrack=1#rd)，作者：乔纳森何，36氪经授权发布。
