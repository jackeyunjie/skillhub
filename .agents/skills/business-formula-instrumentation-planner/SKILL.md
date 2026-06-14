---
name: business-formula-instrumentation-planner
description: "Design the data nodes, event tracking, measurement fields, and validation sequence behind a business formula. Use when the user has a formula or hypothesis but lacks instrumentation, buried data, behavior indicators, dashboard metrics, experiment fields, funnel tracking, customer-success records, sales pipeline data, or an evidence layer to decide continue, stop, or adjust."
---

# Business Formula Instrumentation Planner

Use this after the formula and priority parameters are known. The job is to make the formula observable.

## Workflow

1. Capture the formula or hypothesis.
2. Identify the critical stages or nodes.
3. Assign behavior indicators to each node.
4. Define event / field names and metric definitions.
5. Prioritize instrumentation by decision value.
6. Separate monitoring metrics from experiment metrics.
7. State what decision each metric supports.

## Output Shape

```text
Formula / hypothesis:
Critical nodes:
Behavior indicators:
Recommended tracking fields:
Metric definitions:
Priority order:
Monitoring metrics:
Experiment metrics:
Decision supported:
Implementation notes:
```

## Rules

- Instrument the core contradiction first.
- Every metric should support continue, stop, or adjust decisions.
- Avoid measuring everything before measuring the failing node.
- Record failures, drop-offs, and non-responses, not only successes.
- Define segments and time windows early.

## Instrumentation Priority

1. Node where the main drop-off or uncertainty happens.
2. Behavior that proves the qualitative assumption.
3. Counterexample or failure condition.
4. Outcome metric.
5. Diagnostic context fields.

## When To Read References

- Read [references/instrumentation-fields.md](references/instrumentation-fields.md) for common field patterns.
- Read [references/instrumentation-card.md](references/instrumentation-card.md) when a copyable plan is needed.

