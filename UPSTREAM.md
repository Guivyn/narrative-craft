# UPSTREAM — 上游来源与本地定制说明

本技能是**本地定制合并版**，不是任何上游仓库的原文。`npx skills add` 等工具更新上游时**不会**自动更新本目录，也不会在本目录被重建时保留改动。

## 合并来源

| 来源 | Skill | 版本 / 位置 | 保留方式 |
|------|-------|------------|---------|
| renky1025/agent-skills | `snowflake-novel-writer` | SKILL.md + references（雪花法十步、去 AI 味、反俗套、对白、开头、题材、大纲、质检） | 主干流程与中文语气；references 多数原样迁入 |
| alt-code-ai/agent | `fiction-writing-story-development` | 单文件英文理论（McKee/Egri/Truby/Schechter/Snyder/Vogler/Charters） | 中文提炼为 `references/methodology-overview.md`；原目录已删除 |

## 迁入映射

| 本技能文件 | 来源 |
|-----------|------|
| `references/outline-methods.md` | snowflake（原样） |
| `references/genre-writing.md` | snowflake + 新增「题材→框架→俗套」映射表 |
| `references/anti-cliche.md` | snowflake SKILL.md 的反俗套/反转/钩子/情感弧线 + 与诊断表分工 |
| `references/voice-and-prose.md` | snowflake SKILL.md 第9步 + 散文技法 |
| `references/dialogue-mastery.md` | snowflake（原样） |
| `references/opening-design.md` | snowflake（原样） |
| `references/de-ai-writing.md` | snowflake（原为 `de-ai-writing` 本地副本，现为本技能权威版） |
| `references/banned-words.md` | snowflake（原样） |
| `references/quality-checklists.md` | snowflake（原样） |
| `references/methodology-overview.md` | fiction-writing-story-development 的中文提炼（其完整快照另存于 `C:\Program Files (x86)\Steam\steamapps\common\#Document\叙事开发方法论-精炼.md`） |
| `references/character-workshop.md` | snowflake 第4/5步 + fiction 人物架构 |
| `references/glossary.md` | 新增（中英术语对照） |

## 权威版本约定（避免双源）

- 本目录 `references/` 是**唯一权威源**。
- `#Document` 下的《叙事开发方法论-精炼.md》是最初生成的外部**快照**，可作阅读资料；如与本目录冲突，以本目录为准。

## 已知偏离上游

1. 删除了原 snowflake SKILL.md 中指向 `novel-writing`、`de-ai-writing` 的死链，改为与 `story-long-write` 的分工。
2. 十步流程重组为 0–10 步，区分【必做】与【扩展】，每步加最小交付物。
3. 新增问题清单分级、reference 加载表、降级做法。
4. `methodology-overview.md` 替代了原 fiction 英文单文件。

## 维护建议

- 若需跟踪上游更新：用 git subtree/submodule 保留 `renky1025/agent-skills` 与 `alt-code-ai/agent` 副本，人工比对后再合入。
- 修改本目录后，如需同步给 `npx skills` 体系，请确认 `.agents/.skill-lock.json` 中不含本技能的旧条目。
