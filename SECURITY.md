# Security Policy

## Intended Use

This repository is an educational security lab. Future vulnerable
examples will be intentionally unsafe and must remain in isolated,
authorized environments.

## Testing Boundaries

- Test only self-built local applications or explicitly authorized labs.
- Use synthetic data and dedicated test accounts.
- Keep local services bound to loopback unless an isolated setup
  explicitly requires otherwise.
- Do not expose vulnerable services to the public internet.
- Do not use real personal data or production credentials.

## Secrets and Evidence

Keep credentials outside version control. Use ignored environment files
when credentials are required.

Review logs, screenshots, request samples, and Git diffs before committing.
Remove tokens, cookies, credentials, personal data, and private paths.

If a real credential is exposed, revoke or rotate it. Deleting a file
alone does not remove it from Git history.

## Reporting

For unintended issues in this repository, report reproducible details
using synthetic data. Public reports must not include secrets or
sensitive information.

For issues in external software, follow the affected project's
disclosure policy and remain within its authorized scope.
