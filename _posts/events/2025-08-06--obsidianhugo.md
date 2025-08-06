> id: https://sspai.com/post/101376

> link: https://sspai.com/post/101376

> title: ObsidianHugo

# ObsidianHugo
_Published on Wed, 06 Aug 2025 03:31:20 GMT_

![Article Cover Image](https://cdnfile.sspai.com/2025/07/28/40019b62bdbedabab35ca9b7865e9adb.png)  

**Matrix 首页推荐** 

[Matrix](https://sspai.com/matrix) 是少数派的写作社区，我们主张分享真实的产品体验，有实用价值的经验与思考。我们会不定期挑选 Matrix 最优质的文章，展示来自用户的最真实的体验和观点。   
文章代表作者个人观点，少数派仅对标题和排版略作修改。

* * *

Obsidian to Hugo 工作流
--------------------

Hugo 允许我们使用 Markdown 格式进行写作，并自动转换为静态网站，Markdown 编辑器可以自由地选择。我使用的是 Obsidian 编辑器，将`.md`文件同步至 HomeServer 后，在 Linux 环境中构建并预览网站，最终 Push 至 Github 并由 Cloudflare 解析。这样的工作流并无可说道之处，但是其中的附件（图片、视频）的处理是比较麻烦的，常规的处理办法有：

-   使用 Markdown 风格链接附件，并随项目上传至 Github 仓库；
-   写作时使用图床（图床服务、OSS 等）托管图片并在`.md`文件中以 Markdown 风格插入链接。

不管哪种方法，在写作时都是不够流畅的，在前期、后期还可能要处理图像的压缩问题，当然我们可以引入第三方的工具比如[WebP Cloud Services](https://webp.se/)，但有悖于我用 Cloudflare 一把梭哈的理念1，且无法解决 CF 的 R2 免费存储空间（10GB）可能不足的问题。

为了让`Obsidian - Hugo`的写作、发布流更加顺畅，我之前使用脚本在本地（HomeServer）转换 Obsidian 的 WiKi 链接（双方括号）并压缩图像自动上传至 CloudFlare R2。有 24 小时在线的 HomeServer 辅助，这套流程允许我在全平台同步写作、插入附件，足够流畅。但使用过程中发现，固定的压缩设置使得一些照片质量有明显的下降，而对于一些画面简单的图片，体积似乎还有压缩的空间。

因此，`Obsidian - Hugo`自动化发布的核心在于解决多媒体附件（主要是图片）问题，即自动转换附件链接、自动优化图片体积与质量、自动上传 OSS。

![](https://cdnfile.sspai.com/2025/07/27/0e692f352b2eaea4376e5979fcc09fb2.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

> 图像优化既是一门艺术，也是一门科学：说它是一门艺术，是因为单个图像的压缩并不存在明确的最佳方案，说它是一门科学，则是因为有许多发展成熟的方法和算法都能够显著缩减图像的大小。找到图像的最佳设置需要在许多方面进行认真分析：格式能力、编码数据的内容、质量、像素尺寸等。
> 
> —— Google Web Fundamentals

图像尺寸的确定
-------

首先要确定目标尺寸宽高，高清原图超大的尺寸对于 Web 浏览来说是无意义的2，浏览器会根据 css 样式和设备屏幕自动缩放图像，与其让浏览器对图像降采样，不如在服务端完成，如此可以有效减小存储体积并提高网站加载速度。

应对多设备的最佳画质图片问题，可以通过优化单张图片，或者准备数张不同尺寸的图片并根据设备自动选择。为了在有限容量的 R2 存储桶中尽可能多地存储文件，我们还是采用优化单张图片的路线。因此首先要确定图片的宽高尺寸应该设置为多大。

### 图像元素

根据 hugo-book 的样式源码：

```
// /themes/hugo-book/assets/_defaults.scss
$font-size-base: 16px !default;
$font-size-16: 1rem !default;
$body-min-width: 20rem !default;
$container-max-width: 80rem !default;
$menu-width: 16rem !default;
$toc-width: 16rem !default;
```

`1rem`对应`16px`，因此有效画布的最大尺寸为`80*16px=1280px`，其中菜单`menu`和标签`toc`的组件宽度固定为`16rem`，对于横向分辨率大于`1280px`的浏览器，两边自动留空。在网站的`正文`区域，最大横向显示尺寸为`(80-16-16)*16px=768px`，由此我们初步确定`正文`插图的最大的横向尺寸为`768px`，其它容器中的图像尺寸也可以在 css 样式中查到，或者直接通过浏览器`开发者模式`(`ctrl+shift+c`)并用样式拾取器查看。

![](https://cdnfile.sspai.com/2025/07/27/675783932c16d45c038bdd66bdfb924b.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

对于移动端，我们在浏览器`开发者模式`中模拟移动设备（`Device Toolbar`），可以看到一些预设的设备尺寸，比如`Samsung Galxy S20 Ultra`的尺寸为`412*915px`。然而，如果我们将图像降采样为`412px`像素，会感到模糊不清，`412px`也远低于真实的屏幕分辨率。这和浏览器渲染网页使用的是「CSS 像素（viewport）」而非物理像素有关，例如 Galaxy S20 Ultra 的 CSS 像素为`412px*915px`，物理像素为`1080px*2400px`(FHD+模式)，比值 Device Pixel Ratio (DPR)为 2.62。

### 设备 DPR

在像素密度较高的设备（如 Retina 显示器）上，DPR 大于 1（例如 2、3 甚至更高）。 这意味着单个 CSS 像素将由多个物理像素表示，从而产生更清晰的图像和文本。从本质上讲，DPR 允许 Web 开发人员使内容适应不同的屏幕分辨率，确保图像和文本在各种设备上显示清晰且大小合适。例如在 hugo-book 主题中，通过布局断点`$mobile-breakpoint`来进行移动端适配，`$mobile-breakpoint`的默认值为`56rem`即`896px`。

```
$mobile-breakpoint: $menu-width + $body-min-width * 1.2 + $toc-width !default;
@media screen and (max-width: $mobile-breakpoint) {
  .book-menu {
    visibility: hidden;
    margin-inline-start: -$menu-width;
    z-index: 1;
  }
...
```

但是，我们仍应准备等于或略高于`CSS 像素 * DPR`的图像，这样才能在高清屏（高 DPR）下显示清晰。在移动端，我们也可以简单地直接取物理像素为参考值（即不考虑边距）。

目前，移动端的高分屏已达`1440px`，我们就取这个作为移动端的尺寸上限。在桌面端，由于高分屏的普及，DPR 也随移动端一样水涨船高，比如 4k 屏和 iMac Retina 屏幕，这类屏幕的 DPR 一般可达 2。因此，综合现有硬件和 hugo-book 模板的设置，我们应该准备的插图横向尺寸不应小于`1440px`和`768*2=1536px`。我们将博客中不同种类的图的最大尺寸计算出来，以最终的`综合尺寸`为目标像素值。

图像类型

CSS 像素/px

移动端最大尺寸/px

DPR(desktop)

综合尺寸/px

banner

768

1440

2.0

1536

插图

614

1440

2.0

1440

双栏插图

332

720

2.0

720

卡片插图

120

360

2.0

360

正确地截图
-----

相机/手机拍摄的图像分辨远远超过参考像素值，我们对其进行降采样处理。但如果网站中有大量的屏幕截图，其原始尺寸可能就比参考像素低了，当然我们可以对其进行超采样，但这件事放在前期做效果会更好。

在浏览器中，直接通过`ctrl+鼠标滚轮`对窗口放大（chrome 最大可以至 500%），再对目标进行截图就可以得到分辨率更高的图了。桌面环境（win11），可以通过`系统` - `屏幕` - `缩放和布局` 增加缩放比例，让小元素放大显示。

以截本站侧边栏状态图为例，该组件的 CSS 像素宽度为`224px`，2k/25 寸屏的缩放率一般为 150%，若直接屏幕截图得到的图片宽度为`336px`，放在正文中（768px 宽度）显然是不够的，我们直接将浏览器放大 500%，就可以截到宽度近`1700px`的图，对比如下。

![](https://cdnfile.sspai.com/2025/07/27/7be4c9028ce536db46d6b2cb96f536fc.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

重采样、格式、质量
---------

python 的`Pillow`库可以快速实现图像缩放、压缩和保存。其重采样默认算法为`BICUBIC`，我们对时间不敏感，因此直接显式指定质量最高的`LANCZOS`插值3。

```
img = img.resize((w, h), resample=Image.Resampling.LANCZOS)
```

在保存时，可以进一步选择格式、压缩率和质量。

```
img.save(output_path, format="WEBP", method=6, quality=quality)
```

显式指定速度最慢但压缩率最高的`method=6`，尽可能地降低文件大小。

显式指定格式`format="WEBP"`。WebP 支持有损压缩与无损压缩，且支持动图和 Alpha 透明通道。平均而言，WebP 的文件大小比同类 JPEG 图像减少了 30%。时至今日，`Webp`格式已经得到绝大多数浏览器支持（仅 IE 不支持）4。博客网站完全可以统一使用 Webp 格式图像。

![](https://cdnfile.sspai.com/2025/07/27/3102f54a1d05edd94aec55aa294b3241.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

`quality`极大地影响文件体积和质量，一般来说取值`60-80`就能平衡好`质量 - 体积`这对矛盾。大多文章也就介绍到这了，以一个较为普适但固定的参数来应对所有场景。但我在实践中发现，固定的`quality`取值经常造成图像压缩过度或不足，而用肉眼去评估图像质量显然是低效的。

![](https://cdnfile.sspai.com/2025/07/27/f626595098d1eacc7465f1ec87759a01.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

图像压缩与质量评价
---------

### 评价指标

为了在保证质量的同时，根据每张图片的具体情况最大化地压缩图像体积，要引入评价标准，主观地来说，可以通过以下几点，但无法量化差异：

-   是否模糊、失真（如文字边缘锯齿、细节丢失）；
-   色彩是否偏差、对比度是否异常；
-   压缩伪影（如马赛克、块效应、色带）；

尝试使用 NeRF 常用的评价指标来协助量化差异。

**指标**

**全称**

**原理**

**含义**

**优点**

**缺点**

**PSNR**

Peak Signal-to-Noise Ratio 峰值信噪比

基于 MSE（均方误差）计算信号强度与噪声强度的比值

误差越小，PSNR 越高，代表压缩图像越接近原图

简单快速，历史最悠久

无法反映结构、感知差异；对视觉不敏感

**SSIM**

Structural Similarity Index 结构相似性

模拟人眼对亮度、对比度、结构的感知

更符合人眼感知的结构对比

考虑结构相似性，视觉友好

对多尺度、大范围失真不敏感

**MS-SSIM**

Multi-Scale SSIM 多尺度结构相似性

多分辨率下计算 SSIM，增强全局感知

比 SSIM 更稳定地反映感知质量

比 SSIM 更接近人类主观评分

计算复杂度比 SSIM 稍高

**LPIPS**

Learned Perceptual Image Patch Similarity 感知图像差异

基于深度学习，使用特征空间距离计算感知相似度

越小越接近，越大越不相似

最贴近人眼感知，处理模糊、结构变形效果好

依赖模型，速度慢

实际操作，同时使用 MS-SSIM 和 LPIPS 来评价图像质量，分别设置阈值为`0.98`和`0.02`，通过搜索`quality`的值来获取最佳设置。我测试了博客中的 20 张图片，前 6 张为手机拍摄的照片，后 14 张则包含了电子书插图、屏幕截图、线稿图、PPT 合成图等。以`quality=80`作为参考值，由结果可以看到，自适应的`quality`选择范围很大，10-86 都有；20 张图的平均结果，自适应方法节省空间 84.81%，固定质量（80）则为 81.69%。虽然总的来看空间节省差距不大，但可以初步看出，「照片」所需的`quality`要比截图、线稿要大一些，且分辨率越大的图，`quality`也会偏大；而画面干净的图`quality`可以很小，比如`7.png`，`9.png`，`10.png`，`19.jpg`。

文件名

原始

自适应

Q=80

质量 Q

MS-A

LPIPS-A

MS-Q80

LPIPS-Q80

1.jpg

425.7KB

150.5KB

185.7KB

71

0.9924

0.0191

0.9944

0.0104

2.jpg

2175.4KB

163.7KB

235.5KB

63

0.9898

0.0199

0.9926

0.0120

3.jpg

559.1KB

206.1KB

159.9KB

85

0.9913

0.0191

0.9885

0.0325

4.jpg

537.9KB

177.9KB

146.7KB

84

0.9907

0.0193

0.9889

0.0248

5.jpg

660.3KB

336.2KB

291.1KB

83

0.9912

0.0177

0.9884

0.0276

6.png

1183.5KB

67.5KB

50.9KB

86

0.9915

0.0197

0.9882

0.0309

7.png

288.1KB

61.5KB

146.5KB

12

0.9859

0.0186

0.9962

0.0041

8.jpg

232.1KB

37.9KB

55.2KB

56

0.9892

0.0200

0.9945

0.0074

9.png

101.8KB

12.0KB

26.0KB

13

0.9888

0.0185

0.9976

0.0030

10.png

200.6KB

16.7KB

41.8KB

12

0.9893

0.0189

0.9987

0.0020

11.png

159.8KB

14.8KB

26.1KB

33

0.9881

0.0197

0.9958

0.0053

12.png

402.3KB

163.4KB

147.2KB

83

0.9803

0.0072

0.9792

0.0097

13.png

128.2KB

8.9KB

16.4KB

25

0.9852

0.0179

0.9901

0.0072

14.png

925.1KB

83.1KB

155.3KB

31

0.9844

0.0197

0.9926

0.0086

15.png

642.8KB

61.8KB

114.4KB

40

0.9854

0.0198

0.9924

0.0085

16.png

749.8KB

37.4KB

38.9KB

79

0.9955

0.0188

0.9957

0.0166

17.png

880.0KB

25.1KB

38.9KB

52

0.9905

0.0193

0.9940

0.0076

18.png

523.0KB

35.1KB

41.9KB

76

0.9916

0.0182

0.9933

0.0145

19.jpg

444.8KB

53.8KB

126.7KB

10

0.9911

0.0157

0.9995

0.0009

20.jpg

331.1KB

41.4KB

69.6KB

16

0.9933

0.0189

0.9983

0.0037

**总和**

**11551.3KB**

**1754.8KB**

**2114.6KB**

 

 

 

 

 

### 与在线工具的对比

有很多在线图像压缩工具或 CDN 提供了图像优化服务，来试试我们的压缩效果与之相比如何5。[WebP Cloud Services](https://webp.se/)和 [TinyPNG](https://tinypng.com/)的压缩率选择有较大的差别，WebP Cloud Services 的质量较好，TinyPNG 的压缩率较大。我们无法精细地调试这些在线工具的压缩参数，本地的灵活性则较高，通过参数的调试可以达到同样的效果。最终，根据我们设定的 MS-SSIM 和 LPIPS 阈值，使用`quality=85`获得了 42.5KB 大小的最终文件，而原文件大小 599.0KB。

 

quality=93

WebP Cloud

quality=75

TinyPNG

quality=85

SIZE /KB

75.8

75.7

28.4

28.6

42.5

PSNR /dB

42.82

41.83

37.89

35.27

40.10

SSIM

0.9846

0.9782

0.9598

0.9595

0.9716

MS-SSIM

0.9969

0.9954

0.9903

0.9890

0.9937

VIF

0.8806

0.8513

0.7720

0.7661

0.8279

LPIPS

0.0055

0.0074

0.0263

0.0260

0.0198

链接转换与文件上传
---------

把图片的压缩问题解决后，剩下的就很简单了：

-   使用正则表达式匹配 markdown 文件中的链接（WiKI 和 Markdown 风格）；
-   分类，判断类型：静态/动态图片、视频、本地/外链/站内链接；
-   根据分类进行降采样、压缩，移除元数据；
-   生成唯一文件名，保存至本地，将 markdown 文件中的链接替换为标准图像引用格式；
-   将压缩参数、文件名映射保存至数据库。

![](https://cdnfile.sspai.com/2025/07/27/42fa1fd997f97bf8924a63386881cbd0.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

以下是几种正则匹配的样式和转换后的样式：

```
![](image_filename | url)
[](image_filename | url)
![[image_filename | url]]
[[image_filename | url]]
>>>>>Transfer to>>>>>
![](https://img.osnsyc.top/XXXXXX.webp)
```

```
banner: [[image_filename | url]]
>>>>>Transfer to>>>>>
banner: https://img.osnsyc.top/XXXXXX.webp
```

```
{{< dbcard
    ...
    cover=[[Pasted image 2025.png]]
    ...
>}}
>>>>>Transfer to>>>>>
{{< dbcard
    ...
    cover="https://img.osnsyc.top/XXXXXX.webp"
    ...
>}}
```

```
![](video_filename | url)
[](video_filename | url)
![[video_filename | url]]
[[video_filename | url]]
>>>>>Transfer to>>>>>
{{< video src="https://img.osnsyc.top/XXXXXX.mp4" >}}
```

链接替换完成后生成一个新的 markdown 文件，可以由 hugo 正确地编译。生成的附件也可以用脚本一键上传至 Cloudfalre R2 存储桶。最终，一个完整的 Obsidian 至 Hugo 的工作流只需要两行命令即可完成。相关代码可以移步[GitHub - osnsyc/obsidian-to-hugo-toolbox](https://github.com/osnsyc/obsidian-to-hugo-toolbox)查看。

```
# 格式化 Markdown 文件
python md_publisher.py -f test_post.md
# 上传至 R2
python r2_uploader.py -f <path_to_file_or_folder>
```

![](https://cdnfile.sspai.com/2025/07/28/b74e46debd01f027605b1f3cff8df3f5.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

左: Obsidian，右:静态博客

我在去年建立博客之初[Hugo 博客快速搭建小记](https://osnsyc.top/posts/hugo-blog-building/)写道：

> 我写了 9 篇博文，平均篇幅 4570 字，附件不算少，R2 空间用了 160MB，算下来，免费空间够写 562 篇长文了。

现在看来，博客共有文章 24 篇，各类图像都有6，优化后的附件总大小为 113.9MB，所以现在算下来，CloudFlare R2 免费空间够写 2107 篇长文了。

 

数量

体积/MB

平均体积

静态图片

258

23.1

0.09MB

动态图片

29

87.9

3.03MB

视频

1

3.9

3.9MB

总和

288

113.9

0.40MB

**相关阅读**

-   [How to optimize images for website performance: best image sizes, compression, tools & testing](https://www.foregroundweb.com/image-size/)
-   [web.dev, Responsive Images](https://web.dev/articles/responsive-images?hl=zh-cn)
-   [Hugo 博客快速搭建小记](https://osnsyc.top/hugo-blog-building)

\> 关注 [少数派小红书](https://www.xiaohongshu.com/user/profile/63f5d65d000000001001d8d4)，感受精彩数字生活 🍃

\> 实用、好用的 [正版软件](https://sspai.com/mall)，少数派为你呈现 🚀
