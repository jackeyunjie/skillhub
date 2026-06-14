---
name: lean-hypothesis-decomposer
description: "Decompose a business idea, product concept, growth plan, AI workflow, content product, service, trading idea, or project proposal into lean validation hypotheses. Use when the user asks to identify key assumptions, risk order, validation questions, false assumptions, MVP focus, demand validation, product-market uncertainty, or what to test first before investing more."
---

# Lean Hypothesis Decomposer

Use this skill before designing tests. The job is to turn a vague idea into a small set of ranked assumptions.

## Workflow

1. State the current decision.
2. Classify the idea by risk structure:
   - demand: do people care enough?
   - value: does it solve a painful problem?
   - channel: can users be reached repeatedly?
   - conversion: will they take the next action?
   - delivery: can the promise be fulfilled?
   - retention: will behavior repeat?
   - economics: can the unit model work?
3. Split the idea into assumptions.
4. Rank assumptions by:
   - failure cost
   - uncertainty
   - dependency on other assumptions
   - cost to test
5. Select the critical assumption to test first.
6. Write the validation question in observable terms.

## Output Shape

```text
Current decision:
Business / project type:
Assumption map:
1. ...
2. ...
Critical assumption:
Why this comes first:
Observable validation question:
Invalidation condition:
What not to test yet:
```

## Rules

- Start from the decision, not the idea.
- Prefer one sharp assumption over a broad story.
- Do not design an MVP until the critical assumption is named.
- Separate user statements from user behavior.
- Force at least one invalidation condition.
- Mark assumptions that cannot be tested cheaply.

## Common Failure Modes

- Treating a solution idea as if demand is already proven.
- Testing "would you like this" instead of observing behavior.
- Testing channel or pricing before product kernel is clear.
- Treating one positive case as validation.
- Designing a full product when only one assumption needs testing.

## When To Read References

- Read [references/risk-structures.md](references/risk-structures.md) when choosing which assumption type should be tested first.
- Read [references/output-template.md](references/output-template.md) when the user wants a copyable worksheet.

