---
name: course-to-obsidian
description: Use when the user gives a course link or asks for 落地课程、参考文档、一页速查、Obsidian 笔记 in the S 级私董会 vault. Use for turning a course page, Feishu doc, or lesson page into both a full `03-参考文档/` note and a compact one-page checklist note, with Obsidian wikilinks and README index updates.
---

# Course To Obsidian

## Overview

Turn a course source into two vault-ready Markdown notes:

1. A full `03-参考文档/` note for method, framework, and structured details
2. A compact `一页速查` note for direct execution and quick lookup

Always preserve Obsidian usability:

- Use `[[wikilinks]]`
- Add cross-links between the full note and the quick note
- Update `README.md` under `03-参考文档`

## When To Use

Use this skill when the user:

- pastes a `yitang.top` lesson or `fs-doc` link
- asks for `落地课程`
- asks for `参考文档`
- asks for `一页速查`
- asks to keep output suitable for Obsidian
- asks to keep both long-form and quick-reference versions

## Workflow

1. Identify the source type.
   - `fs-doc`: prefer extracting document structure and durable points
   - `lesson`: prefer extracting course positioning, visible modules, and stable concepts
   - if the page is partial or image-heavy, explicitly note that the整理稿 is based on visible and confirmable content only

2. Decide whether the topic already exists.
   - If the same course already has a note, patch it
   - If not, create a new file in `03-参考文档/`
   - Prefer names like `课程名.md` and `课程名-一页速查.md`

3. Write the full note.
   - Include:
     - title
     - source
     - original URL
     - document positioning
     - completeness note if partial
     - course positioning
     - confirmable structure
     - core concepts
     - execution framework
     - related vault links
   - Do not pretend to have full正文 when only部分可见内容 was captured

4. Write the quick note.
   - Keep it action-oriented
   - Compress into:
     - one-sentence positioning
     - what problem it solves
     - key concepts
     - key steps
     - common mistakes
     - reusable prompts or checklist items

5. Add Obsidian links.
   - In the full note, add a `速查入口` pointing to the quick note
   - In the quick note, add an `关联正文` pointing to the full note
   - Link core concepts to existing `02-核心概念/` notes when appropriate

6. Update `README.md`.
   - Add one line for the full note
   - Add one line for the quick note
   - Keep the source/description phrasing consistent with nearby rows

7. Verify before closing.
   - Check filenames
   - Check title and top metadata lines
   - Check the README entries
   - Check both notes have working `[[wikilinks]]`

## Naming Rules

- Full note:
  - `课程名.md`
  - Example: `进阶课-学会提问.md`
- Quick note:
  - `课程名-一页速查.md`
  - Example: `进阶课-学会提问-一页速查.md`

When the existing vault already uses a stable alias or naming pattern, follow the existing pattern instead of inventing a new one.

## Writing Rules

- Full note should optimize for structured reuse, not verbatim recovery
- Quick note should optimize for fast execution, not completeness
- Prefer stable claims over speculative reconstruction
- When inferring from visible headings or module names, state that it is a cautious interpretation
- Keep style aligned with the existing vault:
  - concise headings
  - direct bullets
  - no unnecessary prose

## Minimum Deliverable

Unless the user says otherwise, the default deliverable is:

- one full note in `03-参考文档/`
- one quick note in `03-参考文档/`
- mutual Obsidian links between them
- `README.md` updated

## Related Skills

- Use `doc-land` when you need the broader vault landing rules
- Use this skill when the user specifically wants the dual-output pattern: full note plus quick note
