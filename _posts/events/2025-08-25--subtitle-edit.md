> id: https://sspai.com/post/101614

> link: https://sspai.com/post/101614

> title: Subtitle Edit

# Subtitle Edit
_Published on Mon, 25 Aug 2025 03:00:00 GMT_

![Article Cover Image](https://cdnfile.sspai.com/25/08/2025/article/0ca91b34-42a0-f6bd-ad0f-5250e6f5e45a.jpeg)  

**Matrix 首页推荐** 

[Matrix](https://sspai.com/matrix) 是少数派的写作社区，我们主张分享真实的产品体验，有实用价值的经验与思考。我们会不定期挑选 Matrix 最优质的文章，展示来自用户的最真实的体验和观点。   
文章代表作者个人观点，少数派仅对标题和排版略作修改。

* * *

缘起
--

今天在听中岛美雪的演唱会时，发现视频里内置了字幕。相比我之前用 Whisper 转写出来的版本，原生字幕肯定要准确得多。于是我开始找工具，希望能把这些内嵌字幕提取出来。试了好几款之后，最终脱颖而出的是 —— Subtitle Edit。

功能概述
----

[Subtitle Edit](https://www.nikse.dk/) 是一款功能强大的开源字幕编辑器，适用于字幕的提取、编辑、格式转换与翻译等多种场景。它支持多种视频与字幕格式，并内置 OCR 字符识别、语音转写、时间轴同步等实用功能。

最新版可在 [GitHub 发布页](https://github.com/SubtitleEdit/subtitleedit/releases)获取，或通过[国内镜像](https://wwva.lanzouq.com/i1mrz32pycbi)下载。支持 Windows，部分 Linux 系统可通过 Mono 兼容运行。

字幕提取
----

### 打开视频文件

启动软件后，点击菜单栏的「文件」（File） -> 「打开」（Open），选择你想提取字幕的视频文件。

### 选择字幕轨道

如果视频中包含多个字幕轨道，Subtitle Edit 会弹出窗口供你选择需要提取的那一条。

### （可选）进行 OCR 识别（适用于图像字幕）

若视频字幕为图像格式（如 DVD 的 VobSub 或蓝光的 PGS 字幕），软件会提示你进行「光学字符识别」（OCR）。此时建议选择 Paddle OCR 引擎，并根据字幕语言进行设置。点击「开始 OCR」后进行识别，完成后点击右侧的「确定」按钮。

**小提示：**对于中文、日文等非拉丁字符，Paddle OCR 的识别效果明显优于 Tesseract 等传统引擎；后者更适用于英文字幕。

![](https://cdnfile.sspai.com/2025/08/05/article/9a6bd91dd2525900bb972aba0506beb1.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1/format/webp)

### 保存为所需格式

字幕提取后，你可以在主界面中查看字幕文本与对应的时间轴。点击「文件」（File） -> 「另存为」（Save as），在保存类型中选择所需格式。

其它功能
----

除了基础的字幕提取功能，Subtitle Edit 还提供了丰富的扩展能力，适用于更复杂的字幕编辑与翻译需求。

### 语音转写

当视频中没有字幕轨道时，可以通过「工具」（Tools） -> 「语音识别」（Audio to text）自动生成字幕。Subtitle Edit 支持多种识别引擎：

-   **Whisper**（推荐，效果最优，支持多语言识别）
-   **Vosk**（轻量级本地模型，适合资源受限环境）

用户可选择语言或启用自动识别，支持断点恢复、每句字幕自动分段等配置。

### 字幕翻译功能

在已有字幕的基础上，Subtitle Edit 支持一键翻译所有字幕内容，可通过「翻译」菜单调用主流翻译引擎，如：Google Translate、DeepL、Yandex 等。你还可以选择手动逐句翻译，适合需要逐句优化语序的场景。

> 如果你需要批量的字幕翻译体验或使用ai翻译字幕，可以使用我开源的 [Subtitle Translator 工具](https://tools.newzone.top/zh/subtitle-translator)。  
> 该工具支持批量上传字幕，调用多个翻译 API，并可选择中英对照、断句模式、自定义输出格式等，适合字幕组、译者和内容创作者使用。

### 字幕同步与修正

Subtitle Edit 提供多种对齐和修正工具，帮助字幕更精确地贴合音视频内容：

-   自动根据音频波形对齐字幕时间
-   快速统一字幕偏移（正向或负向延迟）
-   修改帧率（用于从不同源转换视频）
-   检测并修复字幕重叠、间隔过短、过长等问题

### 字幕格式批处理

-   支持常见字幕格式互转：如 `.srt`、`.ass`、`.sub`、`.vtt` 等
-   支持 UTF-8、ANSI、Unicode 等多种编码转换
-   提供批量文本替换、去空字幕行、规范化字幕格式等自动化操作

### 精修同步字幕

可切换为「波形图」或「频谱图」视图，辅助进行精确的起止时间调整。非常适合精修口型同步字幕或歌词字幕。

常见误区说明
------

-   **MKVToolNix 并不能直接导出文本字幕**：尽管有些 AI 推荐该工具提取 MKV 字幕，但实际上它输出的是 `.mks` 格式（容器文件），而非可读的字幕文本。
-   **HandBrake 不支持字幕提取**：该工具适用于视频转码与压制，但无法直接提取字幕。

\> 关注 [少数派小红书](https://www.xiaohongshu.com/user/profile/63f5d65d000000001001d8d4)，感受精彩数字生活 🍃

\> 实用、好用的 [正版软件](https://sspai.com/mall)，少数派为你呈现 🚀
