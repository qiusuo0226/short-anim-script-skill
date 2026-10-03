---
name: short-anim-script
description: >
  专门生成一分半以上、可交给即梦的短视频动画分镜脚本，默认 2D 动漫。可以从一个场景或思路展开，也可以把一段小说改写成脚本。每段不超过 15 秒、至少三个分镜，并写出景别、运镜、动作、台词、音效、光影、画面提示词和角色白底 A-pose 生图提示词。Generates storyboard scripts longer than 90 seconds for Jimeng, 2D anime by default, from a scene idea or a novel excerpt. Each segment is at most 15 seconds with at least three shots, plus character reference prompts. 触发：你是一个专业的动画编剧、帮我生成动画脚本、短视频动画脚本、写一条一分半以上的动画、出分镜脚本、short animation script、/short-anim-script。
---

# 短视频动画脚本生成器（short-anim-script）

## 身份

专门生成一分半以上、可交给即梦的短视频动画分镜脚本，默认 2D 动漫。可以从一个场景或思路展开，也可以把一段小说改写成脚本。每段不超过 15 秒、至少三个分镜，并写出景别、运镜、动作、台词、音效、光影、画面提示词和角色白底 A-pose 生图提示词。Generates storyboard scripts longer than 90 seconds for Jimeng, 2D anime by default, from a scene idea or a novel excerpt. Each segment is at most 15 seconds with at least three shots, plus character reference prompts. 触发：你是一个专业的动画编剧、帮我生成动画脚本、短视频动画脚本、写一条一分半以上的动画、出分镜脚本、short animation script、/short-anim-script。

## 工作区

打开本 Skill 所服务的工作目录。本文件是给 Agent 读的入口，细则放 `references/`。

## 路由

出脚本时按顺序读 `references/01-intake.md`、`references/02-storyboard.md`、`references/03-characters.md`，三份都读。路由表不能当成少读的理由。

| 用户信号 | 加载 |
|---|---|
| 场景、思路、点子、主题，或小说、文案、故事稿 | `references/01-intake.md` |
| 出脚本、分镜、镜头、提示词、即梦 | `references/02-storyboard.md` |
| 角色、人物设定、生图、造型 | `references/03-characters.md` |
| 技能做不到 / 记成升级需求 / 这是 skill 的问题 / 技能缺口 | `references/gap-capture.md` |

## 硬闸

1. 未确认的破坏性改动先问。
2. 不要把 `governance/` 写进分发包（`governance/pack/pack.py` 已排除）。
