<h3 align="center">PHP 8.3+ API Framework</h3>
<p align="center"><i>Native SOC 2, ISO 27001, NF525 & RGPD compliance built-in</i></p>

<p align="center">
  <img src="https://raw.githubusercontent.com/fennectra/.github/main/profile/fennectra.png" alt="Fennectra" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/fennectra/framework"><img src="https://img.shields.io/badge/PHP-8.3+-8892BF?style=flat-square&logo=php&logoColor=white" alt="PHP 8.3+"></a>
  <a href="https://github.com/fennectra/framework/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="MIT License"></a>
  <a href="https://github.com/fennectra/framework"><img src="https://img.shields.io/badge/Tests-320+-brightgreen?style=flat-square&logo=checkmarx&logoColor=white" alt="Tests"></a>
  <a href="https://packagist.org/packages/fennectra/framework"><img src="https://img.shields.io/badge/Packagist-fennectra-F28D1A?style=flat-square&logo=packagist&logoColor=white" alt="Packagist"></a>
  <a href="https://github.com/fennectra/framework"><img src="https://img.shields.io/badge/FrankenPHP-Ready-00ADD8?style=flat-square&logo=go&logoColor=white" alt="FrankenPHP"></a>
  <img src="https://img.shields.io/badge/OpenAPI-3.0-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white" alt="OpenAPI 3.0">
  <img src="https://img.shields.io/badge/Scalar-API_Docs-FF6B6B?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyTDIgN2wxMCA1IDEwLTV6TTIgMTdsMTAgNSAxMC01TTIgMTJsMTAgNSAxMC01Ii8+PC9zdmc+&logoColor=white" alt="Scalar">
</p>
<p align="center">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis">
  <img src="https://img.shields.io/badge/AWS_S3-232F3E?style=flat-square&logo=amazons3&logoColor=white" alt="AWS S3">
  <img src="https://img.shields.io/badge/GCS-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Google Cloud">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" alt="Kubernetes">
</p>
<p align="center">
  <img src="https://img.shields.io/badge/SOC_2-Compliant-0A66C2?style=flat-square&logo=shield&logoColor=white" alt="SOC 2">
  <img src="https://img.shields.io/badge/ISO_27001-Certified-0A66C2?style=flat-square&logo=shield&logoColor=white" alt="ISO 27001">
  <img src="https://img.shields.io/badge/NF525-Fiscal-0A66C2?style=flat-square&logo=shield&logoColor=white" alt="NF525">
  <img src="https://img.shields.io/badge/RGPD-Privacy-0A66C2?style=flat-square&logo=shield&logoColor=white" alt="RGPD">
  <img src="https://img.shields.io/badge/JWT-Auth-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT">
  <img src="https://img.shields.io/badge/PHPStan-Level_5-4FC08D?style=flat-square&logo=php&logoColor=white" alt="PHPStan">
</p>

---

### Quick Start

```bash
# Install the CLI (once)
composer global require fennectra/installer

# Create a new project
fennectra new my-api
cd my-api
./forge serve
```

<details>
<summary>Alternative: without the installer</summary>

```bash
composer create-project fennectra/skeleton my-api
```
</details>

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
- **OpenAPI 3.0 + Scalar** — Auto-generated API docs from your code
- **Code Generation** — `make:all`, `make:email`, `make:webhook`, `make:audit`
- **Compliance** — NF525, RGPD, SOC 2 audit trails
- **320+ Tests** — Unit + Integration tests, PHPStan level 5, PSR-12

