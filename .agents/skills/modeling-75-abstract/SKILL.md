---
name: modeling-75-abstract
description: "Convert founder intuition, reviewer judgment, or non-standard selection experience into a reusable abstract evaluation model with dimensions, scales, and scoring rules. Use when the user asks to 抽象建模, 搭评估模型, 定评审标准, 做筛选框架, 做评分维度, 统一判断尺度, 人才筛选模型, 评审模型, or faces repeated screening, review, ranking, admission, hiring, and other high-frequency decisions that still depend on one person's feel."
---

# Modeling 75 Abstract

Use this skill to build a 75-point abstract model: turn unstable personal judgment into a team-usable evaluation framework.

## Start Here

1. Define the decision scene.
2. State what is being screened, ranked, or judged.
3. Collect successful and failed cases.
4. Compare them to find hidden dimensions.
5. Convert those dimensions into named axes and scoring rules.
6. Test whether another person could use the model without the original expert.

## Operating Rules

- Build for repeated decision scenes, not one-off analysis.
- Use dimensions that stay stable across cases.
- Separate dimensions from examples.
- Add explicit scoring rules or threshold descriptions.
- Prefer 3 to 5 dimensions unless complexity truly requires more.
- Reject decorative models that look good but do not improve independent judgment.

## Minimum Viable Model

Return all of the following:

1. Decision scene
2. What the expert currently judges by feel
3. Core dimensions
4. Definition of each dimension
5. Scoring or rating rule
6. How to use the model in a real review conversation
7. Failure test: where the model may still break

## Validation Rule

The model passes only if a competent teammate can use it to make above-pass-line decisions in a high-frequency, complex, expensive-to-miss scenario.

If people still need to ask the expert every time, the model is not done.

## Prompt Contract

```text
Use $modeling-75-abstract.
Decision scene: ...
What is currently judged by feel: ...
3 strong cases: ...
3 weak cases: ...
Constraints: ...
Please extract 3-5 dimensions, define scoring rules, and produce a reusable evaluation model.
```

## Chinese Trigger Hints

- 帮我做一个筛选模型
- 这事现在全靠拍板，帮我抽象建模
- 把这个评审标准做成统一框架
- 从这些成功和失败案例里提炼评分维度
- 帮我做一个团队能共用的判断模型

## When To Read References

- Read [references/abstract-models.md](references/abstract-models.md) for the course logic, model quality bar, and example dimension design.
