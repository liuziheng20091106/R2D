> id: https://www.appinn.com/one-million-screenshots/-full

> link: https://www.appinn.com/one-million-screenshots/

> title: One Million Screenshots 100

# One Million Screenshots 100
_Published on Mon, 11 Aug 2025 13:01:31 +0000_

**One Million Screenshots** 说：我们渲染（截图）了超过 100 万个互联网热门主页。

![One Million Screenshots - 这是真的！居然有人为 100 多万个网站截图，还放到了网上 1](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%20804%20350'%3E%3C/svg%3E "One Million Screenshots - 这是真的！居然有人为 100 多万个网站截图，还放到了网上 1")

这是一个挺离谱的网站。

打开[这个链接](https://onemillionscreenshots.com/?q=random)会随机看到一个网页的截图

`https://onemillionscreenshots.com/?q=random`

打开[这个链接](https://onemillionscreenshots.com/?q=appinn.com)，会直接打开 appinn.com 网站的截图。

`https://onemillionscreenshots.com/?q=appinn.com`

甚至，他们还有 API 可以直接显示图片：

`<img src="https://screenshotof.com/appinn.com" />`

效果是这样的：

![One Million Screenshots - 这是真的！居然有人为 100 多万个网站截图，还放到了网上 2](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%20512%20512'%3E%3C/svg%3E "One Million Screenshots - 这是真的！居然有人为 100 多万个网站截图，还放到了网上 2")

你可以[添加自己](https://onemillionscreenshots.com/add)的网站，不过是等待列表，不会立即加入

另外，每一个网站都有一些相关信息，比如[从这里](https://onemillionscreenshots.com/appinn.com)，可以看到：

![One Million Screenshots - 这是真的！居然有人为 100 多万个网站截图，还放到了网上 3](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201086%20559'%3E%3C/svg%3E "One Million Screenshots - 这是真的！居然有人为 100 多万个网站截图，还放到了网上 3")

以及历史截图、站点数据。

青小蛙看到 appinn.com 最早的截图来自2024年1月，一个月一张。

* * *

以下为 One Million Screenshots 的 Q&A：

这是什么？
-----

它是 1,048,576 个主页屏幕截图的集合，你可以一直放大。这是一种探索网络的奇怪而美妙的方式。它也是一个免费的 [API](https://onemillionscreenshots.com/docs)，用于将网站屏幕截图嵌入到您自己的项目中。

为什么存在？
------

我们想庆祝 Urlbox 在 2023 年为客户截取超过 1 亿张屏幕截图……所以我们认为每个月多拍 1,048,576 张屏幕截图会很有趣……我们有没有提到我们真的很喜欢屏幕截图。

它是如何制作的？
--------

该站点是使用 Next.js 和 Leaflet.js 制作的，并部署到 Cloudflare。屏幕截图是用 Urlbox 拍摄的。后期处理是在 Hatchbox 上运行的 Ruby 和 Vips 完成的。

它是什么时候制作的？
----------

我们于 2024 年 1 月 1 日开始为此截取屏幕截图。此后，我们在每个月的第一天都会截取更多屏幕截图。界面和后期处理作为一个副项目随着时间的推移而发展。

如何选择截图的网站？
----------

我们目前使用[通用爬虫网络图](https://commoncrawl.org/web-graphs)中按页面排名靠前的网站。排名最高的网站位于中心层，最低的网站位于边缘层。由于一个错误，您会在 0,0 发现不同的东西。

类似的主页如何运作？
----------

我们为每个屏幕截图创建了各种向量嵌入，以帮助检测异常和敏感内容。有些向量嵌入使用图像本身，有些则使用 URL 中的元数据和内容。

我们还使用这些嵌入，将相似的网站大致放置在屏幕截图每一层的相似区域（左/右/上/下）。这个人工智能目前还无法像你想象的那样持续地建立关联，但这可能是一种有趣的探索方式。

屏幕截图何时更新？
---------

每个月的第一天。可能需要几天时间才能进行后处理并将屏幕截图显示在地图上。

为什么我的主页无法通过 API 访问？
-------------------

我们目前仅通过免费 [API](https://onemillionscreenshots.com/docs) 提供顶级网站。您的可能会在未来几个月添加。您可以使用 [Urlbox](https://urlbox.com/) 呈现您喜欢的任何 URL 并在[此处](https://onemillionscreenshots.com/add)提交建议。

我可以添加我的网站吗？
-----------

还没有。但我们可能会在未来几个月扩展 – 每个月回来查看，您可能会找到它。

### 我可以在我的项目中使用屏幕截图吗？

是的。您可以从地图下载屏幕截图。您还可以使用 API 获取屏幕截图。我们只要求您链接回项目中的 Screenshot Of。

谁做的？
----

乔纳森·马克韦尔 （@[jot](https://x.com/jot)）、卢卡斯·维塞汉 （@[lukaswiesehan](https://x.com/lukaswiesehan)） 和克里斯·罗巴克 （@[cjroebuck](https://x.com/cjroeb)） 做到了这一点。

这到底是在哪里制造的？
-----------

在英国苏塞克斯、德国下萨克森州和英国约克郡。

* * *

原文：https://www.appinn.com/one-million-screenshots/

你要说这个东西有什么用？当然是#[真的没什么用](https://www.appinn.com/tag/%e7%9c%9f%e7%9a%84%e6%b2%a1%e4%bb%80%e4%b9%88%e7%94%a8/)啊！
