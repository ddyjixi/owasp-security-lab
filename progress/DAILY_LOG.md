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

### AI-Assisted Work
- Reviewed the full 56-day plan.
- Verified the official OWASP Web Top 10:2025 category names.
- Drafted project documentation and ignore rules.
- Reviewed supplied command output.
- Explained that remediation needs regression and legitimate-use tests.
- Reviewed all seven staged files; no real credentials were observed.
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
- Staged documentation was reviewed; commit and clean-tree verification remain pending.
- Initially confused actors with assets; conceptual re-check remains pending.

### Pending
- Verify local Git author identity and staged whitespace checks.
- Create the first commit and verify a clean working tree.
- Configure account-specific GitHub authentication.

### Commit
Not created yet.
