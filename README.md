# 🎵 音乐复刻提示词生成器

> 分析音乐特征，自动生成适用于 Mureka / Suno / Udio 等 AI 音乐平台的高质量复刻提示词，并提供曲名建议。

## 功能亮点

- 🎼 **多平台音乐链接支持**：网易云、QQ音乐、Spotify、Apple Music 等
- 📁 **本地音频文件支持**：mp3、wav、flac、m4a 等常见格式
- 🔍 **全面特征识别**：风格流派、情绪基调、BPM、调式、乐器成分
- 📝 **三版提示词输出**：中文基础版 / 英文版 / 进阶版（含情绪时间线）
- 🏷️ **曲名建议**：5个维度推荐 + 最终精选

## 触发词

> 分析音乐、生成复刻提示词、复刻这首歌、生成AI音乐提示词、给音乐起名字、推荐曲名

## 适用平台

| 平台 | 说明 |
|------|------|
| [Mureka](https://mureka.ai) | 专业音乐创作平台 |
| [Suno](https://suno.com) | AI音乐生成先驱 |
| [Udio](https://udio.com) | 创新音乐生成工具 |

## 安装方法

将 `SKILL.md` 文件放入你的 agent 的 skills 目录即可：

```bash
# WorkBuddy
cp SKILL.md ~/.workbuddy/skills/music-prompt-generator/

# OpenClaw
cp SKILL.md ~/.openclaw/workspace/skills/music-prompt-generator/
```

## 使用示例

**输入：**
> 帮我分析这首歌并生成复刻提示词：https://music.163.com/song?id=xxx

**输出：**
- 音乐特征分析报告（风格、情绪、BPM、调式、乐器）
- 中文/英文/进阶版 AI 音乐提示词
- 5个方向的曲名建议

---

Made with ❤️ by 阿黄
