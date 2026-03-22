# Contributing to Fennectra

Thank you for considering contributing to Fennectra! This guide will help you get started.

## Code of Conduct

By participating, you agree to maintain a respectful and inclusive environment for everyone.

## How to Contribute

### Reporting Bugs

1. Check if the issue already exists in [Issues](https://github.com/fennectra/framework/issues)
2. Create a new issue with:
   - Clear title describing the bug
   - Steps to reproduce
   - Expected vs actual behavior
   - PHP version, OS, database driver

### Suggesting Features

Open an issue with the `enhancement` label. Describe:
- The problem you're trying to solve
- Your proposed solution
- Any alternatives you've considered

### Submitting Code

#### Setup

```bash
# Fork the repository, then:
git clone https://github.com/YOUR_USERNAME/framework.git
cd framework
composer install
```

#### Development Workflow

1. **Create a branch** from `main`:
   ```bash
   git checkout -b feature/my-feature
   # or
   git checkout -b fix/bug-description
   ```

2. **Write your code** following our conventions (see below)

3. **Run the quality checks** — your PR will not be merged if these fail:
   ```bash
   composer test       # PHPUnit tests must pass
   composer analyse    # PHPStan level 5, zero errors
   composer lint       # PSR-12 code style
   ```

4. **Write tests** for your changes:
   - Bug fix? Add a test that reproduces the bug
   - New feature? Add unit tests + integration tests if applicable
   - Place unit tests in `tests/Unit/`, integration tests in `tests/Integration/`

5. **Commit** with a clear message:
   ```bash
   git commit -m "Add: user email verification flow"
   git commit -m "Fix: Model belongsTo returns wrong table on multiple models"
   ```

6. **Push and create a Pull Request**:
   ```bash
   git push origin feature/my-feature
   ```
   Then open a PR on GitHub against `main`.

#### Commit Message Format

```
<type>: <description>

Types:
  Add      New feature or capability
  Fix      Bug fix
  Refactor Code restructuring (no behavior change)
  Docs     Documentation only
  Test     Adding or updating tests
  Perf     Performance improvement
```

### Code Conventions

- **PHP 8.2+** — Use typed properties, readonly classes, enums, named arguments
- **PSR-12** — Code style enforced by PHP-CS-Fixer
- **PSR-4** — Autoloading via Composer
- **No magic** — Explicit over implicit. Avoid `__call`, prefer typed methods
- **Framework namespace** — `Fennec\` for all framework code
- **App namespace** — `App\` for application code (skeleton)

### What Makes a Good PR

- **One concern per PR** — Don't mix a bug fix with a refactor
- **Tests included** — No PR without tests (unless it's docs-only)
- **Quality passes** — `composer test && composer analyse && composer lint`
- **Clear description** — What, why, and how to test it
- **Small and focused** — Easier to review, faster to merge

### What We Will NOT Merge

- PRs that break existing tests
- Code without tests
- Changes that don't pass PHPStan level 5
- Features without discussion in an issue first
- Code that introduces external dependencies without justification

## Architecture Overview

```
framework/
├── src/
│   ├── Attributes/     # PHP 8 attributes (#[Required], #[Table], etc.)
│   ├── Commands/       # CLI commands (make:*, migrate, serve, etc.)
│   ├── Controllers/    # Framework-provided controllers (Docs, SSE)
│   ├── Core/           # Core classes (App, Router, Model, Database, etc.)
│   └── Middleware/      # HTTP middleware (CORS, Auth, RateLimit, etc.)
├── config/             # PHPStan, PHPUnit, CS-Fixer configs
├── database/           # Base migrations and seeders
├── tests/              # Unit and integration tests
└── bin/cli             # CLI entry point
```

## Questions?

Open a [Discussion](https://github.com/orgs/fennectra/discussions) or an issue. We're happy to help!
