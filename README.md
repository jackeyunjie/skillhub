# Agent Skills

Global, platform-neutral Agent skills for business formula analysis, lean validation, and Codex workflows.

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

### Codex Workflows

- `agent-first-vault-curator`: curate an Agent First Obsidian vault into reusable knowledge assets.
- `codex-agent-first-workflow`: turn repeatable tasks into Codex-run workflows and automations.
- `codex-automation-briefing`: design and run recurring Codex automations for briefings and summaries.
- `codex-content-factory`: convert a source item into a content production chain.
- `codex-knowledge-base-capture`: turn a successful Codex run into reusable Obsidian knowledge assets.
- `codex-query-webapp`: turn structured business data into a searchable web app.
- `codex-talking-head-video-edit`: clean up talking-head videos and regenerate subtitles.

### Markdown Skill Notes

Standalone skill specifications kept as single Markdown files.

- `ai-daily-radar`: automated daily intelligence radar.
- `automation-task-spec`: task specification for automations.
- `codex-intel-collector`: collect and structure intelligence with Codex.
- `codex-workflow-builder`: build reusable Codex workflows.
- `html-brief-generator`: generate HTML briefs from sources.
- `obsidian-vault-curator`: curate Obsidian vaults for agent use.
- `paper-board-html`: render paper board content as HTML.
- `query-webapp-builder`: build query webapps from structured data.
- `videocut-skills`: video editing skills for cutting and cleanup.

## Structure

```text
.agents/
  skills/
    <skill-name>/
      SKILL.md
      agents/openai.yaml
      references/*.md

skills/
  <skill-name>.md
```

These skills avoid platform-specific instructions and are intended to be reusable by different agent runtimes.
