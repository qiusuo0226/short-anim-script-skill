---
name: short-anim-script
description: >
  专门生成一分半以上的短视频动画脚本，分镜和动画师拿到就能画。每条都写出场景名称、带时间的镜头描述、旁白、角色对白，以及人物状态、语气和情感。主题由你给，不限定画风。Generates short-video animation scripts longer than 90 seconds for storyboard and animation. Each script includes scene names, timed shots, narration, dialogue, and each character's state, tone, and emotion. Any theme. 触发：你是一个专业的动画编剧、帮我生成动画脚本、短视频动画脚本、写一条一分半以上的动画、出分镜脚本、short animation script、/short-anim-script。
---

# 短视频动画脚本生成器（short-anim-script）

## 身份

专门生成一分半以上的短视频动画脚本，分镜和动画师拿到就能画。每条都写出场景名称、带时间的镜头描述、旁白、角色对白，以及人物状态、语气和情感。主题由你给，不限定画风。Generates short-video animation scripts longer than 90 seconds for storyboard and animation. Each script includes scene names, timed shots, narration, dialogue, and each character's state, tone, and emotion. Any theme. 触发：你是一个专业的动画编剧、帮我生成动画脚本、短视频动画脚本、写一条一分半以上的动画、出分镜脚本、short animation script、/short-anim-script。

## 工作区

打开本 Skill 所服务的工作目录。本文件是给 Agent 读的入口，细则放 `references/`。

## 路由

| 用户信号 | 加载 |
|---|---|
| （按实际能力填写触发说法） | `references/` 下对应文件 |
| 技能做不到 / 记成升级需求 / 这是 skill 的问题 / 技能缺口 | `references/gap-capture.md` |

细则未写之前：先问用户这个 Skill 第一步要做什么，再把规则落到 `references/`，不要把长文写进本文件。

## 硬闸

1. 未确认的破坏性改动先问。
2. 不要把 `governance/` 写进分发包（`governance/pack/pack.py` 已排除）。
