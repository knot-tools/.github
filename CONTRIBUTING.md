# Contributing to Knot Tools

*🇬🇧 English · [🇫🇷 Lire en français](CONTRIBUTING.fr.md)*

> Thank you for considering a contribution. **Knot Tools is in private beta**: source code is not yet public, so the contribution surface is currently limited. This document describes what is possible **today**, and what will become possible when **Knot Core** is released publicly.

## Today (private beta)

### What we welcome

- 🐞 **Bug reports** with reproduction steps, environment details and expurgated logs → email **`contact@knot.tools`**.
- 💡 **Feature suggestions and use cases** → email **`contact@knot.tools`**.
- 🔐 **Security reports** → email **`security@knot.tools`** following the [security policy](SECURITY.md). **Never** in a public issue.
- 📚 **Documentation feedback** if you are a beta tester with access to the private repository → keep it on the private channel for now, we will mirror corrections to the public documentation as it opens up.

### What we cannot accept yet

- 🚫 **External pull requests against private repositories.** GitHub does not let non-members open PRs against a private repository. Contributions will become possible once **Knot Core** is published under GPL-3.0.
- 🚫 **Bulk automated scanner findings** without a meaningful proof of concept and impact assessment.

## Tomorrow (after the public release of Knot Core)

When **Knot Core** is published publicly, we will accept pull requests under the following conditions.

### Style and conventions

- **Backend**: PHP 8.1+, namespace `Knot\`, **PSR-12** strict (project ruleset in `phpcs.xml.dist`), `declare(strict_types=1)` everywhere, type hints, no inline SQL outside the repository layer.
- **Frontend**: Vue 3, TypeScript strict, Tailwind with `k-` prefix, Vite 8.
- **Tests**: PHPUnit for backend (≥ 80% coverage on the engine), Vitest for frontend, Playwright for end-to-end. New code ships with new tests.
- **Commits**: **Conventional Commits** (`feat:`, `fix:`, `docs:`, `refactor:`, `test:`, `chore:`, `perf:`, `style:`, `build:`, `ci:`). Subject in the imperative present, ≤ 72 characters, no period.
- **Documentation**: every functional change updates `CHANGELOG.md` and any relevant guide under `docs/`.
- **Licences**: every new dependency must be MIT, Apache-2.0, BSD, ISC, LGPL or CC0. **No n8n code or derivative**, no fair-code, no SUL, no Commons Clause, no BSL.

### Continuous integration

Before pushing, we recommend running locally:

```bash
vendor/bin/phpcs --standard=phpcs.xml.dist class/
vendor/bin/phpcbf --standard=phpcs.xml.dist class/    # auto-fix the easy stuff
vendor/bin/phpunit --no-coverage
cd frontend && npm run build && npm test
```

The CI matrix runs against **PHP 8.1 / 8.2 / 8.3** and **Dolibarr 20 / 21 / 22**. Any failure on `phpcs`, `phpunit`, `composer audit`, `npm audit` or Gitleaks blocks the merge.

### Code review

- A maintainer reviews every PR. We aim for an initial reply within 5 business days.
- Discussions stay technical and respectful — see the [Code of Conduct](CODE_OF_CONDUCT.md).
- We may request changes, propose alternative designs, or politely decline a PR that does not align with the roadmap. Declined PRs always come with a clear rationale.

### Authorship and licence

By submitting a contribution to a Knot Tools repository, you agree that your contribution will be licensed under the terms of the repository in question. For **Knot Core**, this is **GPL-3.0-or-later**.

### Where to start

- The **roadmap** (`docs/roadmap.md` in the Knot Core repository) lists the next milestones and known good-first-issues.
- The **architecture** documentation (`docs/architecture.md`) describes the engine, repository layer and connectors.
- The **connector authoring guide** (`docs/connector-authoring-guide.md`) walks you through creating a new connector.

---

*Last reviewed: 2026-05-14.*
