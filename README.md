# OWASP Security Lab

A 56-day learning project documenting security concepts, authorized
vulnerability reproduction, root-cause analysis, remediation, and
regression testing.

## Goals

- Understand all ten OWASP Web Top 10:2025 risk categories.
- Build selected local labs with vulnerable and fixed implementations.
- Document reproducible evidence and the limitations of each result.
- Explore LLM application security using mocks before optional API use.
- Maintain an honest record of student work and AI assistance.

## Planned Technology

Python 3.12, Flask or FastAPI, pytest, Docker, Burp Suite, and GitHub Actions.
LLM components will use deterministic mocks or API-based inference.
No model training or fine-tuning is planned.

## Authorized Scope

Testing is limited to self-built local applications and explicitly
authorized training labs. Only synthetic users, data, and test secrets
will be used.

Public availability does not imply permission to test a system.
Production systems and third-party targets without authorization are
outside this project's scope.

## Initial Threat Model

Status: planned; no application or security controls implemented yet.

| Element | Initial assumption |
| --- | --- |
| Assets | Synthetic user records, permissions, configuration, and future API credentials |
| Actors | Anonymous visitors, ordinary users, and administrators |
| Entry points | Future HTTP endpoints and LLM inputs |
| Trust boundaries | Client to server; server to database; future app to LLM provider |
| Threats | Cross-user access, privilege escalation, injection, and information disclosure |
| Planned controls | Server-side authorization, input handling, secret isolation, and regression tests |

This model will be revised as the application is implemented.

## Current Status

Day 01 complete — repository foundation verified.
No application or security tests implemented yet.
No vulnerability labs or security results are claimed as complete.

## Evidence Standard

Each completed lab must document its scope, root cause, reproduction,
observed results, impact, remediation, regression tests, and limitations.
Expected results and observed results must be distinguished.

## References

- OWASP Web Top 10:2025: https://top10.owasp.org/2025/
- OWASP Web Security Testing Guide: https://owasp.org/www-project-web-security-testing-guide/
- PortSwigger Web Security Academy: https://portswigger.net/web-security
