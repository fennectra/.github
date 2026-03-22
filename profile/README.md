<p align="center">
  <img src="https://raw.githubusercontent.com/fennectra/.github/main/profile/fennectra.png" alt="Fennectra" width="100%" />
</p>

<h3 align="center">PHP 8.3+ High-Performance MVC API Framework</h3>

<p align="center">
  <a href="https://github.com/fennectra/framework"><img src="https://img.shields.io/badge/PHP-8.3+-8892BF?style=flat-square&logo=php&logoColor=white" alt="PHP 8.3+"></a>
  <a href="https://github.com/fennectra/framework/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="MIT License"></a>
  <a href="https://github.com/fennectra/framework"><img src="https://img.shields.io/badge/Tests-285+-brightgreen?style=flat-square" alt="Tests"></a>
</p>

---

### Quick Start

```bash
composer create-project fennectra/skeleton my-api
cd my-api
php artisan serve
```

### Packages

| Package | Description |
|---------|-------------|
| [`fennectra/framework`](https://github.com/fennectra/framework) | Core framework — ORM, JWT Auth, Queue, Events, Storage, Notifications |
| [`fennectra/skeleton`](https://github.com/fennectra/skeleton) | Application template — ready to `create-project` |
| [`fennectra/installer`](https://github.com/fennectra/installer) | CLI tool — `fennectra new my-app` |

### Features

- **FrankenPHP Worker Mode** — Boot once, serve requests in ~1-2ms
- **Native ORM** — Relations, soft deletes, type casting, eager loading
- **JWT Authentication** — Role-based access control (RBAC)
- **Multi-Database** — PostgreSQL, MySQL, SQLite
- **Queue & Jobs** — Async processing with retry & failure handling
- **Event System** — Sync, Redis, Database brokers
- **Multi-Driver Storage** — Local, AWS S3, Google Cloud Storage
- **Notifications** — Email (SMTP), Slack, Database, Webhooks
- **Email Templates** — Multilingual templates in database
- **Code Generation** — `make:all`, `make:email`, `make:webhook`, `make:audit`
- **Compliance** — NF525, RGPD, SOC 2 audit trails
- **285+ Unit Tests** — PHPStan level 5, PSR-12

