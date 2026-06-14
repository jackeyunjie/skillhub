---
name: business-formula-paradigm-selector
description: "Choose the correct business formula family before decomposing metrics. Use when the user is analyzing GMV, revenue, conversion, retention, renewal, repurchase, customer success, lead generation, pricing, acquisition, or growth but is unsure whether to use transaction, lifecycle, retention, renewal, node-conversion, continuous-action, or value-expansion logic."
---

# Business Formula Paradigm Selector

Use this before metric decomposition. The job is to prevent using the wrong formula for the wrong business type.

## Workflow

1. Identify the business model and customer relationship depth.
2. State the current target and visible gap.
3. Classify the primary bottleneck:
   - acquisition
   - conversion
   - trust
   - activation
   - usage depth
   - retention / repurchase
   - renewal
   - value expansion
   - delivery capacity
4. Choose the formula family.
5. Reject at least one tempting but wrong formula family.
6. State what to decompose next.

## Output Shape

```text
Business type:
Customer relationship depth:
Current target:
Visible gap:
Primary bottleneck:
Recommended formula family:
Formula skeleton:
Wrong-but-tempting formula:
Reason:
Next decomposition target:
```

## Formula Families

- Single transaction: `Revenue = leads x conversion rate x average order value`
- Continuous repurchase: `Revenue = active customers x purchase frequency x average order value x retention`
- Renewal / subscription: `Renewal revenue = active accounts x renewal rate x contract value`
- Node conversion: `Outcome = node 1 rate x node 2 rate x node 3 rate`
- Continuous action: `Outcome = trigger x action completion x repeat behavior`
- Value expansion: `Revenue = base value + upgrade value + cross-sell value + referral value`

## Rules

- Classify before decomposing.
- Do not default to `GMV = traffic x conversion x AOV x repurchase`.
- Mixed models still need one primary bottleneck.
- Choose the formula that exposes the current contradiction, not the formula that looks most complete.

## When To Read References

- Read [references/formula-families.md](references/formula-families.md) for detailed family selection.
- Read [references/selector-card.md](references/selector-card.md) when a copyable worksheet is needed.

