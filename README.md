# Agent Skills

Global, platform-neutral Agent skills for business formula analysis and lean validation.

## Skills

### Business Formula

- `business-formula-core-contradiction-finder`: find the real bottleneck before formula work.
- `business-formula-paradigm-selector`: choose the right formula family before decomposing metrics.
- `business-formula-parameter-deepener`: push broad metrics down to actionable parameters.
- `business-formula-qual-to-quant-converter`: turn fuzzy business judgments into measurable indicators.
- `business-formula-causality-checker`: audit whether a metric relationship is causal enough for decisions.
- `business-formula-instrumentation-planner`: design data nodes and evidence layers behind formulas.

### Lean Validation

- `lean-hypothesis-decomposer`: decompose ideas into ranked validation assumptions.
- `lean-mvp-test-designer`: design low-cost tests for risky assumptions.
- `lean-stage-gate-review`: decide whether validation evidence supports the next investment stage.
- `lean-evidence-review`: review raw feedback and data into evidence level, status, and next action.

## Structure

```text
.agents/
  skills/
    <skill-name>/
      SKILL.md
      agents/openai.yaml
      references/*.md
```

These skills avoid platform-specific instructions and are intended to be reusable by different agent runtimes.

