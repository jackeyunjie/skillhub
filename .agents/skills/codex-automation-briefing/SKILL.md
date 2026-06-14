---
name: codex-automation-briefing
description: "Design and run recurring Codex automations for briefings, summaries, and scheduled repeatable tasks. Use when the user wants a task to run daily/weekly, wants a stable automation spec with trigger time, input sources, output paths, completion summary, or wants to turn an already-manual task into a scheduled Codex automation."
---

# Codex Automation Briefing

Turn a repeatable task into a stable Codex automation.

## Do This

1. Confirm the task repeats and has a clear output artifact.
2. Write the minimum viable automation spec:
   - task name
   - goal
   - trigger time
   - frequency
   - input sources
   - processing rules
   - output path
   - output format
   - completion summary
   - failure handling
3. Keep the first version narrow. One automation should do one job.
4. Make the output path explicit.
5. Keep the completion summary short enough to scan in seconds.

## Operating Rules

- Start from a task that has already run successfully by hand.
- Prefer stable sources over broad source sprawl.
- Mark missing sources explicitly.
- Keep dates exact.
- Preserve a review gate for public or high-risk outputs.

## When To Read References

- Read [references/spec-template.md](references/spec-template.md) to draft the automation contract.
- Read [references/daily-intel.md](references/daily-intel.md) for multi-source briefing patterns.
- Read [references/failure-patterns.md](references/failure-patterns.md) when the task is brittle or source-dependent.

