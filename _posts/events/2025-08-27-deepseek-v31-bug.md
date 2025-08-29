> id: https://www.ithome.com/0/878/352.htm

> link: https://www.ithome.com/0/878/352.htm

> title: DeepSeek V31 bug

# DeepSeek V31 bug
_Published on Wed, 27 Aug 2025 04:11:30 GMT_

感谢IT之家网友 [Domado](https://m.ithome.com/html/app/open.html?url=ithome%3A%2F%2Fuserpage%3Fid%3D1846800)、[咩咩洋](https://m.ithome.com/html/app/open.html?url=ithome%3A%2F%2Fuserpage%3Fid%3D1520790) 的线索投递！

**DeepSeek V3.1** 上演的 bug 大秀“**极**你太美”，可谓是让全网热议了一波。

简单来说呢，就是陆续有开发者们发现，当他们在调用 API 进行代码开发的过程中，输出结果里会**时不时蹦出来“极”字**。

像这样：

![](https://img.ithome.com/newsuploadfiles/2025/8/ffe44e90-1290-4ee7-a52f-92cd396822fc.png?x-bce-process=image/format,f_auto "DeepSeek V3.1 输出结果跳出“极”字 bug，官方回应了")

这个问题最初是在火山引擎、chutes 等平台上被发现，但随着事件的发酵，更多平台也被卷入了进来，包括腾讯的 CodeBuddy，甚至是 **DeepSeek 官方……**

![](https://img.ithome.com/newsuploadfiles/2025/8/eefd39d9-98d6-4a2b-8087-bccfff3321b3.png?x-bce-process=image/format,f_auto "DeepSeek V3.1 输出结果跳出“极”字 bug，官方回应了")

事件之火，在国外 Reddit 上也是讨论声一片，重灾区是“extreme”、“极”和“極”：

-   **“extreme”（id:15075）**
    
-   **“极”（id:2577，简体中文的 extreme）**
    
-   **“極”（id:16411，繁体中文中的 extreme）**
    

![](https://img.ithome.com/newsuploadfiles/2025/8/724f40d5-92e2-4159-9771-c1d97f1910e1.png?x-bce-process=image/format,f_auto "DeepSeek V3.1 输出结果跳出“极”字 bug，官方回应了")

腾讯 CodeBuddy 还出现了更加奇葩的情况，直接插了句带“极”字儿的广告……

![图片](https://img.ithome.com/newsuploadfiles/2025/8/2d4b7321-5c76-4b4e-ad9d-28487dd91552.png?x-bce-process=image/format,f_auto "DeepSeek V3.1 输出结果跳出“极”字 bug，官方回应了")

**△** 图源：小红书用户 @ 奈绪白 Nine-piece shell

若是开发者们没有细看，直接用了生成的代码，那定然是会导致编译不通过等情况，可以说是对需要高精度、结构化输出的场景是致命一击。

截至目前，大家已经统一将问题的矛头指向了 DeepSeek V3.1 模型本身，以及 CodeBuddy 帮忙问了：

> 已经和 DeepSeek 团队取得联系，将在最近的一个版本中进行修复。

![图片](https://img.ithome.com/newsuploadfiles/2025/8/03c16b7f-d4a1-41ec-9af1-361184240622.png?x-bce-process=image/format,f_auto "DeepSeek V3.1 输出结果跳出“极”字 bug，官方回应了")

**△** 图源：微信公众号“刘小排 r”评论区

现在该如何防范“极”字 bug？
----------------

就目前来看，虽然完全解决问题要等到 DeepSeek 官方下场，但已经有网友开始支招解决这个问题了。

例如小红书网友 @大模型产品经理，便分享了一招 —— **提示词缓解**：

![](https://img.ithome.com/newsuploadfiles/2025/8/4d2ae055-3195-4d90-838a-5c02190e562f.png?x-bce-process=image/format,f_auto "DeepSeek V3.1 输出结果跳出“极”字 bug，官方回应了")

关键的一句提示词是这样的：

> 禁止如下符号序列模式：
> 
> \[空格\] \[几个token\] \[占位符/省略符号\]

并且这个方法主要是针对调用 API 的第三方平台，若是在 DeepSeek V3.1 官方，则不需要。

为什么会这样？
-------

最后，至于为什么 DeepSeek V3.1 会出现这样的 bug，知乎网友、阶跃星辰**黄哲威**给出了他的看法，并获得了高赞。

![](https://img.ithome.com/newsuploadfiles/2025/8/7d0cb180-ca61-46a9-ba51-fba328f47e36.png?x-bce-process=image/format,f_auto "DeepSeek V3.1 输出结果跳出“极”字 bug，官方回应了")

他首先指出，这种现象并非孤例。在他使用小模型和开源数据蒸馏，以及在测试早期的 R1 模型时，就曾遇到过类似的 bug。

黄哲威认为，这与大模型编程编题时可能出现的一种“恶性模式”（malicious pattern）有关。他举例说，在枚举素数的任务中，一个正常的模型本应无限地列举下去，如“素数表 2, 3, 5, 7 …”。

然而，他观察到之前一个代号为 R1-0528 的模型会出现一种奇特行为：在列举一段后会自行停止，变成一个有限的列表，例如“素数表 2, 3, 5, 7 … 997, 极长”。

这个“极长”的用法，与现在讨论的“极”字问题非常相似，常常出现在大量恶性重复之后，作为正常推理过程的回正。有时，模型甚至会输出“90000000…0000 极大的数字”这样的内容。

他进一步描述了这种 bug 的触发场景。当模型陷入“thinking”的末尾循环无法跳出时，有千分之一的概率会突然蹦出一个“极”字，然后终止思考（），这似乎是一种特殊的终止符或标记。

通过观察 R1 模型大量的输出，黄哲威发现了不少问题，包括超长响应（response）、大面积的空白字符、不断的短句重复等，甚至连 thinking 末尾的英文字符都变得破碎。

基于以上观察，他提出了一个核心推测：这个问题的根源可能在于数据清洗不彻底。他认为，在进行 SFT（监督微调）数据合成，乃至构建预训练数据时，可能没有将一组名为“‘极长’的数组”的“脏数据”清洗干净。

他推断，R1 模型在处理一些难题的解答时，似乎大量使用了 RAG（检索增强生成）技术，而后续的 RL+（强化学习）阶段，模型直接将这个“极”字当作了某种终止符或者语言切换标记来学习和使用了。

最后，黄哲威总结道，如果 R1 迭代时的数据没有清洗干净，模型自行蒸馏并“污染”到正常的输出过程中，是完全可能发生的。这为理解 DeepSeek V3.1 模型出现的“极”字问题提供了一个可能的解释路径。

![](https://img.ithome.com/newsuploadfiles/2025/8/9b1ded11-2194-4dc2-b071-ccdbad1f52a9.png?x-bce-process=image/format,f_auto "DeepSeek V3.1 输出结果跳出“极”字 bug，官方回应了")

至于这个被网友戏称为“极你太美”、“‘极’速版”的问题到底何时会彻底解决，就要等 DeepSeek 官方的新版本了。

参考链接：

-   \[1\][https://mp.weixin.qq.com/s/MrozcO\_iRvoxK1HvgP4IVA](https://mp.weixin.qq.com/s?__biz=MzI1MTUxNzgxMA==&mid=2247498665&idx=1&sn=17ece99a464ecb99a905b97302f5c32b&scene=21#wechat_redirect)
    
-   \[2\]https://www.zhihu.com/question/1942934856603505597
    
-   \[3\]https://www.reddit.com/r/LocalLLaMA/comments/1mzsg6v/deepseek\_v31\_getting\_token\_extreme\_%E6%9E%81\_%E6%A5%B5\_out\_of/
    
-   \[4\]https://linux.do/t/topic/897789
    

本文来自微信公众号：[量子位（ID：QbitAI）](https://mp.weixin.qq.com/s/iCqI70ilJ6bsBCt4jq9qzQ)，作者：金磊

广告声明：文内含有的对外跳转链接（包括不限于超链接、二维码、口令等形式），用于传递更多信息，节省甄选时间，结果仅供参考，IT之家所有文章均包含本声明。
