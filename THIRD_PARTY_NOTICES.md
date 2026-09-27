# YiCue 第三方声明

**状态：已确认来源的通知与发行清单草案 · 2026-09-28**

YiCue 使用或沿用第三方代码、运行时、库和模型。这些内容继续适用各自的许可，产品 EULA 不限制其独立许可授予的权利。本文件记录已确认的来源；完整发行材料应按实际安装包版本补齐。

## LiveTranslate 继承代码

上游：[TheDeathDragon/LiveTranslate](https://github.com/TheDeathDragon/LiveTranslate)，参考版本：[v2026.08.17.1](https://github.com/TheDeathDragon/LiveTranslate/tree/v2026.08.17.1)。YiCue 的部分音频、ASR、VAD、翻译及相关基础模块沿用或改编自该项目；其原版权和许可通知如下。

```text
MIT License

Copyright (c) 2025 Shiro

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 已确认的组件与许可

| 组件 | 已确认许可或来源 | 发行材料要求 |
| --- | --- | --- |
| FunASR 软件包 | MIT，实际版本以发行包为准 | 保留该版本完整版权和许可 |
| 内置 FunASR Nano 代码 | 来自 LiveTranslate；同时对应 QwenAudio/Fun-ASR 的 Apache-2.0 历史实现 | 保留适用 Apache 许可、署名、NOTICE 和修改说明，核准准确来源版本 |
| transcribe-cpp 0.2.2 / native bundle | MIT；native bundle 另含 ggml、miniz 通知 | 保留运行时中全部 licenses 文件 |
| Koffi 3.1.4 | MIT，含额外 vendor 通知 | 保留完整 LICENSE 及附属通知 |
| Node.js | 运行时包含 Node 和内置依赖的多种许可 | 附与实际 node.exe 版本对应的完整集成 LICENSE |
| PySide6 / Shiboken / Qt | 提供 LGPL/GPL 或商业许可路径 | 按采用的许可满足通知、文本、对应源码及替换／重新链接等要求 |
| PyAudioWPatch | Apache-2.0，含底层音频组件 | 保留对应版本许可和音频库通知 |
| soundfile / libsndfile | Python 包与原生库分别许可；当前原生库包含 LGPL-2.1 条款 | 保留各自版权、许可及适用的原生库材料 |
| PyInstaller | GPL 及程序分发例外 | 按其分发例外和对应发行材料处理 |

本表不是安装包完整的软件物料清单。Python、Torch、NumPy、FFmpeg 等运行时和原生依赖也需按实际分发版本保留适用的第三方材料。

## 模型

Qwen3-ASR GGUF、SenseVoice Small 和 Whisper 模型在应用中单独下载。代码许可、原模型权重许可、量化文件发布条件分别适用；用户应查阅模型权利人和下载仓库的条款。

## 来源与条款

- [LiveTranslate 原许可](https://github.com/TheDeathDragon/LiveTranslate/blob/v2026.08.17.1/LICENSE)
- [FunASR 官方许可](https://github.com/modelscope/FunASR/blob/main/LICENSE)
- [Fun-ASR 历史实现](https://github.com/QwenAudio/Fun-ASR/tree/d9ba359ddf9eeaaa7ad4db8ae209abfe0596cee8)及[历史许可](https://github.com/QwenAudio/Fun-ASR/blob/d9ba359ddf9eeaaa7ad4db8ae209abfe0596cee8/LICENSE)
- [transcribe.cpp 0.2.2 许可](https://github.com/handy-computer/transcribe.cpp/blob/v0.2.2/LICENSE)
- [Qt LGPL 义务说明](https://www.qt.io/development/open-source-lgpl-obligations)
- [PyInstaller 许可与例外](https://pyinstaller.org/en/stable/license.html)
- [FFmpeg 许可说明](https://ffmpeg.org/legal.html)

对应发行包应附完整许可文本及依法需要提供的源码、获取方式或其他材料；本草案不能代替这些材料。
