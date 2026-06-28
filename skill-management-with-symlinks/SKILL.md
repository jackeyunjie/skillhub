---
name: skill-management-with-symlinks
description: Use when the user wants to set up, organize, or maintain Agent Skills in a project-local, symlink-based way. Use for installing skills per-project only, saving context window space, keeping a single source of truth for shared skills, and updating skills across multiple projects with one pull.
---

# Skill Management with Symlinks

A geek-style workflow for managing Agent Skills: install them **project-local only**, and use **symbolic links** to point every project to a single source of truth.

This is opinionated. It may not fit everyone. But it saves context space and makes maintenance trivial once set up.

---

## Core Principles

### 1. Install Skills Inside Projects Only

Agent Skills can be installed globally (shared across all projects) or locally (only the current project sees them).

Choose **project-local only**.

Why:

- The agent's context window is limited. Every Skill name, description, and trigger text consumes space. The more global Skills you have, the more noise the agent carries around.
- More global Skills means a higher chance of false-positive triggers. When the agent thinks a Skill is relevant, it loads the full content. Unused global Skills can waste tokens and attention.
- Project-local Skills keep the workspace clean: only the Skills needed for the current task are visible.

Rule of thumb: if a Skill is not used by the current project, it should not be inside it.

### 2. Use Symbolic Links to Install Skills

This is the heart of the workflow.

A symbolic link is like a shortcut: the real file lives in one place, and many links can point to it. Update the original, and every link reflects the change immediately.

#### Step 1: Keep a Central Clone of Every Skill Source

Create a dedicated folder on your machine for GitHub projects that contain Skills. Example:

```text
~/GitHub/
  baoyu-skills/      ← upstream skill collection
  baoyu-design/      ← another skill source
  baoyu-writing/     ← your own writing project
```

Keep the original Skill files inside these clones. Do not copy them around.

#### Step 2: Symlink Skills Into Each Project

Inside a project that needs a Skill, create a symlink instead of copying.

Example on macOS / Linux:

```bash
ln -s ~/GitHub/baoyu-skills/skills/baoyu-comic \
  ~/GitHub/baoyu-writing/.agents/skills/baoyu-comic
```

Example on Windows (PowerShell, as Administrator):

```powershell
New-Item -ItemType SymbolicLink `
  -Path "C:\Users\You\GitHub\baoyu-writing\.agents\skills\baoyu-comic" `
  -Target "C:\Users\You\GitHub\baoyu-skills\skills\baoyu-comic"
```

Result:

```text
baoyu-writing/
  .agents/
    skills/
      baoyu-comic      →  ~/GitHub/baoyu-skills/skills/baoyu-comic
      baoyu-design     →  ~/GitHub/baoyu-design/skills/baoyu-design
```

#### Step 3: Give Your Agent Runtime an Entry Point

Claude Code looks for Skills under `.claude/skills/`. Create a symlink so it can follow the chain:

```bash
ln -s .agents/skills .claude/skills
```

Now Claude Code sees the same Skills that the OpenAI Agents SDK or Kimi sees under `.agents/skills/`.

For Kimi Code CLI, `.agents/skills/` is already a recognized project-level path, so no extra entry point is needed.

### 3. Let the Agent Create the Symlinks

You do not need to memorize the `ln -s` command. Just tell the agent in plain language:

> 帮我把 ~/GitHub/baoyu-skills/skills/baoyu-comic 软链接到 .agents/skills/baoyu-comic

Or even simpler:

> 帮我把 baoyu-skills 项目里的 baoyu-comic 这个 skill 链接到当前项目

The agent will:

1. Create the destination directory if needed
2. Create the symbolic link
3. Verify the link resolves correctly

The same applies to adding, removing, or updating links later.

---

## Why Bother?

Two big wins after the initial setup:

### Win 1: One Pull Updates Every Project

Because every project links to the same upstream clone, updating a Skill is a single operation:

```bash
cd ~/GitHub/baoyu-skills
git pull
```

All projects using `baoyu-comic` now have the latest version. No copy-paste, no drift.

### Win 2: Bug Fixes Flow Back to the Source

When you find a bug while using a Skill in one project, ask the agent to fix it. Because the project uses a symlink, the agent edits the upstream clone (`~/GitHub/baoyu-skills/skills/baoyu-comic`), not a local copy. After fixing, you can commit and push the improvement back to the original open-source project—turning a private fix into a public contribution.

---

## When to Use This Skill

Use this skill when the user asks about:

- How to organize Agent Skills across projects
- Whether to install Skills globally or locally
- How to avoid wasting context window on unused Skills
- How to keep Skills updated across many projects
- How to contribute fixes back to Skill authors
- Setting up `.agents/skills/`, `.claude/skills/`, or `.kimi/skills/`

---

## Workflow

1. **Identify the Skill source**
   - Which GitHub repo contains the Skill?
   - Where is the Skill directory inside that repo?

2. **Identify the target project**
   - Which project needs the Skill?
   - Which agent runtime will use it? (Claude Code, Kimi, OpenAI Agents SDK, etc.)

3. **Create the symlink**
   - Project path: `.agents/skills/<skill-name>`
   - Source path: `~/GitHub/<source-repo>/<path-to-skill>`
   - Also create `.claude/skills → .agents/skills` if using Claude Code and it does not already exist

4. **Verify**
   - Check that the link resolves: `ls -la .agents/skills/<skill-name>`
   - Check that the agent runtime discovers the Skill
   - Run a quick smoke test by invoking the Skill

5. **Maintain**
   - Update upstream clones with `git pull`
   - Add or remove symlinks as project needs change
   - Commit fixes to upstream when you improve a Skill

---

## Naming Rules

- Use the same directory name in the project as the upstream Skill directory uses.
- If a project needs a modified version, do not overwrite the upstream symlink. Create a local copy with a different name (e.g., `baoyu-comic-local`) and explain why it diverges.
- Keep `.agents/skills/` as the canonical project-level Skills folder. Runtime-specific folders (`.claude/skills/`, `.kimi/skills/`) should symlink to it.

---

## Common Commands

Create a symlink on macOS / Linux:

```bash
ln -s <source> <destination>
```

Create a symlink on Windows PowerShell:

```powershell
New-Item -ItemType SymbolicLink -Path <destination> -Target <source>
```

Verify a symlink:

```bash
ls -la <destination>
```

Remove a symlink (does not delete the source):

```bash
rm <destination>
```

Pull all upstream Skill repos:

```bash
for dir in ~/GitHub/*-skills ~/GitHub/*-design; do
  [ -d "$dir" ] && (cd "$dir" && git pull)
done
```

---

## Minimum Deliverable

When helping the user apply this skill, the default output should be:

- A verified symlink inside `.agents/skills/<skill-name>`
- A `.claude/skills → .agents/skills` symlink if Claude Code is used
- A short note explaining where the original lives and how to update it

---

## Related Skills

- `course-to-obsidian`: when the user wants to land course materials into Obsidian
- `如何做成好的Skill`: when the user wants to design a new Skill from scratch in Chinese
- `writing-great-skills`: when the user wants to improve Skill writing quality
