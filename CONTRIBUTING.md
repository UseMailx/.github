# Contributing

This applies to every repository under the UseMailx organization that does not have its own `CONTRIBUTING.md`.

- **Server changes** (SMTP engine, REST API, delivery pipeline, anything under `internal/` or `cmd/`) belong on [Ferousco-dev/Mailx](https://github.com/Ferousco-dev/Mailx) — see that repo's own `CONTRIBUTING.md` for the full workflow.
- **SDK changes** belong on the specific language's repo (`mailx-go`, `mailx-node`, `mailx-python`, `mailx-php`, `mailx-ruby`). Each SDK mirrors the server's OpenAPI contract (`internal/api/openapi.go` in the server repo) — if you're adding a method, check that the route/shape actually matches what the server exposes before opening a PR.

For anything else — bug reports, feature proposals, questions — open an issue on the repository the request is actually about.
