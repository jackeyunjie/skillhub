---
name: business-formula-causality-checker
description: "Audit whether a business formula, growth diagnosis, metric relationship, or claimed driver is causal enough to guide action. Use when the user wants to check causality, challenge a formula, review whether traffic/conversion/retention/pricing/content/sales/customer-success caused an outcome, avoid correlation mistakes, or identify missing variables and evidence."
---

# Business Formula Causality Checker

Use this after a formula or diagnosis claims "X drives Y".

## Workflow

1. Restate the claimed relationship.
2. Identify whether it is currently correlation, plausible mechanism, or causal enough for action.
3. Explain the transmission mechanism.
4. List alternative explanations.
5. Identify missing nodes or hidden variables.
6. State what evidence would increase confidence.
7. Recommend a safer next test or action.

## Output Shape

```text
Claim:
Current confidence:
Correlation or causality:
Transmission mechanism:
Alternative explanations:
Missing nodes / hidden variables:
Evidence needed:
Safer next test:
Decision warning:
```

## Rules

- Treat unexplained linkage as correlation first.
- Always propose at least one alternative explanation.
- Check whether the claimed driver precedes the outcome.
- Check whether the driver changes the right intermediate node.
- Do not accept before/after improvement as proof by itself.

## Common Traps

- Traffic rose and revenue rose, so traffic caused growth.
- Discounts raised conversion, so discounting is the right lever.
- More calls raised renewal, so calls caused renewal.
- A campaign worked once, so the formula is reusable.
- A high-performing segment proves the whole market.

## When To Read References

- Read [references/causality-checklist.md](references/causality-checklist.md) for audit prompts.
- Read [references/audit-card.md](references/audit-card.md) when a copyable causality audit is needed.

