---
name: modeling-60-process
description: "Turn an error-prone repeated task into a concrete checklist, SOP, warm-up routine, or mnemonic process model. Use when the user asks to 做SOP, 拉清单, 写检查表, 沉淀流程, 流程建模, 操作手册, 执行卡片, 热身清单, onboarding checklist, or wants to capture painful lessons and peak-state conditions into a usable repeated process."
---

# Modeling 60 Process

Use this skill to build a 60-point process model: make uncertain work more stable by turning it into explicit actions.

## Start Here

1. Identify one repeated task.
2. Define the target result in one sentence.
3. Collect past failures, misses, and peak-state moments.
4. Convert them into time-based or action-based steps.
5. Add concrete boundaries, measures, and triggers.
6. Compress the final version into a checklist, card, or short mnemonic.

## Operating Rules

- Build for repeated real execution, not for explanation.
- Record painful mistakes and proven winning conditions, not generic advice.
- Prefer specific triggers such as time, sequence, environment, and tool placement.
- Replace vague phrases with observable actions.
- Keep the finished SOP short enough to use during work.
- If the process must be remembered under pressure, create a mnemonic version.

## Output Format

Return all of the following when possible:

1. Task definition
2. Failure modes
3. Peak-state conditions
4. Final checklist or SOP
5. Optional mnemonic or card version
6. Review note: what should be updated after the next run

## Rewrite Rules

- Rewrite `准备一下` into a visible action.
- Rewrite `保持状态` into a timed warm-up or measurable condition.
- Rewrite `检查设备` into named items and target state.
- Rewrite `避免出错` into the exact error to guard against.

## Prompt Contract

```text
Use $modeling-60-process.
Task: ...
Desired result: ...
Repeated mistakes: ...
Peak-state experience: ...
Constraints: ...
Please produce a concrete SOP, checklist, and an optional mnemonic version.
```

## Chinese Trigger Hints

- 帮我做这个任务的 SOP
- 把这个流程拉成清单
- 这个事情总出错，帮我做流程建模
- 给新人做一个可执行操作手册
- 把直播前准备沉淀成热身清单

## When To Read References

- Read [references/process-patterns.md](references/process-patterns.md) for the underlying logic, examples, and SOP shaping rules from the course notes.
