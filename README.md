# narrative-craft · 叙事工坊

中文小说叙事开发助手 skill。用**雪花写作法**从一句话逐层展开结构，用**西方剧作理论**判断故事是否成立，再用**去 AI 味与反俗套**检查让文字更耐读。

> 适用于：从零构思、已有片段反推结构、大纲补强、结构诊断与修订、样章与定稿。
> 不负责：长篇项目管理、日更、拆文、导入（那属于 `story-long-write` 等长篇工具箱）。

## 特性

- **双引擎**：中文流程（雪花法十步）+ 结构诊断层（McKee / Egri / Truby / Schechter / Snyder / Vogler）。
- **五个入口**：从零 / 从片段 / 从大纲 / 直接要成品 / 从完整草稿修结构。
- **必做-扩展分级**：0–10 步，每步带最小交付物，避免一次性问一堆问卷。
- **按需加载**：主文件只放流程；理论沉淀在 references，按「症状 → 文件」表加载。
- **分级问题清单**：阻断级 / 结构级 / 语言级 / 风格级，先结构后语言修复。
- **内置评测**：`evals/evals.json` 共 10 个 case。

## 结构

```
narrative-craft/
├── SKILL.md                      主流程与路由
├── UPSTREAM.md                   上游来源与本地定制说明
├── evals/evals.json              评测用例
└── references/
    ├── methodology-overview.md   fiction 理论总纲（前提/结构/人物/场景/压缩/诊断）
    ├── character-workshop.md     轻量/深度人物卡、关系网、对手
    ├── anti-cliche.md            反俗套 + 反转 + 钩子 + 情感弧线
    ├── voice-and-prose.md        叙述声音 + 文风模块表
    ├── genre-writing.md          题材公式 + 题材→框架→俗套映射
    ├── outline-methods.md        大纲方法
    ├── dialogue-mastery.md       对白
    ├── opening-design.md         开头
    ├── de-ai-writing.md          去 AI 味三遍法
    ├── banned-words.md           禁用词 / 禁用模式
    ├── quality-checklists.md     成稿质检
    └── glossary.md               中英术语对照
```

## 安装

本 skill 采用 Agent Skills 目录约定（`SKILL.md` + `references/`）。

```bash
# 放入你的 agent skills 目录，例如：
git clone https://github.com/Guivyn/narrative-craft.git ~/.agents/skills/narrative-craft
```

## 来源

合并自两个 skill 的思想：

- `snowflake-novel-writer`（renky1025/agent-skills）—— 雪花写作法流程、去 AI 味、反俗套、对白/开头/题材。
- `fiction-writing-story-development`（alt-code-ai/agent）—— 西方剧作理论，中文提炼为 `references/methodology-overview.md`。

详见 `UPSTREAM.md`。本仓库是**本地定制合并版**，非任何上游的原文。
