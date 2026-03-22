<h3 align="center">PHP 8.3+ API Framework</h3>
<p align="center"><i>Native SOC 2, ISO 27001, NF525 & GDPR compliance built-in</i></p>

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
  <img src="https://img.shields.io/badge/Scalar-API_Docs-FF6B6B?style=flat-square" alt="Scalar">
</p>
<p align="center">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" alt="Kubernetes">
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

---

### Modules

#### Core

| Module | Description |
|--------|-------------|
| **Router** | Attribute-based routing, groups, middleware pipeline, auto-generated OpenAPI 3.0 docs via Scalar |
| **ORM** | Relations (belongsTo, hasMany, hasOne), eager loading, soft deletes, type casting, pagination |
| **DI Container** | Constructor injection, singletons, autowiring, service resolution |
| **Validator** | DTO validation via PHP 8 attributes: `#[Required]`, `#[Email]`, `#[Min]`, `#[Regex]`... |
| **CLI (Forge)** | 35+ commands organized by theme: scaffolding, database, server, compliance |

#### Security & Authentication

| Module | Command | Description |
|--------|---------|-------------|
| **Auth & RBAC** | `make:auth` | Full auth module: users, roles, permissions, personal access tokens, JWT, registration, password reset |
| **Organizations** | `make:organization` | Multi-org SaaS pattern: teams, invitations, member roles |
| **JWT** | built-in | Access + refresh tokens, configurable TTL, revocation via DB |
| **Encryption** | built-in | AES-256-GCM at rest for sensitive fields |
| **Rate Limiting** | built-in | Redis or in-memory stores, per-route or global |
| **Security Headers** | built-in | HSTS, CSP, X-Frame-Options, X-Content-Type-Options |

#### Compliance (built-in, not a plugin)

| Module | Command | Standard |
|--------|---------|----------|
| **Audit Trail** | `make:audit` | SOC 2 — full action logging, retention policies, immutable records |
| **Security Logging** | built-in | ISO 27001 — account lockout, password policies, security events |
| **Fiscal Certification** | `make:nf525` | NF525 — hash chain integrity, FEC export, period closings |
| **Data Privacy** | `make:rgpd` | GDPR — consent management, DPO dashboard, right to erasure |

#### Communication

| Module | Command | Description |
|--------|---------|-------------|
| **Email Templates** | `make:email` | Multilingual templates in DB, SMTP sending, typed Mailable classes |
| **Notifications** | built-in | Multi-channel: Email (SMTP), Slack, Database, Webhooks |
| **Webhooks** | `make:webhook` | Outbound webhooks with HMAC-SHA256 signatures, async delivery |
| **SSE Broadcasting** | built-in | Server-Sent Events via Redis Pub/Sub |

#### Infrastructure

| Module | Description |
|--------|-------------|
| **Multi-Database** | PostgreSQL, MySQL, SQLite — switch with `DB_DRIVER` |
| **Multi-Tenant** | Database-per-tenant isolation, auto-resolved from domain or port |
| **Queue & Jobs** | Async job processing with retry, failure handling, priority queues |
| **Scheduler** | Cron-like task scheduling, K8s-safe with Redis distributed locks |
| **Storage** | Multi-driver: Local filesystem, AWS S3, Google Cloud Storage |
| **Cache** | Redis, file-based, tagged cache groups, route caching |
| **FrankenPHP Worker** | Boot once, serve requests in ~1-2ms, memory-leak safe |
| **Feature Flags** | Enable/disable features at runtime via Redis |

#### Developer Experience

| Module | Description |
|--------|-------------|
| **Code Generation** | `make:all` generates full CRUD (Model + DTOs + Controller + Routes) in one command |
| **Quality** | `./forge quality` runs PHPStan level 5 + PHP-CS-Fixer + PHPUnit in one shot |
| **Tinker** | `./forge tinker --sql="SELECT * FROM users"` — instant SQL queries |
| **Profiler** | Per-request profiling: SQL queries, timing, memory usage |
| **OpenAPI + Scalar** | API documentation auto-generated from your DTOs and attributes |

---

### Packages

| Package | Description |
|---------|-------------|
| [`fennectra/framework`](https://github.com/fennectra/framework) | Core framework |
| [`fennectra/skeleton`](https://github.com/fennectra/skeleton) | Application template |
| [`fennectra/installer`](https://github.com/fennectra/installer) | CLI installer |
