---
name: lean-evidence-review
description: "Turn raw validation evidence into a conclusion status for lean experiments. Use when the user gives interview notes, user feedback, survey results, click data, sales messages, screenshots, usage logs, pilot results, trading samples, or experiment records and asks what they prove, how strong the evidence is, what is still unknown, or what to do next."
---

# Lean Evidence Review

Use this skill to separate evidence from interpretation. The job is to turn raw feedback and data into a status label and next action.

## Workflow

1. Inventory the evidence.
2. Separate observed behavior from opinions and interpretations.
3. Assign evidence level:
   - anecdote
   - single case
   - repeated qualitative signal
   - comparative preference
   - costly commitment
   - structured sample
   - quantitative result
4. Check bias and missing context.
5. Assign conclusion status.
6. Recommend the next action.

## Status Labels

- `unverified`: no usable behavior evidence yet
- `weak-positive`: some signal, too weak for major investment
- `mixed`: conflicting evidence or segment split
- `invalidated`: critical assumption failed
- `promising-next-round`: enough to run a stronger next test
- `validated-for-current-stage`: enough for the current stage only

## Output Shape

```text
Evidence inventory:
Observed behavior:
User statements:
Evidence level:
Bias / missing context:
Conclusion status:
What this proves:
What this does not prove:
Next action:
```

## Rules

- Do not upgrade praise into validation.
- Do not treat sample size as the only quality criterion.
- Prefer costly behavior over polite feedback.
- Mark the stage the evidence supports; do not overgeneralize.
- Keep counterexamples visible.
- If evidence is too messy, recommend better recording fields.

## When To Read References

- Read [references/evidence-ladder.md](references/evidence-ladder.md) when assigning evidence level.
- Read [references/review-card.md](references/review-card.md) when the user wants a copyable evidence review.

