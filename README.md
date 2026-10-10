# 写作教练 writing-coach

中文自媒体人的写作教练 + 写作体检。**不替你写，只让你写得更好。**

请 14 位写作大师、9 套方法给你的稿子会诊，用五道关体检：立意 → 结构 → 证据 → 语言 → 读者。先认文体再请人，科技稿不会被拿去问汪曾祺。只提问、只挑错，改不改由你。

**展示页**：https://laomao-ai.github.io/writing-coach-skill/ （四种用法、体检报告、润色对比）；**大师展厅**：https://laomao-ai.github.io/writing-coach-skill/masters.html

## 四种用法
| 你说 | 它做 |
|---|---|
| “我想写 X，没思路” | **引导写**：先“写前拷问”，由对口大师轮流追问，产出立意卡和骨架，正文你写 |
| “帮我体检这篇” | **体检**：先认文体，五关各 0–4 分，P0/P1/P2 问题都带原文定位，最后推荐一个练法；不改正文。只想查数字和引语时走“只核事实” |
| “请奥威尔和金看看” | **大师会诊**：每位大师从自己的视角挑最多 3 条问题，各附一个追问，最后开 3 条处方 |
| “润色，保留我的风格” | **润色**：最小改动，附改动清单（原句→新句→原因）和没改的地方 |

## 和同类项目有什么不同
多数中文写作 skill 做的是“去 AI 味改写”：把稿子改一遍交给你。这个项目做的是另一件事：

- **只教不代写**：不出全文，不出能直接发的段落；示范段 ≤150 字并标“请勿直接使用”。
- **先认文体再请人**：公众号常见的 9 类文体各配最多 3 位对口大师，余光中做全局语言检查。
- **方法可溯源**：每张大师卡写明出处、核心主张、局限和核对状态，没核对的标“待核”，不编页码、不造名言。
- **打分可复现**：五关每一分都要引原文作依据；同一篇改前改后都能打分对比。
- **自带对抗评测**：13 条用例，诱导编造、改立场、洗稿、冒用大师口吻、一键成文；原始回复全部公开在 evals/runs/。

## 铁律
不编造事实、数据、引文；不改立场和确定程度（“可能”不改成“一定”，也不改成“大概率”）；缺证据标“待补”并给检索建议；没联网时不写“已核实”。不做一键成文、洗稿、热点爬取、排版发布。

## 安装
```bash
# Claude Code
git clone https://github.com/laomao-ai/writing-coach-skill ~/.claude/skills/writing-coach
```
其他支持 Agent Skills 的工具：把仓库放进对应的 skills 目录即可，入口是 SKILL.md。

## 目录
```
SKILL.md        入口：判断用法、铁律、输出约定
gates/          五关与评分锚点
masters/        14 张大师卡 + 入选标准 + 文体路由表
modes/          引导写 / 体检 / 大师会诊 / 润色
methods/        9 套方法：金字塔、SCQA、哈佛论证、倒金字塔、SUCCESs、费曼、冰山、威廉姆斯、卡片笔记
drills/         练法：富兰克林重写、仿写、自由写作、烂初稿、刻意练习、日更
checklists/     逻辑、事实、AI 味、错别字
scenes/         平台场景卡：公众号
templates/      体检报告、会诊报告
references/     素材佐证检索
evals/          用例、稿件、结果、原始回复
docs/           展示页
```

## 致谢
方法来自《叶圣陶谈写作》《文心雕龙》《写作法宝》《风格感觉》《金字塔原理》等，书目见 books/SOURCES.md，全部为自述转述。开源项目只借思路、不搬原文（均为 MIT）：[Humanizer-zh](https://github.com/op7418/Humanizer-zh)、[lieflat-less-ai-tone](https://github.com/larashero3-dotcom/lieflat-less-ai-tone)、[writing-agent](https://github.com/dongbeixiaohuo/writing-agent)、[writing-dna-skill](https://github.com/larashero3-dotcom/writing-dna-skill)、[shuorenhua](https://github.com/MrGeDiao/shuorenhua)。

同系列：[wechat-gzh-publish](https://github.com/laomao-ai/wechat-gzh-publish)（公众号排版发布）。写完、体检完，交给它排版。

License: MIT
