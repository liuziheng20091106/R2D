> id: https://www.36kr.com/p/3430524032372096

> link: https://www.36kr.com/p/3430524032372096

> title: DeepSeek V31 BaseClaude 4R2V4

# DeepSeek V31 BaseClaude 4R2V4
_Published on Wed, 20 Aug 2025 03:48:51 GMT_

就在昨晚，DeepSeek官方悄然上线了全新的V3.1版本，上下文长度拓展到128k。

![](https://img.36krcdn.com/hsossms/20250820/v2_e64255ec4653493f8086cd2154bbbfc4@5091053_oswg95853oswg866oswg233_img_000?x-oss-process=image/format,jpg/interlace,1)

本次开源的V3.1模型拥有685B参数，支持多种精度格式，从BF16到FP8。

综合公开信息和国内大咖karminski3的实测，V3.1此次更新亮点有：

**编程能力：**表现突出，根据社区使用Aider测试数据，V3.1在开源模型中霸榜。

**性能突破**：V3.1在Aider编程基准测试中取得71.6%高分，超越Claude Opus 4，同时推理和响应速度更快。

**原生搜索：**新增了原生「search token」的支持，这意味着搜索的支持更好。

**架构创新**：线上模型去除「R1」标识，分析称DeepSeek未来有望采用「混合架构」。

**成本优势**：每次完整编程任务仅需1.01美元，成本仅为专有系统的六十分之一。

值得一提的是，官方群中强调拓展至128K上下文，此前V3版本就已经支持。

![](https://img.36krcdn.com/hsossms/20250820/v2_b45bd78ec8fa4c5db8b18639c200bccd@5091053_oswg65771oswg1080oswg338_img_000?x-oss-process=image/format,jpg/interlace,1)

对于这波更新，大家的热情可谓是相当高涨。

即便还未公布模型卡，DeepSeek V3.1就已经在Hugging Face的趋势榜上排到了第四。

![](https://img.36krcdn.com/hsossms/20250820/v2_c8f05eb43ad6488aa579fc78f7b12bcf@5091053_oswg227457oswg1080oswg453_img_000?x-oss-process=image/format,jpg/interlace,1)

![](https://img.36krcdn.com/hsossms/20250820/v2_30b1783ff21d47bea421b34d2382fee8@5091053_oswg139867oswg1080oswg272_img_000?x-oss-process=image/format,jpg/interlace,1)

DeepSeek粉丝数已破8万

看到这里，网友们更期待R2的发布了！

![](https://img.36krcdn.com/hsossms/20250820/v2_61395c0af9544347ae9e17d48a5e9e4d@5091053_oswg49820oswg810oswg224_img_000?x-oss-process=image/format,jpg/interlace,1)

**混合推理，编程击败Claude 4**
---------------------

这次最明显的变化是，DeepSeek在官方APP和网页端上，把深度思考（R1）中的「R1」去掉了。

![](https://img.36krcdn.com/hsossms/20250820/v2_b3ddedb264d043399d67848539217bdf@5091053_oswg66942oswg1080oswg313_img_000?x-oss-process=image/format,jpg/interlace,1)

同时，与V3-base相比，DeepSeek V3.1新增了四个特殊Token：

<｜search▁begin｜> (id: 128796)

<｜search▁end｜> (id: 128797)

<think> (id: 128798)

</think> (id: 128799)

![](https://img.36krcdn.com/hsossms/20250820/v2_c7afd78dec4e4efcb53351d6a8b5123e@5091053_oswg396376oswg1080oswg1206_img_000?x-oss-process=image/format,jpg/interlace,1)

对此，有推测认为，这可能暗示推理模型与非推理模型的融合。

![](https://img.36krcdn.com/hsossms/20250820/v2_1f12205bab964639bdc0e38852bd3008@5091053_oswg100021oswg866oswg368_img_000?x-oss-process=image/format,jpg/interlace,1)

在编程方面，根据网友曝出的结果，DeepSeek V3.1在Aider Polyglot多语言编程测试中拿下了71.6%高分，一举击败了Claude 4 Opus、DeepSeek R1。

![](https://img.36krcdn.com/hsossms/20250820/v2_216f40805ffb48d8bc7cdd758ae7cd7c@5091053_oswg146530oswg1080oswg415_img_000?x-oss-process=image/format,jpg/interlace,1)

而且，它的成本仅1美元，成为非推理模型中的SOTA。

![](https://img.36krcdn.com/hsossms/20250820/v2_31feb59c9c174a46a810bb1f186fed0b@5091053_oswg421312oswg1080oswg788_img_000?x-oss-process=image/format,jpg/interlace,1)

最鲜明的对比，V3.1编程性能比Claude 4高1%，成本要低68倍。

![](https://img.36krcdn.com/hsossms/20250820/v2_b8f392c59cff4e7dbe95c7cd991f89e4@5091053_oswg88256oswg1080oswg210_img_000?x-oss-process=image/format,jpg/interlace,1)

在SVGBench基准上，V3.1实力仅次于GPT-4.1-mini，远超DeepSeek R1的实力。

![](https://img.36krcdn.com/hsossms/20250820/v2_ac5c07daf80f482782f376788ed2999e@5091053_oswg328002oswg1080oswg2013_img_000?x-oss-process=image/format,jpg/interlace,1)

在MMLU多任务语言理解方面，DeepSeek V3.1毫不逊色于GPT-5。不过在，编程、研究生级基准问答、软件工程上，V3.1与之有一定的差距。

![](https://img.36krcdn.com/hsossms/20250820/v2_15d419979f534d83b8fa14838f35e85f@5091053_oswg287670oswg1080oswg1748_img_000?x-oss-process=image/format,jpg/interlace,1)

一位网友实测，模拟六边形中小球自由落体的物理测试，DeepSeek V3.1理解力明显提升。

![](https://img.36krcdn.com/hsossms/20250820/v2_bb84ade34c6142a9bc3853030865f976@5091053_img_gif?x-oss-process=image/quality,q_80)

**一手实测**
--------

第一时间，我们对V3.1进行了实测，首先是此次模型更新的重点：上下文长度。

假设对于中文而言，1个token ≈ 1–1.3个汉字，那么这128K tokens ≈ 100,000–160,000汉字。

相当于**整本《红楼梦》正文（约80–100万字）的1/6–1/8**，或者一篇**超长博士论文/大部头学术专著**。

实际测试也很准确，DeepSeek告诉我们它只能阅读差不多9%，也就是大约十分之一。

![](https://img.36krcdn.com/hsossms/20250820/v2_545477e01ab544878ee5a87e53ee6d96@5091053_oswg34804oswg1080oswg286_img_000?x-oss-process=image/format,jpg/interlace,1)

由于总结内容太长，我们截取了前三回，你觉得这个总结的怎么样？

![](https://img.36krcdn.com/hsossms/20250820/v2_e2cbf713ec2043d7ac7edd744d103793@5091053_oswg275603oswg1080oswg891_img_000?x-oss-process=image/format,jpg/interlace,1)

在128K上下文测试中，DeepSeek-V3.1输出速度相比以往获得较大提升，并且在工程上做了一些优化。

![](https://img.36krcdn.com/hsossms/20250820/v2_033d4fd856044cc6938e62b3e093fd02@5091053_oswg172325oswg1080oswg602_img_000?x-oss-process=image/format,jpg/interlace,1)

此次更新，DeepSeek重点强调了对上下文的支持。

整个活，给DeepSeek-V3.1上点压力，让它根据「梦」这个字，输出尽可能多的内容，尽量达到上下文极限。

![](https://img.36krcdn.com/hsossms/20250820/v2_402975b470004567aaa308140fa1a658@5091053_oswg24512oswg1080oswg133_img_000?x-oss-process=image/format,jpg/interlace,1)

不过最后，差不多只输出了3000字左右，模型就停止了输出。

![](https://img.36krcdn.com/hsossms/20250820/v2_35333fcce05e4034a3cd1f472eaaa77b@5091053_oswg133931oswg1080oswg616_img_000?x-oss-process=image/format,jpg/interlace,1)

再来看下推理能力。

经典的9.11和9.9比大小问题，两种询问方式都能正确做答。

这次更新的一大体感还是速度变快了很多。

![](https://img.36krcdn.com/hsossms/20250820/v2_818ae043da084c3b936c1a1ca1209053@5091053_oswg74906oswg1080oswg342_img_000?x-oss-process=image/format,jpg/interlace,1)

最后再来看看编程能力。

DeepSeek的上一个模型是R1-0528，主打的是编程能力。

看看这次V3.1是否有更大的提升。

![](https://img.36krcdn.com/hsossms/20250820/v2_bba226afe0dd4c4db6ab79e470e92ee1@5091053_oswg152677oswg1080oswg615_img_000?x-oss-process=image/format,jpg/interlace,1)

最终结果只能说，打个80分吧，基本要求都满足了，但是画面风格和颜色变换功能并没有完美实现。

![](https://img.36krcdn.com/hsossms/20250820/v2_be40392a20b743149f202c06d226cba4@5091053_img_gif?x-oss-process=image/quality,q_80)

并且和R1-0528的结果相比，两者之间还是有些差距的，但孰好孰坏还需看个人偏好。

以下是开启思考模式后的结果，你觉得哪个更好？

![](https://img.36krcdn.com/hsossms/20250820/v2_bc96939b8d4447e884f5612bdb61947b@5091053_img_gif?x-oss-process=image/quality,q_80)

接下来，看看DeepSeek V3.1能否复刻出GPT-5发布会上的法语学习小程序。

我们再来让V3.1画一个自己的SVG自画像，两种效果着实有些抽象。

![](https://img.36krcdn.com/hsossms/20250820/v2_4ffab579995b48f3ad9f9bbd4336ca19@5091053_oswg64131oswg1080oswg245_img_000?x-oss-process=image/format,jpg/interlace,1)

![](https://img.36krcdn.com/hsossms/20250820/v2_3037fbbff8c04fe88f93e90203c2d115@5091053_oswg1056831oswg1080oswg2836_img_000?x-oss-process=image/format,jpg/interlace,1)

![](https://img.36krcdn.com/hsossms/20250820/v2_04e641f637fb4089997dccfe786d761d@5091053_oswg584155oswg1080oswg2072_img_000?x-oss-process=image/format,jpg/interlace,1)

**参考资料：HYX**

https://weibo.com/2169039837/Q0FC4lmeo

https://x.com/karminski3/status/1957928641884766314

https://github.com/johnbean393/SVGBench/

https://huggingface.co/deepseek-ai/DeepSeek-V3.1-Base

本文来自微信公众号[“新智元”](https://mp.weixin.qq.com/s/panSxt0KlfUoaudcdE8y5Q?click_id=489)，作者：新智元，编辑：桃子 定慧，36氪经授权发布。
