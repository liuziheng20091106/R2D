> id: https://sspai.com/post/101859

> link: https://sspai.com/post/101859

> title: iPhone Pixel Google Tensor G5 GPU

# iPhone Pixel Google Tensor G5 GPU
_Published on Tue, 26 Aug 2025 06:46:22 GMT_

![Article Cover Image](https://cdnfile.sspai.com/2025/08/20/dc18a8fadc77cf8c9ecb214e5f7d72f8.png)  

几天前，Google 发布了 [Pixel 10](https://blog.google/intl/zh-tw/products/devices-services/pixel-10/) 系列产品，最引人关注的自然是由台积电代工的「纯血」[Tensor G5](https://blog.google/products/pixel/tensor-g5-pixel-10/) 芯片。

![](https://cdnfile.sspai.com/2025/08/21/5f2121f84ce9814a76681bdb032e24d2.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

2016 年，Google 推出了第一代 Pixel 手机，给用户带来最纯正的 Android 体验；2021 年，Google 和三星合作推出了 Tensor 芯片，虽有 Exynos 换皮之嫌疑1，但总归算是将 Pixel 的「自研」程度再提高了一个层次；2025 年，Tensor G5 芯片告别了 Exynos 换皮，也终于摆脱了害人不浅的三星工艺。

![](https://cdnfile.sspai.com/2025/08/20/2b42d0b2b9a4ee0fc801c3473db35dc5.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

值得关注的是，Tensor G5 的 GPU 部分采用了来自 Imagination 的 PowerVR 架构——你可能对这个名字有些眼熟——它曾和 Apple 一道走过 A 系列芯片的起步阶段，为 A4 到 A10X 等芯片提供了 GPU 解决方案，然后又突然被 Apple 抛弃，在多年艰难求生后熬到今天，再次登上了智能手机。

在科技发展的历程中，这样的故事其实已经足够精彩，但 Imagination PowerVR 的故事还远不止于此。

从 VideoLogic 到 Imagination
--------------------------

1985 年，Tony Maclaren 创立了一家名为 VideoLogic 的公司，为当时日益普及的 PC 与 Mac 开发用于增强电脑多媒体功能的拓展卡，在图形、声音加速、家庭音频系统、视频捕捉、视频会议系统等领域都有涉足。这为 VideoLogic 在视觉计算领域积累了早期的技术和市场经验，尽管这时公司的业务重心尚未触及后来的核心——3D 图形。

### 革命性 PowerVR 架构的诞生

公司历史的决定性转折发生在 1992 年，[Hossein Yassaie](https://en.wikipedia.org/wiki/Hossein_Yassaie) 加入 VideoLogic 公司担任技术总监。在 Yassaie 的推动下，VideoLogic 进行了一场大胆的战略转型，将目光投向了当时尚处于萌芽阶段的 3D 图形加速技术。此时 3D 图形加速仍是一个新兴技术，少数几家在市场上占据主导地位的公司都采用了简单直接但非常消耗计算资源的渲染方法。VideoLogic 团队意识到，他们可以通过一种更加灵活、高效的渲染方法在市场中杀出一条独特的道路。正是在这样的背景下，一个最终被命名为 PowerVR 的内部项目启动了。

![](https://cdnfile.sspai.com/2025/08/21/6e557faa4eaca195ffac6ade118f15b7.PNG?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/21/99ee9f12350dde61796edaf196816d34.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

当时主流的是 IMR 架构，即「立即模式渲染」(Immediat Mode Rendering)，基于「暴力计算」的逻辑按照图元（通常是三角形）被提交的顺序，对其进行立即处理与渲染。这意味着，即使一个物体最终会被另一个物体完全遮挡，GPU 仍需要花费宝贵的计算资源、占用紧缺的内存带宽来渲染这个「看不见」的物体。对于计算资源并不充足的 90 年代，此等浪费行径严重拖累了计算机的图形性能。

PowerVR 的核心理念是 TBDR ，即**「分块延迟渲染」(Tile-Based Deferred Rendering)**，其渲染过程可以分为两个主要阶段：

1.  **几何处理与分块（Tiling）**：GPU 在接收整个画面的所有数据后，会将其划分为一个个小的矩形区域（图块，Tiles），并生成一个列表以精确记录每个图块内包含了哪些三角形图元；
2.  **延迟渲染（Deferred Rendering）**：在完成几何处理与分块后，GPU 才会开始逐个图块地进行像素渲染，且在渲染每个图块前都会执行一次 HSR （隐藏面移除，Hidden Surface Removal），比较图块内所有图元的深度信息，只将最终可见的像素发送到后续渲染管线进行着色与纹理处理。

![](https://cdnfile.sspai.com/2025/08/21/687fc683bad8ff587ead95d3ddefefc4.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/21/e66fbc404cadda0bfa3d28071ea8144a.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

这一技术显著提高了渲染效率，大幅降低了功耗与对内存带宽的需求，后来成为 Imagination 公司的标志性创新与核心竞争力。如果感兴趣的话，你也可以在 Imagination 官网上阅读[《 PowerVR Architecture Overview 》](https://docs.imgtec.com/starter-guides/powervr-architecture/html/architecture-overview-index.html)。

1993 年，PowerVR 架构的 FPGA 演示版本在当年的计算机图形学顶级会议 SIGGRAPH 上进行了秘密展示，初步验证了其发展潜力。一年后，VideoLogic 成功在伦敦证劵交易所上市，为后续技术研发与市场扩张筹集了资金。

### 从 PC 与游戏主机，到 IP 授权模式

在确立了 PowerVR 架构在技术上的优势后，VideoLogic 开始将其商业化，首先便瞄准了 PC 市场。他们采取了与半导体制造商合作的模式，将其技术授权给 NEC 等合作伙伴，由后者负责芯片的生产与销售。在 Matrox M3D 和 Apocalypse 3Dx 等当时颇受欢迎的显卡产品中，都跳动着 PowerVR 的脉搏。

![](https://cdnfile.sspai.com/2025/08/21/405fccd9f82f7ae41343b5803754a5ec.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

NEC PowerVR PCX2 (1997)

21 世纪初，他们又与意法半导体（ST Micro Electronics）、大力神（Hercules）合作，推出了基于 PowerVR Series3 架构的 Kyro II 芯片，并应用在 3D Prophet 4500 显卡上，以低于 NVIDIA GeForce 2 的价格实现了更强的性能，取得了商业上的成功。

但真正让 PowerVR 声名鹊起的，是其在游戏主机领域的辉煌战绩。上世纪 90 年代末，世嘉 Sega 正在为下一代游戏主机 Dreamcast 寻找 GPU 技术，最终放弃了当时在 PC 市场如日中天的 3dfx Voodoo 架构，选择了 PowerVR Series 2 GPU 方案。该方案同时用于世嘉的 Naomi 街机，这使得开发者可以轻松将《能量宝石》《死亡之屋 2 》等街机热门游戏移植到家用 Dreamcast 主机上，也创造了 Dreamcast 的另一个核心卖点。

![](https://cdnfile.sspai.com/2025/08/21/6d6d0dcd39f3e2b561c1d8fa6a8dff25.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/21/a198239d1f2260238e417e2f4b9e1109.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Dreamcast 于 1998 年在日本发布，其惊艳的图形性能使其被誉为「领先时代」的作品。到 1999 年，NEC 已经向世嘉出货超过一百万颗 PowerVR 2DC 芯片。Dreamcast 最终总销量超过了一千万台，极大巩固了 PowerVR 的行业地位。

在与世嘉的合作取得巨大成功的同时，VideoLogic 公司的管理层——尤其是 1998 年升任 CEO 的 Yassaie ——作出了另一项影响深远的战略决策。他们意识到，公司的核心价值在于独一无二的技术与知识产权，而非（与其他厂商合作完成）硬件制造。因此他们决定，**公司将从销售自有品牌硬件的模式转型至 IP 开发与授权模式**。

![](https://cdnfile.sspai.com/2025/08/21/1d78dbfefd2b7c87e32b6d5292513e39.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

1999 年，VideoLogic 更名为 Imagination Technologies ，专注于设计 GPU 核心，再将这些设计作为 IP 授权给德州仪器、三星等半导体公司，由他们将 PowerVR GPU 集成到他们设计、生产的 SoC 中。这种商业模式与英国另一家半导体巨头，大名鼎鼎的 ARM 公司如出一辙。这使得他们能够将资源集中于最擅长的研发环节，同时也有利于将其技术推广到更加广阔的市场中。

### 第一个「超级客户」的崩溃

鸡蛋不能放在一个篮子里，建立在单一支柱上的商业成功往往是脆弱的。

世嘉 Dreamcast 虽然在技术上备受赞誉，但在商业上未能抵挡住索尼 PlayStation 2 的强大攻势，最终于 2001 年 3 月 31 日——恰好是 Imagination 财年的最后一天——宣布停产，这一事件对 Imagination 造成了非常沉重的打击。

![](https://cdnfile.sspai.com/2025/08/21/1f4edc9901661a827fc1fb33ae67742f.avif?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

与世嘉的授权协议是公司当时最大的收入来源和利润引擎，被形容为 The Big Cash Cow（现金牛），世嘉的败退直接导致 Imagination 的年利润暴跌了 30% 。这次冲击不仅是财务上的挫折，更深层次地暴露了 Imagination 商业模式中的一个致命弱点：**对单一「超级客户」的过度依赖**。

可惜的是，人类能从历史中学到的唯一经验，就是什么都没学到。Imagination 没有预料到的是，历史将在 16 年后以一种更加毁灭性的方式重演。

移动 GPU 霸主的黄金枷锁
--------------

在经历世嘉 Dreamcast 停产的阵痛之时，Imagination 做出了一个关键且正确的决定：将业务重心从 PC 和游戏主机市场，转向当时方兴未艾的移动领域。他们正确地预见到，硬件 3D 加速将在未来的移动设备上扮演至关重要的角色，而 **PowerVR 架构低功耗、高能效的设计理念，与移动设备对电池续航和散热的严苛要求完美契合。**

![](https://cdnfile.sspai.com/2025/08/20/d754a8b50f7355386ec6a79a95ec4a68.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/20/8287424ec5bc2539cc0858a47cbfb02e.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Imagination 的技术为诺基亚 N95 和索尼爱立信 P1 等早期手机产品与 PlayStation Vita 等掌上游戏机带来了不俗的表现，证明了 PowerVR GPU 在移动和便携设备领域的领先地位。

### 成也「MFi」，败也「MFi」

2007 年，乔布斯在舞台上发布了初代 iPhone ，「重新定义了智能手机」。初代 iPhone 搭载了三星蜂鸟 S5L8900 芯片，采用 90nm 工艺制程、ARM11 核心与 PowerVR MBX-Lite GPU 。一段长达十年、既成就了 Imagination 也最终几乎摧毁了它的合作关系，就此开始。  

![](https://cdnfile.sspai.com/2025/08/20/article/db3521e7fa8a84e334e86d9afc60abab.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

乔布斯与初代 iPhone

2010 年，iPhone 4 发布。在其搭载的 Apple 自研2A4 处理器中，与前三代 iPhone 上使用的三星蜂鸟芯片一样集成了 PowerVR GPU ，型号为 SGX535 。此后七年间的 A 系列芯片都一直使用着 PowerVR GPU ，实现了优于同代竞品的性能表现。

Apple SoC

GPU

代表设备

年份

A4

PowerVR SGX535

iPhone 4, iPad

2010

A5

PowerVR SGX543 MP2

iPhone 4S, iPad 2

2011

A5X

PowerVR SGX543 MP4

The New iPad

2012

A6

PowerVR SGX543 MP3

iPhone 5, iPhone 5c

A6X

PowerVR SGX554 MP4

iPad 4

A7

PowerVR G6430 MP4

iPhone 5S, iPad Air

2013

A8

PowerVR GXA6450 MP4

iPhone 6

2014

A8X

PowerVR GXA6850 MP8

iPad Air 2

A9

PowerVR GT7600 MP6

iPhone 6s, iPhone SE

2015

A9X

PowerVR GT7800 MP12

iPad Pro

A10 Fusion

PowerVR GT7600+ MP6

iPhone 7

2016

A10X Fusion

PowerVR GT7800+ MP12

iPad Pro 2

2017

随着 iPhone 和 iPad 在全球范围内的火爆，Imagination 的 IP 授权费和版权收入呈爆炸式增长。公司的股价随之飙升，一时成为资本市场的宠儿。但 Imagination 不知不觉给自己埋下了一颗定时炸弹，它们一半以上的营收来源于 Apple ——或许我们可以戏谑地将这段时间称作 PowerVR 的「MFi3」时代。

![](https://cdnfile.sspai.com/2025/08/21/d0cc239195133246d0b1f18162aafeb1.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

发布于 2017 年 6 月的 A10X Fusion 集成了 PowerVR GT7800+ 12 核 GPU ，也是最后一代采用 PowerVR GPU 的 A 系列芯片

这种极端依赖与 Apple 对自研越来越强的渴求之间，显然存在着无可避免的冲突。一旦 Apple 这个超级客户离开 Imagination ，对于 Imagination 来说将会是灭顶之灾，冲击力甚至强于前面提到的 21 世纪初与世嘉合作终止一事。

2017 年 4 月 3 日，也许是 Imagination 历史上最黑暗的一天。Imagination 发布公告称，Apple 已正式通知，计划在未来 15 至 24 个月内停止在其新产品中使用 Imagination 的知识产权。而 Apple 给出的理由是，其「**正在开发一种独立、自主的图形设计，以更好掌控产品**」。

重磅炸弹落下，资本市场瞬间被引爆。当天 Imagination 的股价暴跌 70% ，市值蒸发达数亿英镑。分析机构将 Imagination 的股票评级下调至无法投资（Uninvestable），几乎相当于宣告了一家上市公司的死刑。

![](https://cdnfile.sspai.com/2025/08/23/96be95cc9e844dce9796fd4dee4428af.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Imagination 迅速作出反应，发表了一份措辞强硬的公开声明，向宣称「将在两年内停止使用 Imagination 的技术」的 Apple 发出质疑——「从零开始设计一个全新的 GPU 架构而不侵犯其专利、知识产权和机密信息，是极具挑战性的」。Imagination 要求 Apple 提供未侵权的证据，但要求被 Apple 拒绝，双方矛盾进一步激化并逐步公开。这场纠纷的背景更为复杂——在此之前 Apple 试图收购 Imagination 未果，且正在持续从 Imagination 挖走其 GPU 核心工程师设立自己的研发团队—— Apple「背叛」Imagination 是蓄谋已久的。

### 插播一则收购旧闻

失去了 Apple 这个最大的收入来源后，Imagination 的财务状况迅速恶化，公司运营难以为继。在内外部的巨大压力下，公司于 2017 年 6 月宣布将整体出售，并于同年 11 月被具有国资背景的私募股权基金 Canyon Bridge 收购。

![](https://cdnfile.sspai.com/2025/08/23/05314c478b4bed39ddd315bf2072a192.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

为了确保这笔交易能够顺利完成，Imagination 先向美资的 Tallwood Venture Capital 出售了其 2012 年收购而来的 MIPS 处理器业务，巧妙分离了其位于美国的 MIPS 业务与位于英国的 GPU IP 资产，以脱离 CFIUS （The Committee on Foreign Investment in the United States ，美国外国投资委员会）的管辖范围，规避地缘政治风险。此前，CFIUS 就以国家安全为由，阻止了 Canyon Bridge 对莱迪思半导体（Lattice Semiconductor）的收购。   

苟延残喘，何处寻觅又一春？
-------------

俗话说得好，事不过三。在两次因过度依赖单一超级客户而陷入谷底之后，拆分收购后的「新」Imagination 逐渐推行积极多元化发展战略，以降低「爆雷」风险、开拓新的增长市场。新  Imagination 的业务主要聚焦于其四大战略支柱：汽车电子、数据中心与桌面计算、移动设备 GPU 以及边缘侧 AI 与计算。

![](https://cdnfile.sspai.com/2025/08/23/146d2843d43fb0d0e47948e4bb3c3064.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

 2020 年 1 月 2 日，传来了一则令人疑惑的消息：Imagination 官方宣布与 Apple 达成新的多年期授权协议——当然，这得交钱，对于 Imagination 来说也算是一笔不小的收入。有人说，这表示「分手」时高调宣称「将在两年内停止使用 Imagination 的技术」的 Apple 终于低头了。

从零开始自研 GPU 并不容易，哪怕是富可敌国的 Apple 也很难做到。A11 的 GPU 设计就与此前 Imagination 的 Rogue 非常类似，A12 的 GPU 也依然支持 PVRTC （PowerVR 纹理压缩， Imagination 的专利技术）。直到今天，A 系列芯片中的 GPU 都无法完全脱离 Imagination PowerVR 的技术——不过既然双方重归于好签订 IP 授权合约了，这也无伤大雅。

![](https://cdnfile.sspai.com/2025/08/23/521e9d81defb9687d31507936470ee57.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/23/f45e32e9b2f1d0c40f68fd5909b3e1ad.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

手头宽裕一些后的 Imagination 于 2021 年宣布重返 CPU 市场，基于开放标准的 RISC-V 架构推出了 Catapult 内核家族。他们希望自身不再仅仅是一个 GPU IP 供应商，而能转型成为一家更完整的 CPU + GPU + AI 异构计算平台解决方案提供商。但事与愿违，市场给予他们的反馈并不好。今年年初，Imagination 宣布将停止开发 RISC-V CPU 内核，以更好专注于传统与 AI 业务——说人话就是不挣钱，砍了。

那 Imagination 的老本行 PowerVR GPU 又情况如何呢？

在智能电视、智能穿戴、开发板等品类中，PowerVR 并不少见。例如，设计优雅的 LG U+ TV Soundbar 音响中就是 PowerVR Series 9 XE 的 GPU ，一款很有趣的开源掌机 Retroid Pocket 3 搭载的虎贲 T310 也采用了 PowerVR GE8300 GPU 。

![](https://cdnfile.sspai.com/2025/08/24/03875c948010111e1285d7a84350fb28.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/24/7047bb553fe7a81b163cbccdf5ec8174.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

而在 PowerVR 曾叱咤一时的手机市场，情况就不太乐观了。

在与 Apple 度蜜月时，Imagination 总是把最新一代、最高规格的 GPU 独家授权给 Apple 使用，而其他厂商则只能使用较低规格甚至是上一代方案。其他厂商感受不到 Imagination 的合作诚意，因而也缺少与之深入合作的经验和意愿。这样一来，自从 A10X 之后，PowerVR 8 系和 9 系 在市面上就再也找不到高端用例了；甚至在 2020 年中低端的联发科 Helio P95（搭载 PowerVR GM9446 MP2）之后的很长一段时间内，手机行业的主流视线里都没有出现过使用 PowerVR GPU 方案的 SoC 。

![](https://cdnfile.sspai.com/2025/08/23/febac86e0c49ac42daac343c2b5e6169.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/23/d4529ff326df4e2b457a1d45c8fc447b.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

不过嘛，在查阅资料的过程中，我有了些意外而惊喜的发现。

在 9 系之后，PowerVR GPU 改用字母表示代数，目前最新的是 E 系。很多人都知道，摩尔线程的 S70 、S80 等显卡产品中便使用了 PowerVR Series B XT 的 IP 授权；而我们还可以从 Imagination 在今年三月公布的授权信息得知，PowerVR Series D XT 被授权给了当时还未发布的 Google Tensor G5 与「另一款小米玄戒」。众所周知五月登场的玄戒 O1 搭载的是 ARM Mali GPU ，那么这款 PowerVR 版玄戒又是什么呢？实验室中玄戒 O1 的废案？

![](https://cdnfile.sspai.com/2025/08/23/5d66fede63d57d73f05cc39722708da7.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

Imagination Tech 官方公众号在今年三月揭露了相关信息

虽然有 Tensor G5 和「废案」玄戒选择了 PowerVR 方案，但我们依然无法对 PowerVR 回归主流手机市场抱有太大希望，高通以外的 SoC 厂商没有理由不选择更加成熟的 ARM Mali 方案。

2020 年 3 月 Google 推出 Android GPU Inspector（安卓 GPU 监视器）时，首批只支持了高通的 Adreno 与 ARM Mali 产品，一个月后才与 Imagination 合作补上了对所剩无几的 PowerVR GPU 的支持，仿佛 PowerVR 早已被 Android 生态遗忘、低人一等；诸多游戏往往也只针对 Adreno 和 Mali 适配、优化，PowerVR 在兼容性上存在着很大的问题。——何况 PowerVR 如今的「高端」产品性能与功耗表现如何也是一个谜，刚刚问世的 Tensor G5 上搭载了 PowerVR DXT-48-1536 GPU ，可图形性能跑分表现甚至不如上代顶着三星工艺 debuff 的 Tensor G4 。

![](https://cdnfile.sspai.com/2025/08/24/5d3aed7cbe285570cfc7babd5304304a.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/24/dba2b47f7ac8dcf9296cdfd4617b70ac.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

另一个试图打破 Adreno 与 Mali 二分 Android 的局面的是三星，还拉来了 AMD 合作，把 RDNA2 架构改造成了手机 SoC 上的 Xclipse GPU ，最终却只落下了「高分低能」的结局。

据传三星将终止与 AMD 的技术合作转而「自研」下一代 GPU ，但这里的「自研」会不会是「回归」Exynos 曾使用过的 Mali 呢？暂且存疑。

![](https://cdnfile.sspai.com/2025/08/24/ebe36ea8b1e97510a0a9e5901d4c3239.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)![](https://cdnfile.sspai.com/2025/08/24/34bc3bc3f447daaf5356753a744e3134.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

话又说回来，Pixel 作为 Google 的「亲儿子」都用上了 PowerVR GPU ，那么 Android 必然将从系统层面优化 PowerVR GPU 的性能表现与兼容性；且考虑到 Pixel 在最近几年稳中向好的销量，Imagination 应该能从中获取比较丰厚的利润来投入下一代的研发。这样一来，PowerVR 还真有可能焕发第二春，成为 Android 生态下 GPU 的一种「新」选择。

![](https://cdnfile.sspai.com/2025/08/24/055d92e4d9b27dcd651c17b2ac3ec7e8.jpeg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

有趣的是，今年年初又传出了 Canyon Bridge 打算出手 Imagination 的消息。不得不说，Imagination 不仅写下了一部 GPU 技术演进的编年史，更上演了一场展现出惊人韧性的商业戏剧。谁都无法预料 PowerVR 未来的走向，正如（上文提到的、带着戏谑的）人类从历史中学不到任何教训。
