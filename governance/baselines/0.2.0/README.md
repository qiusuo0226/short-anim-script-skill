# 短视频动画脚本生成器（short-anim-script）

专门生成一分半以上、可交给即梦的短视频动画分镜脚本，默认 2D 动漫。可以从一个场景或思路展开，也可以把一段小说改写成脚本。每段不超过 15 秒、至少三个分镜，并写出景别、运镜、动作、台词、音效、光影、画面提示词和角色白底 A-pose 生图提示词。Generates storyboard scripts longer than 90 seconds for Jimeng, 2D anime by default, from a scene idea or a novel excerpt. Each segment is at most 15 seconds with at least three shots, plus character reference prompts. 触发：你是一个专业的动画编剧、帮我生成动画脚本、短视频动画脚本、写一条一分半以上的动画、出分镜脚本、short animation script、/short-anim-script。

## 开发

本目录是 Skill **开发仓**。版本控制、基线、升级记录和打包都在 `governance/`（不进分发包）。改本 Skill 时让助手读 `governance/rules/skill-governance.md`，不必再调用 skill-devkit。

```
powershell -File governance/dev.ps1 pack
powershell -File governance/dev.ps1 release
```

## 许可证

[MIT](LICENSE) © 2026 qiusuo0226
