# Claude Code Skills

A collection of reusable skills for [Claude Code](https://claude.ai/code) that standardize common development workflows.

## Skills

### `/commit`

Generates standardized git commits using strict [Conventional Commits](https://www.conventionalcommits.org/) formatting.

**Rules enforced:**
- Single-line message only
- Conventional Commits prefix (`feat:`, `fix:`, `chore:`, `style:`, `refactor:`, `docs:`)
- Third-person present tense verb after the prefix (`adds`, `removes`, `fixes`, `updates`) — never past tense or imperative
- Lowercase throughout, except for exact codebase identifiers (e.g., class names, variables)
- No AI co-author tags

**Usage:** `/commit`

---

### `/workflow`

A structured, 7-step framework for planning and executing complex multi-step tasks with full alignment before any code is written.

**Steps:**
1. **High-level goal** — Claude asks what the overarching goal is before touching anything
2. **Interview** — Clarifying questions asked one at a time; codebase explored when relevant
3. **Planning** — Sequential task list ordered from foundational to complex
4. **Summary** — Goal, decisions, and plan presented for approval before execution begins
5. **Execution mode** — Choose between `Hands On` (approval between each step) or `Hands Off` (autonomous)
6. **Execution** — Tasks run in order with progress tracking, diffs, and rationale shown between each step
7. **Wrap up** — Final summary of all changes and how they satisfy the original goal

**Usage:** `/workflow`

## Installation

Skills live in `~/.claude/skills/`. Claude Code automatically makes them available as slash commands using the folder name.

To install:
```sh
git clone <this-repo> ~/.claude/skills
```

Or copy individual skill folders into `~/.claude/skills/`.