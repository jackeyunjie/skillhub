---
name: modeling-router
description: "Route a modeling request to the right layer among process modeling, abstract modeling, and essence extraction. Use when the user asks for 建模, 高阶建模, 建模能力, 做个模型, 这个问题怎么建模, or is unclear whether the need is SOP/process, evaluation framework/abstract model, or essence extraction/strategic definition."
---

# Modeling Router

Use this skill as the entry point when the user says they want to model something but the modeling layer is not explicit.

## Routing Decision

Choose exactly one primary path first:

1. Use `modeling-60-process` when the problem is unstable execution.
2. Use `modeling-75-abstract` when the problem is unstable judgment.
3. Use `modeling-85-essence` when the problem is unstable definition or strategic choice.

## Fast Diagnosis

Ask these internal questions:

1. Is the user asking how to do the task repeatedly with fewer mistakes?
   Route to `modeling-60-process`.
2. Is the user asking how to judge, screen, rank, review, or standardize choices across cases?
   Route to `modeling-75-abstract`.
3. Is the user asking what the topic really is, what its essence is, or how to define it for real decisions?
   Route to `modeling-85-essence`.

## Symptom Map

- `总出错 / 不稳定 / 交接困难 / 新人不会做 / 需要SOP`
  Route to `modeling-60-process`.
- `全靠拍板 / 标准不统一 / 评审很难 / 需要筛选框架 / 想做评分维度`
  Route to `modeling-75-abstract`.
- `概念很乱 / 想提炼本质 / 要做战略定义 / 需要压成一句话 / 要指导关键选择`
  Route to `modeling-85-essence`.

## Response Pattern

When routing, explicitly say:

1. Why this request belongs to 60, 75, or 85.
2. What artifact you will produce.
3. What input is most useful next.

## Output Artifacts By Layer

- `60`: checklist, SOP, warm-up list, mnemonic card
- `75`: dimensions, scoring model, review framework, decision rubric
- `85`: compressed definition, required elements, decision test

## Prompt Contract

```text
Use $modeling-router.
Problem: ...
Current pain: ...
What keeps going wrong: ...
What decision or result matters: ...
Please decide whether this should be modeled as 60, 75, or 85, then proceed with the right skill.
```
