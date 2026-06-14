---
name: business-formula-qual-to-quant-converter
description: "Convert qualitative business judgments into observable behaviors and measurable indicators. Use when the user mentions trust, value perception, urgency, satisfaction, customer success, product interest, willingness to pay, user experience, brand, pain point, activation quality, switching cost, stickiness, or other fuzzy business factors and needs metrics, proxies, definitions, or data fields."
---

# Business Formula Qual To Quant Converter

Use this when teams are using soft words that cannot yet be tracked or tested.

## Workflow

1. Capture the qualitative judgment.
2. Define what the word means in this business context.
3. Identify observable behaviors behind it.
4. Propose candidate metrics and exact definitions.
5. Choose the minimum viable metric set.
6. Separate monitoring metrics from experiment metrics.

## Output Shape

```text
Qualitative judgment:
Context-specific definition:
Observable behaviors:
Candidate metrics:
Minimum viable metric set:
Monitoring metrics:
Experiment metrics:
Data collection method:
Warning:
```

## Rules

- Every qualitative statement needs at least one behavior proxy.
- Prefer recordable metrics over elegant but unavailable metrics.
- Use multiple weak proxies when no single direct metric exists.
- Do not let a proxy pretend to be the full truth.
- Define numerator, denominator, time window, and segment when possible.

## Common Mappings

- Trust: proof exposure, dwell time, inquiry rate, objection reduction, payment completion.
- Urgency: time-to-action, follow-up response, immediate booking, deadline sensitivity.
- Value perception: feature usage, willingness to pay, repeat visit, comparison preference.
- Satisfaction: repeat behavior, refund rate, complaint rate, recommendation, completion.
- Customer success: activation, usage depth, stakeholder adoption, value report acceptance.

## When To Read References

- Read [references/soft-factor-metrics.md](references/soft-factor-metrics.md) for common qualitative-to-metric mappings.
- Read [references/metric-definition-card.md](references/metric-definition-card.md) for copyable metric definitions.

