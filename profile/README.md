<div align="center">
  <h1>MailX</h1>
  <p>Open-source, developer-first email infrastructure built from the protocol up in Go.</p>

  <p>
    <a href="https://github.com/Ferousco-dev/Mailx"><img src="https://img.shields.io/badge/server-Ferousco--dev%2FMailx-635BFF?style=flat-square" alt="Server repository"></a>
    <a href="./LICENSE"><img src="https://img.shields.io/badge/license-MIT-00ADD8?style=flat-square" alt="MIT license"></a>
  </p>
</div>

## What this org is

MailX accepts mail over SMTP or a tenant-scoped REST API, stores the source message, processes delivery through a durable PostgreSQL and Redis pipeline, and exposes lifecycle events through signed webhooks. It's built to be understood and self-hosted, not a wrapper around a third-party provider.

There are two ways to use it:

- **Self-host it.** Clone the server, set a few environment variables, run it against your own Postgres and Redis. The whole thing is one Go binary plus two well-understood dependencies — no proprietary services required to run any part of it.
- **Use a hosted instance** — planned for later, once the server itself is further along. The SDKs already point at that future API by default so the same client code will work against either.

Every SDK in this org defaults to the hosted API but takes a `base_url` override, so self-hosted deployments work identically to the hosted one.

## Repositories

| Repo | What it is | Install |
| --- | --- | --- |
| [Ferousco-dev/Mailx](https://github.com/Ferousco-dev/Mailx) | The server. SMTP engine, REST API, delivery pipeline, DKIM/SPF/DMARC/BIMI, open/click tracking, contacts/audiences/broadcasts, webhooks. | `git clone` and run |
| [mailx-go](https://github.com/UseMailx/mailx-go) | Official Go SDK — a separate module from the server, no build coupling. | `go get github.com/UseMailx/mailx-go` |
| [mailx-node](https://github.com/UseMailx/mailx-node) | Official Node.js / TypeScript SDK. | `npm install mailx-sdk` |
| [mailx-python](https://github.com/UseMailx/mailx-python) | Official Python SDK. | `pip install mailx-sdk` |
| [mailx-php](https://github.com/UseMailx/mailx-php) | Official PHP SDK. | `composer require mailx/sdk` |
| [mailx-ruby](https://github.com/UseMailx/mailx-ruby) | Official Ruby SDK. | `gem install mailx-sdk` |

All five SDKs are published and installable today.

## Status

MailX is under active development and is not yet production-ready. Follow the server repo's own status notes before deploying anywhere untrusted traffic can reach it.

## Contributing

Issues and PRs are welcome on the server repo — see [CONTRIBUTING.md](https://github.com/Ferousco-dev/Mailx/blob/main/CONTRIBUTING.md).
