> id: https://www.ithome.com/0/876/985.htm

> link: https://www.ithome.com/0/876/985.htm

> title: DeepSeek-V31 AI Agent

# DeepSeek-V31 AI Agent
_Published on Thu, 21 Aug 2025 06:34:53 GMT_

感谢IT之家网友 [看资讯的小碳](https://m.ithome.com/html/app/open.html?url=ithome%3A%2F%2Fuserpage%3Fid%3D2524156) 的线索投递！

[IT之家](https://www.ithome.com/) 8 月 21 日消息，深度求索官方今日正式对外发布 **DeepSeek-V3.1**。本次升级包含以下主要变化：

-   **混合推理架构**：一个模型同时支持思考模式与非思考模式；
    
-   **更高的****思考效率**：相比 DeepSeek-R1-0528，DeepSeek-V3.1-Think 能在更短时间内给出答案；
    
-   **更强的 Agent 能力**：通过 Post-Training 优化，新模型在工具使用与智能体任务中的表现有较大提升。
    

官方 App 与网页端模型**已同步升级为 DeepSeek-V3.1**。用户可以通过**“深度思考”**按钮，实现思考模式与非思考模式的自由切换。

DeepSeek API 也已同步升级，deepseek-chat 对应**非思考模式**，deepseek-reasoner 对应**思考模式，**且上下文均已扩展为 128K。同时，API Beta 接口支持了 strict 模式的 Function Calling，以确保输出的 Function 满足 schema 定义。

另外，深度求索增加了对 **Anthropic API** 格式的支持，让用户可以将 DeepSeek-V3.1 的能力接入 **Claude Code** 框架。

工具调用 / 智能体支持增强
--------------

### 编程智能体

![图片](https://img.ithome.com/newsuploadfiles/2025/8/b4378105-c3b3-4cb4-a9c3-84d1ebbe58c0.png?x-bce-process=image/format,f_auto "DeepSeek-V3.1 正式发布，官方详解迈向 AI Agent 时代的第一步")

▲ 编程智能体测评（SWE 使用内部框架测评，相比开源框架 OpenHands 所需轮数更少；Terminal Bench 使用官方 Terminus 1 framework）

在代码修复测评 SWE 与命令行终端环境下的复杂任务（Terminal-Bench）测试中，DeepSeek-V3.1 相比之前的 DeepSeek 系列模型有明显提高。

### 搜索智能体

![图片](https://img.ithome.com/newsuploadfiles/2025/8/63e0527f-43ce-4e34-8c25-59b0c5970feb.png?x-bce-process=image/format,f_auto "DeepSeek-V3.1 正式发布，官方详解迈向 AI Agent 时代的第一步")

▲ 搜索智能体测评（测试结果调用商用搜索引擎 API + 网页过滤 + 128K context window；R1-0528 使用内部 workflow 模式测试；HLE 测试同时使用 python 与 search 工具）

DeepSeek-V3.1 在多项搜索评测指标上取得了较大提升。在需要多步推理的复杂搜索测试（browsecomp）与多学科专家级难题测试（HLE）上，DeepSeek-V3.1 性能已大幅领先 R1-0528。

思考效率提升
------

深度求索官方的测试结果显示，经过思维链压缩训练后，V3.1-Think 在输出 token 数减少 20%-50% 的情况下，各项任务的平均表现与 R1-0528 持平。

![图片](https://img.ithome.com/newsuploadfiles/2025/8/937425df-5419-460e-a01a-9072db91a496.png?x-bce-process=image/format,f_auto "DeepSeek-V3.1 正式发布，官方详解迈向 AI Agent 时代的第一步")

▲ 在各项评测指标得分基本持平的情况下（AIME 2015: 87.5/88.4，GPQA: 81/80.1，liveCodeBench: 73.3/74.8），R1-0528 与 V3.1-Think 的 token 消耗量对比图

同时，V3.1 在非思考模式下的输出长度也得到了有效控制，相比于 DeepSeek-V3-0324 ，能够在输出长度明显减少的情况下保持相同的模型性能。

API & 模型开源
----------

### 模型开源

V3.1 的 Base 模型在 V3 的基础上重新做了外扩训练，一共增加训练了 840B tokens。Base 模型与后训练模型均已在 Huggingface 与魔搭开源。IT之家附开源地址：

**Base 模型：**

-   Hugging Face：
    
    [https://huggingface.co/deepseek-ai/DeepSeek-V3.1-Base](https://huggingface.co/deepseek-ai/DeepSeek-V3.1-Base)
    
-   魔搭：
    
    [https://modelscope.cn/models/deepseek-ai/DeepSeek-V3.1-Base](https://modelscope.cn/models/deepseek-ai/DeepSeek-V3.1-Base)
    

**后训练模型：**

-   Hugging Face：
    
    [https://huggingface.co/deepseek-ai/DeepSeek-V3.1](https://huggingface.co/deepseek-ai/DeepSeek-V3.1)
    
-   魔搭：
    
    [https://modelscope.cn/models/deepseek-ai/DeepSeek-V3.1](https://modelscope.cn/models/deepseek-ai/DeepSeek-V3.1)
    

需要注意的是，DeepSeek-V3.1 使用了 UE8M0 FP8 Scale 的参数精度。另外，V3.1 对分词器及 chat template 进行了较大调整，与 DeepSeek-V3 存在明显差异。建议有部署需求的用户仔细阅读新版说明文档。

价格调整
----

深度求索将于**北京时间 2025 年 9 月 6 日凌晨起**，对 DeepSeek 开放平台 API 接口调用价格进行如下调整：

-   执行新版价格表（如下图所示，详见定价页面）；
    
-   取消夜间时段优惠。
    

![图片](https://img.ithome.com/newsuploadfiles/2025/8/a93d2654-6c5b-4318-a3c1-4d9484b437a1.jpg?x-bce-process=image/format,f_auto "DeepSeek-V3.1 正式发布，官方详解迈向 AI Agent 时代的第一步")

在 9 月 6 日前，所有 API 服务仍按**原价格政策计费**，用户可继续享受当前优惠。同时，为更好地满足用户的调用需求，深度求索已进一步扩容 API 服务资源。

**相关阅读：**

-   《[DeepSeek 开源新模型 V3.1：约 685B 参数，上下文长度拓展至 128K](https://www.ithome.com/0/876/637.htm)》
    
-   《[DeepSeek 通知线上模型版本升级至 V3.1，上下文长度拓展至 128k](https://www.ithome.com/0/876/555.htm)》
    

广告声明：文内含有的对外跳转链接（包括不限于超链接、二维码、口令等形式），用于传递更多信息，节省甄选时间，结果仅供参考，IT之家所有文章均包含本声明。
