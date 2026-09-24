<div align="center">

# MailX

### The Developer Email Infrastructure Platform.

Built from the protocol up in Go.

<p>
  <a href="https://github.com/Ferousco-dev/Mailx">
    <img src="https://img.shields.io/badge/server-MailX-635BFF?style=flat-square" alt="MailX Server">
  </a>
  <a href="./LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-00ADD8?style=flat-square" alt="MIT License">
  </a>
</p>

</div>

---

MailX is email infrastructure for developers — SMTP, REST APIs, delivery pipelines, domain authentication, webhooks, tracking, and SDKs.

Run it yourself or build against the MailX API.

## Repositories

| Repository | Description |
| --- | --- |
| [Mailx](https://github.com/Ferousco-dev/Mailx) | Core MailX server and delivery infrastructure |
| [mailx-go](https://github.com/UseMailx/mailx-go) | Go SDK |
| [mailx-node](https://github.com/UseMailx/mailx-node) | Node.js / TypeScript SDK |
| [mailx-python](https://github.com/UseMailx/mailx-python) | Python SDK |
| [mailx-php](https://github.com/UseMailx/mailx-php) | PHP SDK |
| [mailx-ruby](https://github.com/UseMailx/mailx-ruby) | Ruby SDK |

## Quick Start

```bash
# Go
go get github.com/UseMailx/mailx-go

# Node.js
npm install mailx-sdk

# Python
pip install mailx-sdk

# PHP
composer require mailx/sdk

# Ruby
gem install mailx-sdk
```

## Self-host

MailX is designed to run on your own infrastructure.

```text
MailX
├── Go
├── PostgreSQL
└── Redis
```

No third-party email provider is required to run the core infrastructure.

## Status

MailX is under active development and is not yet production-ready.

## Contributing

Contributions are welcome.

Read the [contributing guide](https://github.com/Ferousco-dev/Mailx/blob/main/CONTRIBUTING.md) or open an issue in the core repository.

---

<div align="center">

**Built for developers who want control over their email infrastructure.**

</div>
