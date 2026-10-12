# 56-Day Roadmap

Source: OWASP_Security_Lab_56_Day_Plan.md.
Check a day only after its deliverables and verification are recorded.
This roadmap does not claim implementation or test completion.

## Week 1 — Foundations
- [x] Day 01: Initialize repository, goals, scope, initial threat model, and Git hygiene.
- [ ] Day 02: Document HTTP basics and five annotated local requests.
- [ ] Day 03: Build an app skeleton with two test users and a fixture database.
- [ ] Day 04: Capture and replay three authorized local requests with Burp.
- [ ] Day 05: Configure pytest and linting; verify five baseline tests.
- [ ] Day 06: Complete two or three authorized access-control training labs.
- [ ] Day 07: Review foundations and verify setup from scratch.

## Week 2 — Access Control and Authentication
- [ ] Day 08: Reproduce cross-user profile access in a vulnerable local endpoint.
- [ ] Day 09: Build an authorization matrix and demonstrate intended failures.
- [ ] Day 10: Add ownership and permission checks; verify cross-user denials.
- [ ] Day 11: Add role restrictions and verify unauthorized roles are denied.
- [ ] Day 12: Implement login/logout and test authentication behavior.
- [ ] Day 13: Test session expiration and invalid tokens; write A01/A07 reports.
- [ ] Day 14: Compare vulnerable and fixed behavior with regression evidence.

## Week 3 — Injection and Misconfiguration
- [ ] Day 15: Demonstrate unsafe SQL behavior in a local toy search endpoint.
- [ ] Day 16: Use bound parameters and verify the same attack input is contained.
- [ ] Day 17: Demonstrate unsafe command construction using a harmless mock.
- [ ] Day 18: Verify untrusted HTML content is escaped.
- [ ] Day 19: Separate development/production configuration and reject unsafe settings.
- [ ] Day 20: Verify security headers and production error responses.
- [ ] Day 21: Finalize A05/A02 reports and reproducibility instructions.

## Week 4 — Web Risk Breadth
- [ ] Day 22: Produce pinned dependencies, an SBOM, and review notes.
- [ ] Day 23: Record a dependency audit and explain remediation decisions.
- [ ] Day 24: Verify secure password storage and password verification.
- [ ] Day 25: Document trust boundaries and three design abuse cases.
- [ ] Day 26: Verify tampered artifacts are rejected using safe fixtures.
- [ ] Day 27: Test sanitized security events and an alert threshold.
- [ ] Day 28: Test exceptional conditions and document all ten Web categories.

## Week 5 — LLM Foundations
- [ ] Day 29: Verify the official LLM taxonomy and record version, IDs, and sources.
- [ ] Day 30: Implement a provider interface with deterministic offline mocks.
- [ ] Day 31: Build a tiny mock-backed RAG demo with synthetic documents.
- [ ] Day 32: Document LLM trust levels and three explicit failure criteria.
- [ ] Day 33: Enforce permissions for a read-only tool and approval-required write action.
- [ ] Day 34: Create twelve labeled synthetic benign/adversarial cases.
- [ ] Day 35: Verify clean setup and offline tests; document optional API limits.

## Week 6 — LLM Security Scenarios
- [ ] Day 36: Record a synthetic prompt-injection baseline and success criterion.
- [ ] Day 37: Compare boundary protections using the same dataset.
- [ ] Day 38: Test unauthorized access to a synthetic canary secret.
- [ ] Day 39: Verify retrieval isolation and secret redaction.
- [ ] Day 40: Verify natural-language requests cannot bypass mock tool authorization.
- [ ] Day 41: Test deny-by-default tool policies, schemas, and audit records.
- [ ] Day 42: Write three scenario reports with verified taxonomy mappings.

## Week 7 — Evaluation and Quality
- [ ] Day 43: Define valid runs, attack success, denominators, and benign cases.
- [ ] Day 44: Build a deterministic offline replay runner with JSON results.
- [ ] Day 45: Optionally run repeated live API cases with an explicitly approved budget.
- [ ] Day 46: Compute attack success and legitimate-task success from actual runs.
- [ ] Day 47: Verify installation and replay in a fresh environment.
- [ ] Day 48: Verify CI linting, tests, and secret scanning without live API calls.
- [ ] Day 49: Audit evidence hygiene, licenses, references, and mappings.

## Week 8 — Portfolio and Final Review
- [ ] Day 50: Polish README goals, architecture, scope, and quickstart.
- [ ] Day 51: Link actual Web coverage to code, tests, and reports.
- [ ] Day 52: Write an evidence-backed LLM case study.
- [ ] Day 53: Review reports for root cause, mapping, remediation, and limitations.
- [ ] Day 54: Run a five-to-seven-minute demonstration and record actual outputs.
- [ ] Day 55: Draft truthful CV bullets backed by project evidence.
- [ ] Day 56: Audit a fresh clone, document remaining issues, and create a release/tag.
