# Melodies of Learning

## 项目简介

本项目利用以下技术实现创新的磨听力视频格式：
- **ChatTTS**: 进行语音合成
- **MSST**: 进行人声分离
- **Whisper**: 进行语音识别

我们将传统的磨听力视频格式（“三句英文 + 一句中文 + 一句英文”）进行了改造：
- **英文部分**: 替换为英文歌曲片段
- **中文部分**: 用歌词的直译进行替换，并让 AI 朗读

最终，使用 `ffmpeg` 将这些音频片段按照原视频的节奏依次剪辑在一起，完成了项目。

## 项目挑战与未来计划

在项目中，编写歌曲切分算法的部分耗时最长。由于实验性地采用工厂模式来编写代码，后期修改底层代码变得困难。尽管通过不断调整参数，使每个切割出的片段都非常适合，但我计划未来使用深度学习 AI 来训练一个更高效的切割算法，以进一步提升效果和效率。
