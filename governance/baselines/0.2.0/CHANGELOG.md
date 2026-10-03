# Changelog

## 0.2.0 — 2026-10-03

补上能出片的脚本规则。目标：用原有触发语，从一个场景或思路展开，或把一段小说改写成即梦向分镜脚本。

- 改了 `SKILL.md`、`skill.json`、`README.md` 的契约段。触发语七条不改。
- 新增 `references/01-intake.md`、`references/02-storyboard.md`、`references/03-characters.md`。
- 测了结构校验、打包试运行，以及答得对、正向改写、反向拒放宽、旧字段四条样稿。记录在 `governance/regression-reports/RR-20261003-001.md`。
- 回滚：用 `governance/baselines/0.1.0/` 覆盖同名分发包文件，删掉三份新细则和 `tests/cases-0.2.0.md`，并用 `git checkout ea3e3f4 -- tests/README.md` 恢复测试说明。不覆盖 0.1.0 基线。

## 0.1.0 — 2026-09-28

脚手架诞生（初始化）。本版无业务能力，只建立开发仓。

- 版本控制：根目录 `VERSION` + git
- 基线：`governance/baselines/0.1.0/`
- 升级记录：`CR-000-init`、`upgrade-to-0.1.0.md`
- 变更门禁与打包：见 `governance/`
