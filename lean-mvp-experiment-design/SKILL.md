---
name: lean-mvp-experiment-design
description: Use when designing a low-cost lean experiment, MVP, fake-door test, concierge/manual service test, borrowed-tool prototype, AI-assisted validation, or staged test plan for a business hypothesis. Trigger on 精益测试方案、MVP设计、低成本验证、假产品测试、人工服务验证、借用工具、AI辅助验证、灰度测试、转化路径测试、样本和指标设计.
---

# Lean MVP Experiment Design

Use this skill after the key hypothesis is clear. Design the lightest experiment that can disconfirm or support the hypothesis without building the full product.

## Core Rule

```
精益不是省小钱，省的是全盘失败的大钱。
```

AI can reduce execution cost, but it does not remove the need to split hypotheses. Use AI for faster materials, prototypes, scripts, mock services, and analysis; keep humans responsible for judgment.

## Experiment Ladder

Prefer the left side when it can answer the question.

| Level | Method | Use when |
|---|---|---|
| Fake-door | landing page, poster, sales page, course outline, product brochure, waitlist | Need interest/click/lead/payment signal before product exists |
| Concierge | human manually delivers what product would automate | Need outcome proof before system building |
| Wizard-of-Oz | user sees product-like interface; human/AI operates behind it | Need product experience signal without full tech |
| Borrowed-tool | modify existing tools, no-code, forms, groups, spreadsheets | Need workflow proof cheaply |
| AI-assisted prototype | AI generates copy, mockups, content, code, analysis | Need fast materials or partial automation |
| Minimum version | build only the critical path | Need real behavior on the core feature |
| Full system | build broader product | Only after earlier milestones justify it |

## Workflow

### 1. Write The Hypothesis As A Testable Sentence

Use:

```
For [user] in [scene], [problem] is painful enough that they will [behavior] when offered [solution], measured by [metric] within [time].
```

Bad: users like AI home-video beautification.

Good: home decor sellers with existing raw footage will submit 10 clips and pay for 3 edited videos after seeing a manually produced sample within 7 days.

### 2. Choose Disconfirmation First

Ask what evidence would make you stop, shrink, or pivot. Early experiments should find false assumptions cheaply.

Examples:

- Demand: users refuse to spend time, share data, book calls, leave deposit, or switch from existing workaround.
- Product core: users try once but do not repeat, do not choose it over alternatives, or do not give strong qualitative feedback.
- Business model: CAC, delivery cost, or payback makes the unit model impossible.
- Growth: one channel cannot produce acceptable ROI or enough ceiling.

### 3. Design The Lightest Test

Define:

| Field | Requirement |
|---|---|
| Hypothesis | One primary hypothesis only |
| Test asset | Fake page, manual service, prototype, sample, brochure, event, etc. |
| Audience | Exact segment and acquisition route |
| Behavior | What users must actually do |
| Metric | One primary metric and 2-3 secondary diagnostics |
| Threshold | Pass / fail / unclear |
| Cost cap | Time, money, sample, and opportunity cost |
| Fallback | Lighter route if blocked |

### 4. Pick Metrics By Business Type

| Type | Useful signals |
|---|---|
| Tool / AI product | core feature use, AI output adoption, repeat use, next-week return, willingness to pay |
| Content / course | paid trial, completion, strong feedback, comparison choice, referral, repeat purchase |
| Local / offline service | visit to paid conversion, premium conversion, repeat visit, delivery margin |
| Consumer product | observed scene behavior, comparison group, repeat purchase, packaging attention, usage friction |
| ToB | serious problem acknowledgment, decision-maker meeting, pilot commitment, paid PoC, delivery feasibility |
| Marketplace / two-sided | split buyer and supplier hypotheses; test each role separately |

### 5. Avoid Overbuilding

For a multi-layer conversion path, test one layer at a time:

```
lead → entry offer → core offer → repeat/retention → franchise/referral/scale
```

Do not test the final high-ticket or franchise stage before the earlier conversion path exists.

## Output Template

```markdown
## 低成本验证方案

### 1. 主假设
- 

### 2. 最轻实验
- 实验类型：
- 实验资产：
- 目标用户：
- 行为信号：
- 核心指标：
- 通过标准：
- 失败标准：
- 成本上限：

### 3. 执行步骤
1. 
2. 
3. 

### 4. 诊断指标
| 指标 | 用来判断 |
|---|---|
|  |  |

### 5. 降级路径
- 如果资源拿不到：
- 如果样本不够：
- 如果数据模糊：
```

## Guardrails

- Do not design a full MVP when a fake-door, concierge, or borrowed-tool test can answer the hypothesis.
- Do not test multiple unrelated hypotheses in one experiment unless the purpose is exploratory and the interpretation limits are explicit.
- Do not use AI-generated output as proof of demand; use it as a cheaper way to create test material or deliver service.
- For stated preference, prefer behavior: payment, deposit, repeated use, sharing, time spent, switching, completion, or referral.
