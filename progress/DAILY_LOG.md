# Daily Learning Log

## Day 01 — 2026-10-12

### Goal
Initialize the repository, document authorized scope and an initial threat
model, and verify the repository configuration.

### Status
In progress.

### Student-Performed Work
- Reported completing repository initialization and local Git identity setup.
- Created README.md, SECURITY.md, and .gitignore from AI-assisted drafts.
- Ran verification commands and supplied terminal output.
- Correctly explained authentication versus authorization.
- Recognized that public availability does not imply testing permission.
- Explained why .env is ignored and .env.example is tracked.
- Created LICENSE, ROADMAP.md, and progress documents from AI-assisted drafts.
- Staged seven Day 01 files and supplied the complete staged diff.
- Explained that client-controlled input may be used to bypass controls.
- Correctly identified user A as the actor and user B's profile as the asset.

### AI-Assisted Work
- Reviewed the full 56-day plan.
- Verified the official OWASP Web Top 10:2025 category names.
- Drafted project documentation and ignore rules.
- Reviewed supplied command output.
- Explained that remediation needs regression and legitimate-use tests.
- The chat mentor reviewed all seven staged files; no real credentials were observed in the supplied diff.
- Clarified the distinction between actors and assets.

### Verification Evidence
Student-supplied terminal output:

Command: git status --short
Observed:
    ?? .gitignore
    ?? README.md
    ?? SECURITY.md

Command: git diff --check
Observed: no output.
Limitation: the files were untracked, so their contents were not checked.

Command: git check-ignore .env .env.local .venv/example __pycache__/example.pyc
Observed: all four paths were printed.

Command: git check-ignore .env.example
Observed: no output, consistent with the example file not being ignored.

### Learning and Limitations
- Impact analysis does not replace verification of a security fix.
- Git author configuration does not authenticate a GitHub account.
- No application or security tests exist yet.
- Staged documentation was reviewed; the initial commit exists and the working tree was clean before this documentation update.
- Correctly distinguished actor and asset after clarification.

### Pending
- Verify Git author identity and staged whitespace checks.
- Verify a clean working tree after the current documentation update is committed.
- Configure account-specific GitHub authentication.

### Commit
Initial commit: d6e667b — day-01: initialize project scope and security documentation.
The current documentation update has not been committed.
