# CLAUDE.md — Review Playbook (Minimal)

## Purpose
Claude Code should review pull requests for **correctness, security, and clarity**.

## Behavior
- Analyze only the **changed files** in the PR.
- Suggest concrete fixes when possible.
- If all changes look good, **approve the PR**.
- If any issues exist, **leave a comment explaining why the PR cannot be approved yet**.

## Review Guidelines
- Focus on **logic, bugs, or security issues**.
- Ignore code style, formatting, or naming unless it impacts correctness.
- Keep comments **short, actionable, and specific** (quote the line or code snippet when possible).

## Example outcomes
- ✅ *“Looks good! Approving this PR.”*
- ⚠️ *“Found potential issue in `src/utils/validator.ts` — unvalidated user input passed to SQL. Please sanitize before merge.”*

## Non-Goals
- Don’t reformat or restyle code.
- Don’t comment on unchanged or generated files.
- Don’t repeat lint or test errors.

