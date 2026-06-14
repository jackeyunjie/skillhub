---
name: lean-mvp-test-designer
description: "Design the smallest credible validation test for a business hypothesis, product idea, growth tactic, AI workflow, content offer, service offer, or operational change. Use when the user asks for MVP design, low-cost experiment, smoke test, fake-door test, concierge test, prototype test, pilot plan, validation plan, or how to test an assumption before full build or large investment."
---

# Lean MVP Test Designer

Use this skill after the critical assumption is clear. The job is to design the lowest-cost test that can change a decision.

## Workflow

1. Restate the assumption and decision.
2. Choose the test type:
   - landing page / fake door
   - interview / problem discovery
   - concierge service
   - manual prototype
   - content sample
   - sales call / preorder
   - internal workflow pilot
   - data backtest / sample review
3. Define the minimum realistic context.
4. Define the behavior to observe.
5. Define success, weak-positive, mixed, and invalidated thresholds.
6. Define sample, timebox, cost, owner, and recording fields.
7. Add anti-bias controls.

## Output Shape

```text
Assumption:
Decision this test informs:
Test type:
Minimum setup:
Target sample:
Observed behavior:
Success threshold:
Weak-positive threshold:
Invalidation threshold:
Recording fields:
Timebox and budget:
Anti-bias controls:
Next action by result:
```

## Rules

- Test the smallest assumption, not the whole system.
- Prefer 10% of the cost if it can produce the same directional learning.
- Make the test realistic enough to observe behavior, not just opinion.
- Do not ask users to perform feedback theater.
- Do not use late-stage statistical standards for early directional tests.
- If failure would consume the whole budget, shrink the test.

## Test Selection

- Use interviews when the risk is problem clarity or buying process.
- Use fake doors when the risk is action intent.
- Use preorders or paid pilots when the risk is willingness to pay.
- Use concierge tests when delivery feasibility is uncertain.
- Use internal pilots when the risk is workflow repeatability.
- Use sample review/backtest when the risk is pattern stability.

## When To Read References

- Read [references/test-patterns.md](references/test-patterns.md) when choosing a test type.
- Read [references/test-card.md](references/test-card.md) when the user wants a copyable experiment card.

