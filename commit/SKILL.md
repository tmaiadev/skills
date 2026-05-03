---
name: commit
description: A streamlined utility skill for reviewing repository changes, logically grouping them, proposing a commit plan, and generating standardized commits sequentially to handle potential hooks. Uses strict Conventional Commits formatting and specific verb tenses.
---

## Execution Instructions

When executing this skill, you must perform the following steps and strictly adhere to these formatting rules:

1. Review and Group Changes: List all current modifications, deletions, and additions in the repository. Analyze the diffs and logically group related modifications together into distinct, isolated commits (e.g., keep database schema changes separate from UI styling updates).

2. Propose Commit Plan: Before making any actual commits, display a clear, formatted list of the commits you plan to make to the user for review. Stop and wait for the user's explicit approval before proceeding.

3. Sequential Execution: Once approved, execute the commits strictly one at a time. After executing a commit, check for any pre-commit hook executions, linting errors, or test failures. You must address and resolve any hook failures before moving on to the next commit in your plan.

4. One-Line Message: Formulate each commit using a concise, single-line message.

5. Conventional Commits Format: Prefix the message using standard Conventional Commit types (e.g., feat:, fix:, chore:, style:, refactor:, docs:).

6. Third-Person Present Tense: The first word immediately following the prefix MUST be an action verb in the third-person present tense (e.g., "adds", "removes", "fixes", "updates"). You must NEVER use past tense (e.g., "added", "fixed") or imperative mood (e.g., "add", "fix").

7. Lowercase Preference: Write the entire commit message in lowercase. The only exception to this rule is when referencing specific programming terms, class names, or variables, which should retain their exact codebase casing (e.g., feat: adds UserType to group).

8. No AI Co-authors: Never append a co-author tag for yourself (the AI agent) to the commit message.