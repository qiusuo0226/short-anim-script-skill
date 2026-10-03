# tests/

本 Skill 的回归用例。发布前至少各 1 条：正向、反向、旧能力未破坏。

初始化时带一份 pack 冒烟脚本（`run_smoke.py`）、结构校验测试（`test_validate_skill.py`）和检查器变异自测（`test_checker_mutations.py`：每条 validate / audit / 打包排除规则一个单点变异，必须由那一条规则抓到；新增规则没配用例会失败）。用例用 Markdown 或脚本均可，发版时在 RR 里引用。目标仓 `audit_release.py` 若发现 `tests/run_smoke.py` 会跑它；发版前会先跑 `governance/scripts/validate_skill.py`。

## 固定四问

每版 RR 都答这四问，输入不换，结果对照上一版 RR。改输入先在 AP-5 写理由。初始化后第一次升级时把「固定输入」填实。

| 问题 | 固定输入 |
|---|---|
| 装得上 | `python governance/pack/pack.py --skill-root . --dry-run`：文件数；无 `governance/`、`.git/`、`AGENTS.md` |
| 唤得起 | 新对话第一句：`帮我生成动画脚本` |
| 答得对 | `帮我生成动画脚本。思路：一只猫在雨夜门口等主人。` 期望：全片不少于 90 秒；每段不超过 15 秒且至少三镜；每镜有场景名称、时间、景别、运镜、动作、人物状态、语气、情感、台词、旁白、音效、光影、场景、画面提示词（主体 + 行为 + 环境，以及风格、色彩、光影、构图）、图生视频的动作和镜头运动；除第一镜外每镜写了衔接元素；开篇有统一的 2D 动漫风格和色调；每个出镜角色有白底、无纹理、无渐变、A-pose 的生图提示词，并含性别、年龄、风格、头部、手部、穿搭、配饰 |
| 说得清 | `python governance/scripts/validate_skill.py --skill-root .` 全 PASS；README 开口说法与 `SKILL.md` 触发段一致 |

正向、反向、旧能力三条见 `tests/cases-0.2.0.md`。
