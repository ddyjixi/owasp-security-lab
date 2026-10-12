# Daily Learning Log

## Day 01 — 2026-10-12

### Goal
Initialize the repository, document authorized scope and an initial threat
model, and verify the repository configuration.

### Status
Complete — repository foundation verified using local checks and
student-provided evidence. No application or security tests implemented yet.

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
- Created the initial and learning-update commits listed below.
- Supplied WSL terminal evidence of a clean working tree and matching local
  HEAD and origin/main hashes after the learning-update commit.
- Reported using ~/.ssh/id_ed25519_ddyjixi for GitHub SSH authentication.

### AI-Assisted Work
- Reviewed the full 56-day plan.
- Verified the official OWASP Web Top 10:2025 category names.
- Drafted project documentation and ignore rules.
- Reviewed supplied command output.
- Explained that remediation needs regression and legitimate-use tests.
- The chat mentor reviewed all seven staged files; no real credentials were observed in the supplied diff.
- Clarified the distinction between actors and assets.
- Successfully re-checked the student's distinction between actor and asset.
- Verified the seven Day 01 files, all 56 roadmap tasks, README foundation
  sections, Git author identity, origin URL, and ignore behavior locally.
- Prepared and reviewed this Day 01 summary using student-provided remote
  synchronization evidence; did not independently verify remote synchronization.

### Verification Evidence
Early student-provided evidence (before the initial commit):

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

Closing student-provided evidence, run directly in the student's WSL terminal
after the learning-update commit and before this summary:

```text
git status --short --branch
## main...origin/main

git rev-parse HEAD
891aadb26ec0a69167a91484d1c92d09ea3870f2

git ls-remote origin refs/heads/main
891aadb26ec0a69167a91484d1c92d09ea3870f2 refs/heads/main
```

Prior whitespace checks (`git diff --check` and `git diff --cached --check`)
passed after the documentation was tracked and staged.

Codex local verification before this summary:
- All seven files exist: .gitignore, README.md, SECURITY.md, LICENSE,
  ROADMAP.md, progress/DAILY_LOG.md, and progress/SKILL_MATRIX.md.
- ROADMAP.md contains 56 tasks, numbered Day 01 through Day 56.
- README.md contains Goals, Authorized Scope, and Initial Threat Model.
- `git var GIT_AUTHOR_IDENT` reports ddyjixi <tuongkiemdrl@gmail.com>.
- Origin fetch and push URLs are
  `git@github-ddyjixi:ddyjixi/owasp-security-lab.git`.
- `git check-ignore .env .env.local .venv/example __pycache__/example.pyc`
  prints all four paths; `.env.example` produces no output (exit 1), as expected.
- Local HEAD matches the student-provided hash above; the working tree was
  clean before this summary was edited.

### Definition of Done

| Day 01 requirement | Evidence | Result |
| --- | --- | --- |
| Repository foundation and seven Day 01 files | Codex local file checks; existing commits | Met |
| Goals, authorized scope, and initial threat model | Codex review of README.md | Met |
| Full 56-day plan recorded | Codex verified 56 sequential roadmap tasks | Met |
| Git author identity and intended remote | Codex local identity and origin checks | Met |
| Ignore rules and safe example-file handling | Student explanation and local check-ignore results | Met |
| Documentation reviewed and whitespace checked | Mentor review of seven staged files; prior passing whitespace checks | Met |
| Initial work committed, clean, and synchronized | Student-provided WSL status and matching HEAD/origin hashes at 891aadb | Met |
| Foundation concepts understood | Correct authentication/authorization, actor/asset, and .env/.env.example explanations | Met |

### Learning and Limitations
- Impact analysis does not replace verification of a security fix.
- Git author configuration does not authenticate a GitHub account.
- No application or security tests exist yet.
- Correctly distinguished actor and asset after clarification; re-check passed.
- The threat model is preliminary; no controls, coding proficiency, security
  testing, or lab exploitation are demonstrated by this documentation work.
- Credential review was limited to the supplied staged diff; it was not a
  repository-wide secret scan.
- Codex could not authenticate to origin because this session could not access
  an SSH agent. The effective SSH configuration selects
  ~/.ssh/id_ed25519_ddyjixi, but the remote query failed with
  Permission denied (publickey). No private key, token, or passphrase was printed.
- Remote synchronization is accepted from student-provided evidence for
  891aadb only. It does not establish that this summary commit was pushed.

### Pending
- No Day 01 foundation requirement remains open under the evidence above.
- This summary's local commit and clean-tree verification are performed after
  editing; their outcome is reported separately, not assumed here.
- Publishing this summary remains a student follow-up; Codex will not push it.

### Commit
- Initial commit: d6e667b — day-01: initialize project scope and security documentation.
- Learning-update commit: 891aadb — day-01: update learning evidence and skill tracking.
- Summary commit message: day-01: finalize verified setup and learning log.
  Its creation is not claimed in advance; no summary push is claimed.
