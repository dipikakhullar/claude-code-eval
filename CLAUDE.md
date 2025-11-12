# CLAUDE.md — Review Playbook (Short)

Context
- This is a TypeScript monorepo (Node 20). We use ESLint + Prettier, Vitest, and Playwright. Data layer is Prisma + Postgres.

Primary goals
- Security and correctness over style.
- Flag input validation, auth, access control, and database queries.

Non-goals
- Do not reformat files or rename symbols unless asked.
- Avoid commenting on unchanged files.

When reviewing PRs
- Focus on files that changed.
- Propose minimal, targeted fixes with line references.
- If risk is low, say so briefly.
