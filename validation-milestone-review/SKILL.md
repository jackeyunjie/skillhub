---
name: validation-milestone-review
description: Use when reviewing lean validation results to decide whether evidence is enough, whether to continue, stop, pivot, increase sample size, run another MVP round, or enter the next stage. Trigger on 测到什么程度、样本够不够、进入下一阶段、MVP一轮还是多轮、里程碑复盘、验证结果判断、证伪还是证实、是否进入增长阶段、单元模型是否成立.
---

# Validation Milestone Review

Use this skill to review validation evidence and decide the next milestone. The goal is not to declare success too early; it is to reduce fatal uncertainty step by step.

## Core Rule

```
早期小样本证伪，后期大样本证实。
```

Milestones are not bureaucracy. They keep later tests from masking earlier failure.

## Milestone Logic

Typical order:

1. Demand / scene exists.
2. Product core or solution works.
3. Unit model / business model works.
4. At least one growth channel works.
5. Scale and moat questions become worth testing.

Entering growth usually requires:

```
单元模型成立 + 找到一个增长渠道
```

Do not judge "growth readiness" from a single attractive metric. Put metrics into the core unit: one user, one SKU, one store, one course, one customer, one transaction, or one delivery unit.

## One Round Or Multiple Rounds

Use one MVP round when:

- One or two core hypotheses dominate the risk.
- Hypotheses sit in the same stage.
- Failure interpretation will be clear.
- The cost is small and reversible.

Use multiple rounds when:

- Hypotheses are distributed across demand, solution, model, and growth.
- Later hypotheses depend on earlier ones.
- Failure in a combined test would not reveal the broken link.
- A single full test would consume too much time, money, audience, or trust.

Decision question:

```
If this round fails, can we tell what failed?
```

If not, split the experiment.

## Evidence Review

### 1. Classify The Evidence

| Evidence type | Use |
|---|---|
| Weak signal | Raises attention; not enough for resource commitment |
| Strong disconfirmation | Enough to stop, narrow, or pivot |
| Strong qualitative signal | Enough to design next quantitative test |
| Small quantitative signal | Enough to continue if aligned with qualitative evidence |
| Large quantitative signal | Enough for scaling only if unit model is clear |

### 2. Interpret By Stage

| Stage | Good enough early | Needs later |
|---|---|---|
| Demand | users show real pain, time, switching, deposit, or repeat interest | larger segment proof |
| Product core | strong usage, choice, qualitative praise, repeat use, completion, referral | stable conversion/retention |
| Business model | credible price, CAC, delivery cost, payback, gross margin | repeatable unit economics |
| Growth | one channel has positive ROI and enough ceiling | channel repeatability and capability fit |

### 3. Decide Next Action

Use these actions:

- Stop: prerequisite or fatal assumption failed.
- Narrow: one segment/scene works, others do not.
- Iterate: signal exists but product core or path has friction.
- Quantify: qualitative signal is strong enough to measure.
- Scale test: unit model works and channel has plausible ROI.
- Park: not enough evidence and cost of more evidence is not justified.

## Common Reviews

### Sample Size Is Small

Ask whether the purpose was disconfirmation or confirmation. Small samples can be enough to disconfirm a bad assumption. They are rarely enough to prove a growth thesis.

### Users Say They Like It

Treat stated liking as weak. Look for behavior: payment, repeated use, completion, choice over alternatives, sharing, referral, or real workflow adoption.

### Metrics Are Mixed

Map the funnel. A good top-of-funnel metric does not rescue a broken core conversion or impossible delivery cost.

### Boss Wants To Test Everything

Show the hypothesis dependency chain. If alignment fails, execute the chosen path fully and set review checkpoints so the learning can become internal common sense.

## Output Template

```markdown
## 验证里程碑复盘

### 1. 本轮验证目标
- 主假设：
- 所属阶段：
- 本轮是证伪还是证实：

### 2. 证据摘要
| 证据 | 强弱 | 指向 | 备注 |
|---|---|---|---|
|  |  |  |  |

### 3. 判断
- 结论：停止 / 缩窄 / 迭代 / 定量验证 / 进入下一里程碑 / 暂停
- 理由：

### 4. 下一里程碑
- 下一个前置假设：
- 推荐测试：
- 样本与指标：
- 不应提前测试的内容：
```

## Guardrails

- Do not use "stages can run in parallel" as an excuse to skip prerequisites.
- Do not call a business model validated until the unit model is visible.
- Do not enter growth because a page, post, or ad performed well once.
- Do not ask for large samples before the hypothesis is split enough for small-sample disconfirmation.
