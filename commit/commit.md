# commit

**Description:** A streamlined utility skill for reviewing repository changes and generating standardized, single-line commits using strict Conventional Commits formatting and specific verb tenses.

## Execution Instructions

When executing this skill, you must perform the following steps and strictly adhere to these formatting rules:

1. Review Changes: List all current modifications, deletions, and additions in the repository to accurately assess what needs to be committed.

2. One-Line Message: Formulate and execute the commit using a concise, single-line message.

3. Conventional Commits Format: Prefix the message using standard Conventional Commit types (e.g., feat:, fix:, chore:, style:, refactor:, docs:).

4. Third-Person Present Tense: The first word immediately following the prefix MUST be an action verb in the third-person present tense (e.g., "adds", "removes", "fixes", "updates"). You must NEVER use past tense (e.g., "added", "fixed") or imperative mood (e.g., "add", "fix").

5. Lowercase Preference: Write the entire commit message in lowercase. The only exception to this rule is when referencing specific programming terms, class names, or variables, which should retain their exact codebase casing (e.g., feat: adds UserType to group).

6. No AI Co-authors: Never append a co-author tag for yourself (the AI agent) to the commit message.