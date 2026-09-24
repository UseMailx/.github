# Security Policy

This applies to every repository under the UseMailx organization that does not have its own `SECURITY.md`.

## Reporting a vulnerability

Please **do not** open a public GitHub issue for a security vulnerability. Instead:

- For the MailX server itself, use GitHub Private Vulnerability Reporting on [Ferousco-dev/Mailx](https://github.com/Ferousco-dev/Mailx/security/advisories/new).
- For an official SDK (`mailx-go`, `mailx-node`, `mailx-python`, `mailx-php`, `mailx-ruby`), use Private Vulnerability Reporting on that SDK's own repository, or report it against the server repo if it's unclear which one is affected.

Include a description of the issue, the affected component and version, reproduction steps, and potential impact. Never include real API keys, SMTP credentials, or other secrets in a report.

## Scope

The SDKs are thin HTTP clients — most security-relevant surface (authentication, delivery, data handling) lives in the server. If you're unsure which repo a report belongs to, report it against the server; it will be redirected if needed.
