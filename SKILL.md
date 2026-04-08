---
name: music-prompt-generator
description: 分析用户上传的音乐或音乐链接，自动生成AI音乐平台复刻提示词并提供曲名建议。生成4种提示词：中文基础版、英文基础版、中文进阶版、英文进阶版。适用于Mureka、Suno、Udio等平台。当用户要求分析音乐、生成复刻提示词、复刻这首歌、生成AI音乐提示词、给音乐起名字、推荐曲名时使用。
---

# 音乐复刻提示词生成器

## 功能概述

分析用户上传的音乐或音乐链接，自动生成AI音乐平台复刻提示词并提供曲名建议。适用于 Mureka、Suno、Udio 等平台。

## 支持的音乐源

### 1. 音乐链接分析
- 网易云音乐
- QQ音乐
- Spotify
- Apple Music
- 其他主流音乐平台

### 2. 本地音频文件
支持格式：mp3 / wav / aac / m4a / flac / ogg

## 音乐特征识别

### 风格流派
- 古风 / 流行 / 电子 / 摇滚 / 古典 / 民谣 / 爵士 / 嘻哈 / 乡村 / 金属 / 新世纪

### 情绪基调
| 能量等级 | 情绪关键词 |
|---------|-----------|
| 高能量 | 激昂、热血、战斗、爆发、欢快、兴奋 |
| 中能量 | 深情、温柔、浪漫、史诗、壮观 |
| 低能量 | 安静、平静、忧伤、孤独、空灵 |

### 速度 BPM
- 慢速：60-80 BPM
- 中速：80-110 BPM
- 快节奏：110-140 BPM
- 极速：140+ BPM

### 调式
- 大调 / 小调 / 五声音阶 / 七声音阶 / 特殊调式

### 乐器配置
支持识别主要乐器和次要乐器

## AI音乐平台提示词生成

### 中文基础模板

```
[风格描述]，情绪[情绪词]，[速度描述]
[主要乐器]、[次要乐器]
无歌词/纯器乐，[人声描述]
- [详细场景描述]
```

### 英文基础模板

```
[Genre] music, [mood], [tempo] BPM
[instruments], [texture]
[Instrumental/With vocals], [vocal style]
- [Scene description]
```

### 中文进阶版提示词（包含情绪时间线）

```
中文 [流派]

情绪时间线：[情绪1](0:00-X:XX) → [情绪2](X:XX-X:XX) → [情绪3](X:XX-end)

速度：[BPM范围] | 调性：[调式] | 拍号：[节拍]

【分段编排】
- 前奏：[描述]
- 主段：[描述]
- 高潮：[描述]
- 尾声：[描述]

【乐器配置】
- 主奏：[乐器]
- 伴奏：[乐器]
- 氛围：[元素]

【制作要求】
[制作风格描述]

- [详细描述]
```

### 英文进阶版提示词（Advanced with Emotional Timeline）

```
English [Genre]

Emotional Timeline: [Emotion 1](0:00-X:XX) → [Emotion 2](X:XX-X:XX) → [Emotion 3](X:XX-end)

Tempo: [BPM Range] | Key: [Mode] | Time Signature: [Time]

【Section Arrangement】
- Intro: [Description]
- Main: [Description]
- Climax: [Description]
- Outro: [Description]

【Instrumentation】
- Lead: [Instrument]
- Accompaniment: [Instruments]
- Atmosphere: [Elements]

【Production Requirements】
[Production Style Description]

- [Detailed Description]
```

## 曲名建议

根据音乐风格和情绪，提供 3-5 个曲名选项：

| 类别 | 曲名选项 |
|------|----------|
| 磅礴大气类 | 示例1、示例2 |
| 诗意优雅类 | 示例1、示例2 |
| 电影感类 | 示例1、示例2 |
| **最终推荐** | [推荐曲名] - [理由] |

## 输出格式

严格按照以下格式输出完整报告：

### 1. 音乐分析报告
- 音乐来源：[链接/文件名]
- 分析时间：[时间戳]

### 2. 音乐特征分析
| 特征 | 分析结果 |
|------|----------|
| 风格流派 | [识别结果] |
| 情绪基调 | [识别结果] |
| 速度 BPM | [识别结果] |
| 调式 | [识别结果] |
| 主要乐器 | [识别结果] |
| 次要乐器 | [识别结果] |

### 3. AI音乐平台提示词

#### 中文提示词
```
[生成的中文提示词]
```

#### 英文提示词
```
[生成的英文提示词]
```

#### 中文进阶版提示词
```
[生成的中文进阶版提示词]
```

#### 英文进阶版提示词
```
[生成的英文进阶版提示词]
```

### 4. 曲名建议
[曲名建议表格]

### 5. 使用说明
[如何在各平台使用这些提示词的说明]

## 乐器关键词对照表

### 中国传统乐器
| 乐器 | 英文 | 适用风格 |
|------|------|----------|
| 古筝 | Guzheng | 古风、传统、仙侠 |
| 笛子 | Bamboo Flute | 古风、传统、仙侠 |
| 二胡 | Erhu | 悲伤、怀旧、传统 |
| 琵琶 | Pipa | 古典、传统、战斗 |
| 中国鼓 | Chinese Drum | 节日、传统、战斗 |
| 编钟 | Bianzhong | 古典、宫廷 |
| 萧 | Xiao | 古风、忧伤、空灵 |
| 笙 | Sheng | 传统、节日 |
| 扬琴 | Yangqin | 古典、民乐合奏 |

### 西洋乐器
| 乐器 | 英文 | 适用风格 |
|------|------|----------|
| 钢琴 | Piano | 古典、流行、爵士 |
| 吉他 | Guitar | 流行、摇滚、民谣 |
| 小提琴 | Violin | 古典、电影配乐 |
| 大提琴 | Cello | 古典、忧伤、史诗 |
| 架子鼓 | Drum | 摇滚、电子、流行 |
| 贝斯 | Bass | 摇滚、电子、爵士 |
| 萨克斯 | Saxophone | 爵士、布鲁斯 |
| 小号 | Trumpet | 爵士、古典、庆典 |

## 使用示例

**用户输入**：
"分析这首音乐并生成复刻提示词：https://music.example.com/track/12345"

**Agent 输出**：
```
## 音乐分析报告
- 音乐来源：网易云音乐
- 曲名：示例音乐

## 音乐特征分析
| 特征 | 分析结果 |
|------|----------|
| 风格流派 | 古风、仙侠 |
| 情绪基调 | 空灵、忧伤 |
| 速度 BPM | 75 (慢速) |
| 调式 | 五声音阶 |
| 主要乐器 | 古筝、笛子 |
| 次要乐器 | 萧、编钟 |

## AI音乐平台提示词

### 中文提示词
古风仙侠风格，情绪空灵悠远，慢速悠扬
古筝、笛子为主，萧声点缀
纯器乐，无人声
- 仿佛置身云雾缭绕的山巅，月光洒落，古道西风

### 英文提示词
Chinese Ancient Fantasy, ethereal and melancholic, 75 BPM
Guzheng lead, Bamboo Flute, Xiao flute accents
Instrumental, no vocals
- Ethereal mountain top scene, moonlight, ancient path in wind

### 中文进阶版提示词
中文 古风仙侠

情绪时间线：空灵(0:00-0:30) → 忧伤(0:30-1:30) → 释然(1:30-end)

速度：70-80 BPM | 调性：E羽五声 | 拍号：4/4

【分段编排】
- 前奏：古筝独奏，悠远空灵
- 主段：笛子加入，旋律展开
- 高潮：萧声与编钟交织
- 尾声：渐弱回归宁静

【乐器配置】
- 主奏：古筝
- 伴奏：笛子、萧
- 氛围：编钟、流水声

【制作要求】
追求空灵感，使用混响营造空间感，注意气息控制的连贯性

### 英文进阶版提示词
English Chinese Ancient Fantasy

Emotional Timeline: Ethereal(0:00-0:30) → Melancholic(0:30-1:30) → Release(1:30-end)

Tempo: 70-80 BPM | Key: E Minor Pentatonic | Time Signature: 4/4

【Section Arrangement】
- Intro: Guzheng solo, distant and ethereal
- Main: Bamboo flute joins, melody unfolds
- Climax: Xiao flute and Bianzhong intertwine
- Outro: Fade into serenity

【Instrumentation】
- Lead: Guzheng
- Accompaniment: Bamboo Flute, Xiao
- Atmosphere: Bianzhong, flowing water sounds

【Production Requirements】
Pursue ethereal quality, use reverb for spatial depth, maintain breath control consistency

## 曲名建议

| 类别 | 曲名选项 |
|------|----------|
| 磅礴大气类 | 云山雾隐、月落乌啼 |
| 诗意优雅类 | 望月怀远、寒江独钓 |
| 电影感类 | 仙侠传·序章、古道西风 |
| **最终推荐** | 月落乌啼 - 契合音乐空灵忧伤的基调 |

## 使用说明

### Mureka 平台
[使用上述提示词的复制建议]

### Suno 平台
[使用上述提示词的复制建议]

### Udio 平台
[使用上述提示词的复制建议]
```
