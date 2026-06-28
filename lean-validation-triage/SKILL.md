---
name: lean-validation-triage
description: Use when deciding whether a business uncertainty should be handled by common sense, expert interview, competitor/benchmark research, user research, survey, or a lean experiment. Trigger on 精益验证分流、要不要做MVP、专家访谈还是调研、问卷样本量、验证成本、降低试错成本、验证手段选择、or when a user asks how to validate a business question with the lowest cost.
---

# Lean Validation Triage

Use this skill to choose the cheapest reliable way to get the next piece of business evidence. The default bias is: do not run an experiment if the answer already exists in common sense, experts, competitors, or public/gray research.

## Core Rule

```
先拿别人已经有的答案 → 再做定性研究 → 最后才自己做实验
```

Cost order, from low to high:

1. Common sense / industry baseline: use when the issue is an established rule, basic constraint, or obvious impossibility.
2. Expert interview: use when industry practitioners can answer the risk from experience.
3. Competitor / benchmark research: use when similar businesses already ran the test.
4. User interview / field observation: use when the problem, scene, motivation, or decision logic is unclear.
5. Survey: use only after qualitative work has narrowed options enough for structured choices.
6. Lean experiment / MVP: use when prior sources cannot answer the specific high-risk hypothesis.

## Workflow

### 1. Restate The Uncertainty

Do not accept vague questions like "how many samples do I need" or "how should I validate this." First pin down:

| Field | Ask |
|---|---|
| Product form | Is it app, course, book, service, store, SaaS, hardware, consumer product, content, or offline training? |
| Stage | Is this opportunity pre-judgment, demand validation, product core, business model, or growth? |
| Hypothesis | What exactly might be false? |
| Failure cost | If this is false, does the business die, waste a sprint, or just lose a minor optimization? |
| Existing evidence | Who may already know the answer? |

If product form or stage is unclear, say that validation method, sample size, and metrics cannot be responsibly chosen yet.

### 2. Pick The Evidence Route

| Situation | Prefer | Avoid |
|---|---|---|
| Industry rules or feasibility are known by insiders | Expert interview | Building an MVP to rediscover common knowledge |
| Similar players already exist | Competitor / benchmark research | Testing from scratch before studying them |
| Need to understand fine-grained user scenes | User interview / observation | Surveying before options are clear |
| Options are narrowed and need relative magnitude | Survey / small quantitative test | Open-ended questionnaires |
| Need real behavior or payment signal | Fake-door, concierge, manual service, borrowed tool, or MVP | Asking "would you buy" only |
| Need growth channel judgment | Channel evaluation: ROI, ceiling, test cost, capability fit | Testing growth before demand/product/business are plausible |

### 3. Separate Qualitative And Quantitative

- Use qualitative methods to find details, contradictions, scenes, language, and options.
- Use quantitative methods after options are limited and behavior definitions are clear.
- In demand validation, prefer disconfirming bad options over proving demand.
- In product-core validation, use core behavior metrics: conversion, repeat use, retention, repurchase, recommendation, high-quality feedback.

### 4. Treat Sample Size As Contextual

There is no universal sample size. Anchor it to product form and stage:

| Product / Business | Early evidence can be |
|---|---|
| ToB | A few serious customers can be meaningful if the demand is concentrated and decision makers are real |
| Offline training / local service | Dozens may reveal strong conversion or delivery problems |
| App / high-volume toC | Hundreds may be needed for paid conversion or retention signal |
| Content product | Tens to hundreds can test product core via strong feedback, choice, payment, completion, and referral |
| Consumer product | Observation in real scene, comparison groups, repeat purchase, and usage behavior matter more than stated liking |

Use small samples for early disconfirmation. Use larger samples only after the hypothesis survives and the question becomes confirmation or scaling.

## Output Template

```markdown
## 验证分流判断

### 1. 问题重述
- 产品形态：
- 当前阶段：
- 待验证假设：
- 如果假设为假，后果：

### 2. 最低成本证据路线
| 优先级 | 手段 | 为什么 | 产出 |
|---|---|---|---|
| 1 |  |  |  |
| 2 |  |  |  |
| 3 |  |  |  |

### 3. 不建议直接做的事
- 

### 4. 进入实验的前置条件
- 
```

## Guardrails

- Do not recommend surveys before qualitative options are clear.
- Do not recommend growth tests before demand, product core, and business model risks are located.
- Do not ask users whether they like an idea when behavior, payment, or usage can be observed.
- If competitors already answered the question, recommend researching or buying the answer before testing.
