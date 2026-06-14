---
name: codex-talking-head-video-edit
description: "Clean up recorded talking-head or whiteboard videos by removing filler, pauses, and repetition, then regenerate subtitles. Use when the user has already recorded a video and wants Codex to handle rough-cut editing, subtitle regeneration, and low-value speech cleanup, especially with videocut-style workflows."
---

# Codex Talking Head Video Edit

Handle the repetitive post-recording cleanup work.

## Do This

1. Confirm the source video path.
2. Treat this as a post-recording workflow, not a scriptwriting workflow.
3. Remove filler, pauses, and repetition.
4. Regenerate subtitles from the edited audio.
5. Validate subtitle quality before calling the job done.
6. Output the final video and subtitle file in a clear location.

## Operating Rules

- Keep rough-cut automation separate from aesthetic final edit decisions.
- Do not hide subtitle uncertainty.
- Make the output filenames explicit.
- If the user has not installed the editing skill yet, say so and route installation first.

## When To Read References

- Read [references/edit-pattern.md](references/edit-pattern.md) for the standard sequence.
- Read [references/output-checks.md](references/output-checks.md) for validation after the cut.

