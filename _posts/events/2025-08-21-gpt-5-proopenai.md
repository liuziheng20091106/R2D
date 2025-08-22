> id: https://www.36kr.com/p/3431915583999616

> link: https://www.36kr.com/p/3431915583999616

> title: GPT-5 ProOpenAI

# GPT-5 ProOpenAI
_Published on Thu, 21 Aug 2025 03:10:23 GMT_

> 微软前AI副总裁兼杰出科学家Sebastien Bubeck发文表示GPT-5 Pro从零攻克了数学论文中的未解区间，这个发现让他大受震撼。该发现引得众多大佬转发，OpenAI总裁认为AI或将加速数学研究。

AI真的能解决人类的**前沿问题**吗？

比如类似庞加莱猜想、求解麦克斯韦方程、费马大定理、黎曼猜想等问题。

今天这个问题有了答案。

**AI还真的可以！**完全独立，不参考人类已有的任何方法。

昨晚，GPT-5 Pro可以从零开始完全求解一个复杂的数学问题。

![](https://img.36krcdn.com/hsossms/20250821/v2_6b1430718bdf4ce0b426eb1ef51aa060@5091053_oswg118406oswg1080oswg535_img_000?x-oss-process=image/format,jpg/interlace,1)

并且再次强调，它没有使用任何人类此前的证明方法。

而它的答案比论文中的求解方法都要好。

![](https://img.36krcdn.com/hsossms/20250821/v2_1fc908757ba34425a85a1e88db24b568@5091053_oswg254533oswg1080oswg664_img_000?x-oss-process=image/format,jpg/interlace,1)

不过值得人类庆幸的是，论文作者后面又提供了全新的方法超过了AI。

**Sebastien Bubeck**是OpenAI的研究工程师，此前曾担任微软人工智能副总裁兼杰出科学家。

他把一篇论文直接扔给了GPT-5 Pro。

这篇论文研究了一个非常自然的问题：在光滑凸优化中，梯度下降法的步长η满足什么条件时，迭代点所对应的函数值形成的曲线是凸的？

![](https://img.36krcdn.com/hsossms/20250821/v2_7819f5ab4aef4b869ccf7b3c23aaf1c3@5091053_oswg29657oswg1080oswg262_img_000?x-oss-process=image/format,jpg/interlace,1)

论文地址：https://arxiv.org/pdf/2503.10138v1

在论文的v1版本中，他们证明了如果η小于1/L（L为光滑度），则可以得到此属性。

如果η大于1.75/L，作者他们就构造了一个反例。

因此，未解决的问题是：**在区间\[1/L,1.75/L\]内会发生什么情况。**

首先，简单解释下这个问题。

**梯度下降**就像下山，每一步要选一个**步长η**。**L**可以理解成地形的「弯曲程度」（越大越陡/越敏感）。

![](https://img.36krcdn.com/hsossms/20250821/v2_87d7443c41524c8182b1e7fb35529a57@5091053_oswg126663oswg1080oswg333_img_000?x-oss-process=image/format,jpg/interlace,1)

论文不只关心「会不会往下走」（单调下降），还关心**下降的轨迹是不是「凸」的**：也就是**每一步的进步幅度不会忽大忽小**，不会「前面像平台、后面突然跳崖」。

这对**何时停下来**很有用——凸就表示越来越平稳，不会突然又大降。

![](https://img.36krcdn.com/hsossms/20250821/v2_3d85723d6aaf4f9aa261508223a7450c@5091053_oswg86650oswg1080oswg496_img_000?x-oss-process=image/format,jpg/interlace,1)

Sebastien用GPT-5 Pro去攻这个未解决区间，模型把已知下限从1/L推进到1.5/L。

以下是GPT-5 Pro给出的证明。

虽然初看不明觉厉，但整体证明过程看起来非常优雅。

![](https://img.36krcdn.com/hsossms/20250821/v2_d63d718d1fc245cc9c653ad16a035fd8@5091053_oswg75839oswg1050oswg1262_img_000?x-oss-process=image/format,jpg/interlace,1)

本来这个发现让Sebastien兴奋了好一阵，甚至想要直接发一篇arXiv论文。

但是，人类还是比AI快了一步。

论文原作者很快发了v2版本，彻底收尾，他们将阈值改写**1.75/L**。

Sebastien认为这个发现依然非常令人鼓舞，为什么？AI不是并没有打败人类吗？

因为GPT-5 Pro在证明中，它试图证明的是1.5/L而不是1.75/L，这也表明GPT-5 Pro并没有直接去搜索v2版本。

另外，上述证明与v2的证明也非常不同，它更像是v1证明的一种演进。

这么看，现在的AI能力，不仅仅是博士级，很多时候都超过博士了。

这个发现也让很多大佬们表示，AI下一个可能改变和影响的就是数学领域。

在AI的帮助下，人类知识的边界将会再次被拓宽。

![](https://img.36krcdn.com/hsossms/20250821/v2_2cd717284b314c8f94bf0e5cb3b32f37@5091053_oswg120659oswg1068oswg310_img_000?x-oss-process=image/format,jpg/interlace,1)

OpenAI的总裁Greg Brockman甚至表示这可能是AI在数学领域**展现生命力**的一种迹象。

![](https://img.36krcdn.com/hsossms/20250821/v2_d18d3a9975f84be2920f3b8e348d24d1@5091053_oswg75363oswg1080oswg282_img_000?x-oss-process=image/format,jpg/interlace,1)

此外，这次发现也和之前OpenAI官宣自己拿下IMO和IOI金牌不同。

这次攻破数学题的模型，就是面向用户的GPT-5 Pro版本，而不是内部推理模型。

![](https://img.36krcdn.com/hsossms/20250821/v2_a1224cd87b4a4699a83abc6c20fcf5ed@5091053_oswg312575oswg1080oswg643_img_000?x-oss-process=image/format,jpg/interlace,1)

Sebastien表示这个结论是经过自己25分钟验证。

作为前微软人工智能副总裁兼杰出科学家，他的证明应该没问题，看来AI确实实际证明了该数学问题。

![](https://img.36krcdn.com/hsossms/20250821/v2_1c078a02f666483e8b65d5db7768b5ed@5091053_oswg231662oswg1067oswg717_img_000?x-oss-process=image/format,jpg/interlace,1)

GPT-5发布后虽然毁誉参半。

但是，GPT-5 Pro是真的达到，甚至超过了奥特曼所说的「博士级」AI。

虽然这次解决的问题还没有超过人类，但这种完全自主、自发现的能力苗头还是彰示了AI的能力。

这让我想起了流浪地球里的MOSS，也是自发现、自组织、自编程的AI。

Sebastien是一个很厉害的人。

他目前在OpenAI从事人工智能相关的工作。

![](https://img.36krcdn.com/hsossms/20250821/v2_ac5ee7358f3e424bb3e9ca9334c5294c@5091053_oswg214317oswg1080oswg422_img_000?x-oss-process=image/format,jpg/interlace,1)

在此之前，Sebastien曾担任**微软的副总裁兼首席科学家**，在微软研究院工作了10年（最初加入理论研究组）。

Sebastien还在普林斯顿大学担任了3年的助理教授。

在Sebastien的职业生涯的前15年里，他主要研究**凸优化**、在线算法以及机器学习中的对抗鲁棒性。

因这些研究工作**多次获得最佳论文奖**（包括STOC2023、NeurIPS2018和2021最佳论文奖、与微软研究院实习生合作获得的ALT2018和2023最佳学生论文奖、COLT2016最佳论文奖以及COLT2009最佳学生论文奖）。

他现在更加关注于理解**智能是如何在大语言模型中涌现的**，以及如何利用这种理解来提升大语言模型的智能水平，可能最终实现通用人工智能（AGI）。

Sebastien们将这种方法称为「AGI物理学」，因为他试图从不同的尺度（参数、神经元、神经元组、层、数据课程等）揭示AI系统各部分如何协同工作，从而产生这些模型惊人且出人意料的行为。

看起来，像Sebastien这样的数学家、科学家们正在致力于尝试破解大模型的黑箱之谜。

希望AI在拓展人类认知边界的同时，人类也能破解大模型的秘密。

**参考资料：**

https://x.com/Sebastien%20Bubeck/status/1958198661139009862

本文来自微信公众号[“新智元”](https://mp.weixin.qq.com/s/tX83wD5xXthk73jvh-5XxQ)，作者：新智元，编辑：定慧，36氪经授权发布。
