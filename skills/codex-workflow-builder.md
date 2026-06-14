# Codex Workflow Builder Skill

## Purpose

Use this when a repeated task needs to be turned into a stable workflow that Codex can run or assist with.

## What It Does

- Converts a messy task description into a structured workflow
- Identifies inputs, outputs, review gates, and failure modes
- Separates reusable rules from one-off task details
- Produces a note that can be archived in Obsidian

## Input Contract

- Task name
- Goal
- Audience
- Frequency
- Input sources
- Constraints
- Output format
- Review requirement

## Output Contract

- Workflow purpose
- Step-by-step process
- Responsible agent roles
- Reusable prompt snippets
- Quality gates
- Archive path

## Operating Rules

- Keep one workflow focused on one repeatable task
- Make inputs and outputs explicit
- Mark human review points clearly
- Prefer structured bullets over long prose
- Stop and flag missing prerequisites instead of guessing

## Prompt Shape

```text
Task: ...
Goal: ...
Inputs: ...
Output: ...
Constraints: ...
Review gate: ...
Please turn this into a reusable Codex workflow.
```

## Best Use Cases

- New automation ideas
- Turning manual routines into repeatable workflows
- Converting workshop notes into operating procedures

## Failure Modes

- Vague outputs that cannot be executed
- Workflow steps that overlap too much
- Missing archive or review steps

## Related Notes

- [Workflows/knowledge-base-pipeline.md](../Workflows/knowledge-base-pipeline.md)
- [Concepts/repeatable-work.md](../Concepts/repeatable-work.md)
- [Workflows/workflow-index.md](../Workflows/workflow-index.md)
