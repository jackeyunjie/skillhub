---
name: codex-agent-first-workflow
description: "Turn repeatable tasks into Codex-run workflows, automations, and reusable Obsidian knowledge assets. Use when the user wants to redesign a repeated task with Agent First thinking, create Codex automations, build content/video/query-webapp workflows, convert workshop notes into a reusable workflow, or package a task into a skill/agent split."
---

# Codex Agent First Workflow

Use this skill when a task repeats, can be described clearly, or should be converted into a reusable Codex workflow.

## Start Here

1. Identify the repeatable task.
2. Decide the output artifact.
3. Choose the right mode:
   - automation
   - content factory
   - video editing
   - query webapp
   - knowledge base capture
4. Separate workflow steps from agent roles.
5. Save the stable contract into Obsidian.

## Core Operating Rules

- Start from the output, not the prompt.
- Keep one skill focused on one repeatable job.
- Make inputs, outputs, review gates, and failure modes explicit.
- Prefer source-backed facts over interpretation.
- Mark any external plugin or service dependency clearly.
- Do not duplicate long reference material in this file; keep details in `references/`.

## Decision Map

- Use `automation` when the task should recur on a schedule.
- Use `content factory` when one source item should become research, visual concepts, and script.
- Use `video editing` when the output is a talking-head clip that needs cleanup and subtitles.
- Use `query webapp` when structured data should become a searchable page.
- Use `knowledge base capture` when a successful run should become reusable notes.

## When To Read References

- Read [references/automation.md](references/automation.md) for recurring tasks and daily briefing patterns.
- Read [references/content-factory.md](references/content-factory.md) for source-to-script workflows.
- Read [references/video-editing.md](references/video-editing.md) for clip cleanup and subtitle regeneration.
- Read [references/query-webapp.md](references/query-webapp.md) for spreadsheet-to-webapp flows.
- Read [references/knowledge-base.md](references/knowledge-base.md) for Obsidian capture patterns.
- Read [references/plugin-catalog.md](references/plugin-catalog.md) for the plugin map from the talk.

## Prompt Contract

```text
Task: ...
Goal: ...
Inputs: ...
Output: ...
Constraints: ...
Review gate: ...
External tools/plugins: ...
Please turn this into a reusable Codex workflow.
```

## Package Shape

- Keep the skill folder lean.
- Put variant-specific details in `references/`.
- Keep this file as the routing layer.
