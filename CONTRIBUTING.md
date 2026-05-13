# Contributing

Thanks for your interest in contributing to a SebasTN-Rhys project.

## Getting started

1. Fork the repo + clone locally
2. Create a branch: `git checkout -b your-name/short-description`
3. Make your changes; keep commits focused and signed (`git commit -S`)
4. Run tests if the repo has them (`npm test` / `pytest` / etc.)
5. Open a pull request against `main`

## Code style

We use the linters + formatters configured per repo (`npm run lint`, `prettier --write`, etc.). Run them locally before pushing.

## Commit messages

Conventional commits preferred — e.g.:
- `feat(api): add /v2/orgs endpoint`
- `fix(auth): handle expired refresh tokens`
- `chore: bump deps`
- `docs: explain CAA records`

## Reporting bugs

Open a GitHub issue with a clear repro, expected vs. actual behavior, environment details.

## Reporting security vulnerabilities

**Don't open a public issue.** See [SECURITY.md](./SECURITY.md) and email security@sebastn.com.

## Code of conduct

By participating you agree to follow the [Code of Conduct](./CODE_OF_CONDUCT.md).
