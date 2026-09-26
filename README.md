# narrative-craft · 叙事工坊

中文小说叙事开发 skill：**雪花法搭骨架，剧作理论做诊断，去 AI 味收尾**。

从一句话逐层展开成可写的结构，判断结构是否成立、哪里失效，再让文字和故事都更耐读。

## 触发

写小说、故事结构、人物弧光、场景规划、反套路、去AI味、叙事开发。

管单部作品的构思、结构诊断与定稿。长篇连载的项目管理（日更、追踪、分卷细纲、拆文导入）交给 `story-long-write`，两者可接力：本技能定前提/结构/人物/声音，它负责跨章节执行。

## 五个入口

先看你手里已经有什么：

| 你现在的状态 | 从哪里进 |
|---|---|
| 只有一个想法 | 第 0/1 步，从零顺序推进 |
| 有片段或设定 | 从片段反推第 1/3/4 步，再进第 7、9 步 |
| 有现成大纲 | 补强第 4/8/9 步 |
| 只想要成品 | 极简补齐第 0–3 步关键判断，先给样章，再决定是否扩写 |
| 有完整草稿要修结构 | 直接进第 10 步结构诊断 |

## 工作流

0–10 步，每步标**必做**或扩展，并且只交付一个**最小交付物**——一句话前提、五段大纲、场景表、样章任务。不会一上来问一堆问卷。

修订两遍，先结构后语言；发现的问题按 **阻断级 → 结构级 → 语言级 → 风格级** 的顺序修。

## 按需加载

主文件只放流程，理论沉淀在 `references/`，由「症状 → 文件」表定位：

```text
references/
├── methodology-overview.md   剧作理论总纲：前提 / 结构 / 人物 / 场景 / 压缩 / 诊断
├── character-workshop.md     人物卡、关系网、对手与反派层级
├── anti-cliche.md            反俗套、反转工具箱、钩子、情感弧线
├── voice-and-prose.md        叙述声音、文风模块表
├── genre-writing.md          题材 → 推荐框架 → 常见俗套
├── outline-methods.md        大纲方法、升级感、黄金前三章
├── dialogue-mastery.md       对白
├── opening-design.md         开头
├── de-ai-writing.md          去 AI 味三遍法
├── banned-words.md           禁用词 / 禁用模式
├── quality-checklists.md     成稿质检
└── glossary.md               中英术语对照
```

## 安装

```bash
git clone https://github.com/Guivyn/narrative-craft.git ~/.agents/skills/narrative-craft
```

## 来源与维护

雪花法、去 AI 味、反俗套来自 `snowflake-novel-writer`（renky1025/agent-skills）；结构理论来自 `fiction-writing-story-development`（alt-code-ai/agent），已提炼成 `references/methodology-overview.md`。本仓库是本地定制的合并版，与上游没有原文继承关系——迁入映射与已知偏离见 `UPSTREAM.md`。

`evals/evals.json` 提供 10 个评测 case，覆盖从零构思、结构修补、人物与语言等路径。
