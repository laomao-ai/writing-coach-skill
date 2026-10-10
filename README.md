# 写作教练 writing-coach

**把全球顶尖的写作大师，请进你的 AI。**

选题、标题、框架、成稿、打磨，每一步都有大师的方法；五道关打分，告诉你哪里还能更好。

14 位写作大师（叶圣陶、鲁迅、汪曾祺、奥威尔、津瑟、斯蒂芬·金……）、9 套方法（金字塔原理、SCQA、哈佛论证写作……）、6 种练法，先认文体再请人：科技稿请平克和津瑟，随笔请汪曾祺和朱光潜。可以从一个想法一路写到成稿，也可以只用其中一步，或者接进你自己的 Agent 和写作流程。

**展示页**：https://laomao-ai.github.io/writing-coach-skill/ ｜ **大师展厅**：https://laomao-ai.github.io/writing-coach-skill/masters.html

![大师团](docs/img/wall.svg)

## 五步，从哪一步进来都行
| 你说 | 它做 |
|---|---|
| “我想写写 AI 工具，帮我想个选题” | **① 选题立意**：3 个角度、各附一句话立意和目标读者，推荐一个；想更透可以让对口大师追问 |
| “起几个标题，搭个框架” | **② 标题框架**：3–5 个风格不同的标题 + 提纲（每段要点和需要的材料） |
| “写一篇” / “把这些卡片写成文章” | **③ 成稿**：从题目、观点、卡片、半成品、提纲任一起点写成全文，附待核实清单和五关自评 |
| “帮我体检 / 打个分 / 请大师看看” | **④ 体检**：五关各 0–4 分，每个问题带原文定位和改法；可请大师会诊、只核事实，或输出评分块给别的 Agent 读 |
| “润色 / 改得更像我 / 按奥威尔删一遍” | **⑤ 打磨**：轻 / 中 / 重三档，保留原风格或按指定大师、文体、平台改，附改动清单 |

## 五关
立意 → 结构 → 证据 → 语言 → 读者，每关 0–4 分，满分 20，每一分都要引原文作依据。评分锚点见 [gates/](gates/README.md)。

## 有什么不一样
- **方法来自大师**：每张大师卡写明出处、核心主张、用在哪一步、局限和核对状态；请的是方法，不模仿口吻。
- **先认文体再请人**：10 类文体各配最多 3 位对口大师，余光中做全局语言检查。
- **能量化**：五关打分可复现，改前改后能对比。
- **能集成**：每一步可单独调用；体检能输出 JSON 评分块，方便接进别的 Agent 当质检层。
- **守“写得好”**：不追热点、不做 SEO、不教标题党，这些交给运营类工具。

## 安装
```bash
# Claude Code
git clone https://github.com/laomao-ai/writing-coach-skill ~/.claude/skills/writing-coach
```
Codex、OpenClaw 等支持 Agent Skills 的工具：把仓库放进对应的 skills 目录，入口是 SKILL.md。

写完交给同系列的 [wechat-gzh-publish](https://github.com/laomao-ai/wechat-gzh-publish) 排版发布。

## 目录
```
SKILL.md        入口：从哪一步进、质量标准、输出约定
stages/         五步：topic 选题立意 / outline 标题框架 / draft 成稿 / review 体检 / polish 打磨
gates/          五关与评分锚点
masters/        14 张大师卡 + 入选标准 + 文体路由表
methods/        9 套方法：金字塔、SCQA、哈佛论证、倒金字塔、SUCCESs、费曼、冰山、威廉姆斯、卡片笔记
drills/         练法：富兰克林重写、仿写、自由写作、烂初稿、刻意练习、日更
style/          风格档案（可选）
checklists/     逻辑、事实、AI 腔、错别字
scenes/         平台场景卡：公众号
templates/      体检报告、会诊报告
references/     素材检索
evals/          用例、稿件、结果
docs/           展示页与大师展厅
```

## 致谢
方法来自《叶圣陶谈写作》《文心雕龙》《写作法宝》《风格感觉》《金字塔原理》等，书目见 books/SOURCES.md，全部为自述转述。开源项目只借思路、不搬原文（均为 MIT）：[Humanizer-zh](https://github.com/op7418/Humanizer-zh)、[lieflat-less-ai-tone](https://github.com/larashero3-dotcom/lieflat-less-ai-tone)、[writing-agent](https://github.com/dongbeixiaohuo/writing-agent)、[writing-dna-skill](https://github.com/larashero3-dotcom/writing-dna-skill)、[shuorenhua](https://github.com/MrGeDiao/shuorenhua)。

大师插画为示意创作，不是照片。

## 版本
- v4：定位改为“把全球顶尖的写作大师，请进你的 AI”；五步全流程（选题、框架、成稿、体检、打磨），任一步可单独用；新增风格档案、评分块；评测精简为 8 条；展示页加大师插画。
- v3：14 位大师按文体路由、9 套方法、6 种练法、大师展厅。
- v2：五关评分、大师会诊、评测、展示页。
- v1.2：首个公开版本。

License: MIT
