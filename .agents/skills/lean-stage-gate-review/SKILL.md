---
name: lean-stage-gate-review
description: "Review validation results and decide whether a project, product idea, business experiment, AI workflow, campaign, course, service, or strategy should advance, pause, pivot, or run another test. Use when the user asks whether evidence is enough for the next stage, whether to invest more, how to interpret MVP results, what milestone comes next, or if current validation is sufficient."
---

# Lean Stage Gate Review

Use this skill after one or more validation rounds. The job is to protect the user from skipping dependencies or over-investing on weak evidence.

## Workflow

1. State the stage and next investment decision.
2. List evidence already collected.
3. Identify the previous-stage dependency.
4. Judge evidence strength by stage:
   - subjective confidence
   - qualitative feedback
   - comparative preference
   - orders / commitments
   - interval quantitative signal
   - quantitative evaluation
5. Decide: advance, explore next stage cheaply, continue current test, pivot, or stop.
6. Name the missing evidence if not advancing.

## Output Shape

```text
Current stage:
Next decision:
Evidence summary:
Dependency check:
Evidence strength:
Decision:
Reason:
Allowed next actions:
Forbidden next actions:
Missing evidence:
Next test if needed:
```

## Decision Rules

- Do not skip a prerequisite assumption.
- Low-cost exploration of a later stage is allowed only after the current core assumption has a directional read.
- A local positive signal does not justify full-scale investment.
- One-round MVP is enough only when risk is concentrated and easy to observe.
- Multi-round system testing is required when risks are layered, interdependent, or high-cost.

## Stage Signals

- Early stage: concrete behavior and qualitative clarity matter more than statistical precision.
- Middle stage: compare alternatives, observe repeat behavior, and seek commitments.
- Late stage: unit economics, consistency, and quantitative reliability matter more.

## When To Read References

- Read [references/gate-criteria.md](references/gate-criteria.md) for advance / pause / pivot criteria.
- Read [references/review-template.md](references/review-template.md) when the user wants a copyable review.

