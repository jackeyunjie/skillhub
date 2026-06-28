---
name: s-private-board-grouping
description: Use when structuring S级私董会/S级私董会3.1 grouping rules, NPC role design, 案主准备度, S1/S2/S3/S4 selection logic, behavior-weight governance, 小组角色分工, or converting private-board meeting/wiki materials into Obsidian-ready structured notes. Trigger on 私董会分组、NPC、S1/S2/S3/S4、高强组、全案组、战略组、案主、笔记官、主持人、行为权重、结营评估、or 分组作业落地.
---

# S Private Board Grouping

Use this skill to structure S-level private board materials into reusable grouping, role, and governance logic. Keep the output about the system itself, not personal coaching, unless the user explicitly asks for a recommendation.

## Core Principle

```
不是越高越好，而是越匹配越有效。
```

S-level private board grouping matches problem type, business stage, participation intensity, and role readiness. Do not treat S1-S4 as status levels.

## Grouping Map

| Group | Positioning | Use when | Key requirement |
|---|---|---|---|
| S1 路演私董会 | 讲清业务，问清业务 | The business cannot be explained clearly in a structured way | Train commercial expression and structured questioning |
| S2 问题私董会 | 梳理真问题，出口式咨询 | There is a real pain point, but the true problem is unclear | Clarify facts, split issues, identify hypotheses |
| S2 高强组 | 高投入、高追问、高复盘 | The user wants stricter challenge and can carry more work | Accept homework, direct feedback, strict review, 360 evaluation |
| S3 全案私董会 | 单案主 ABCD 假设全案梳理 | A complex business needs full-system decomposition | Case owner readiness and willingness to open real information |
| S4 战略私董会 | 亿级一号位战略决策 | The participant is a revenue-100M+ company first chair facing strategic decisions | Requires real operating stage, not prestige |

## Governance Logic

Structure the system as:

```
真实问题 → 标准流程 → NPC控场 → 角色协作 → 行为记录 → 结营反馈 → 下期分组优化
```

Important claims:

- Official grouping, not free grouping.
- Standard process, not casual discussion.
- NPC facilitation, not uncontrolled discussion.
- Real problems, not generic networking.
- Serious participation, not consumer experience.
- Graduation review, not meetings that disappear after they end.

## Role Table

| Role | Core work |
|---|---|
| NPC / 半官方身份 | Lead, advocate scientific business methods, organize ice-breaking, connect roles, provide fallback |
| 案主 / 幕僚董事 | Bring real cases, open facts, receive challenge, contribute as peer director |
| 知识管理官 / 笔记官 CIO | Use AI to evaluate, extract, model, record key questions and meeting outputs |
| 主持人 / 私董官 COO | Control time, topic direction, emotional rhythm, and meeting process |
| CEO / 项目经理 PM | Manage schedule, progress, and follow-up actions |
| Optional roles | 飞行嘉宾, 飞书官, CPO, CMO, CFO, or other role needed by the group |

## Structuring A Landing Note

When converting a wiki, meeting, or投屏文档 into Obsidian:

1. Capture source URL and local source file.
2. State completeness and whether direct fetch, screenshot, or local text was used.
3. Convert important image-only concepts into tables.
4. Separate grouping rules, role mechanics, behavior-weight rules, and evaluation rules.
5. Add direct Obsidian links to related notes.
6. Avoid personal recommendation language unless the user asks for selection advice.

## Output Template

```markdown
## 文档定位
- 来源：
- 整理目标：
- 完整性说明：

## 核心总纲
- 

## 重要图片结构转译
| 图片/结构 | 结构化转译 | 用途 |
|---|---|---|
|  |  |  |

## 分组机制
| 组别 | 定位 | 适合对象 | 不适合 |
|---|---|---|---|
| S1 |  |  |  |
| S2 |  |  |  |
| S3 |  |  |  |
| S4 |  |  |  |

## 角色机制
| 角色 | 职责 | 输出物 |
|---|---|---|
| NPC |  |  |

## 行为权重与结营
- 

## 关联链接
- [[]]
```

## Guardrails

- Do not rank groups as better or worse.
- Do not recommend S4 unless the material states a real revenue-100M+ first-chair condition.
- Do not collapse S2 basic and S2 high-intensity; intensity and problem type are different axes.
- Do not leave images as opaque media only; extract their reusable structure into text tables.
