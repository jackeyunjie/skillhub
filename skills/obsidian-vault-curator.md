# Obsidian Vault Curator Skill

## Purpose

Use this when a landing document, workshop note, or successful run should become a structured Obsidian vault rather than a loose summary.

## What It Produces

- A source note
- Concept notes
- Workflow notes
- Skill notes
- Agent notes
- Updated index pages

## Input Contract

- Source path or source link
- Topic or domain
- Target vault structure
- Required note types
- First import or incremental update

## Output Contract

- Clear split between raw source and derived notes
- Linked notes that are easy to scan in Obsidian
- Updated indexes that support the next run
- Explicit gaps and refresh path

## Operating Rules

- Start from the source layer, not interpretation.
- Separate concepts from procedures.
- Separate procedures from role boundaries.
- Keep each note narrow enough to be reused later.
- Update MOC and overview pages in the same pass.

## Prompt Shape

```text
Please turn this source into a structured Obsidian knowledge base.

Source: ...
Topic: ...
Need note types: concepts, workflows, skills, agents, sources
Update mode: first import / incremental refresh
Output requirement: reusable vault with indexes
```

## Quality Gates

- Source note exists
- Every derived note has a clear purpose
- MOC points to the new notes
- Notes guide future work instead of summarizing the past only

## Failure Modes

- Mixing source text and derived rules in one note
- Creating note sprawl with no linking page
- Writing generic summaries that cannot guide action

## Related Pages

- [Workflows/knowledge-base-capture-from-doc.md](../Workflows/knowledge-base-capture-from-doc.md)
- [Workflows/knowledge-base-pipeline.md](../Workflows/knowledge-base-pipeline.md)
- [Agents/knowledge-base-archivist-agent.md](../Agents/knowledge-base-archivist-agent.md)
