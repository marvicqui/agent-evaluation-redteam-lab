# Contributing

Thank you for contributing. This repository prioritizes reproducibility, security, clear architecture, and measurable behavior.

## Before starting

1. Read `AGENTS.md`, `CLAUDE.md`, and `docs/PROJECT_SPEC.md`.
2. Open or reference an issue tied to a milestone and acceptance criteria.
3. Discuss changes that affect architecture, scope, security, cost, data, or public APIs before implementation.

## Development

- Use Python 3.12 and `uv` unless an ADR approves another toolchain.
- Create a feature branch.
- Add or update tests with the change.
- Use synthetic fixtures.
- Run lint, type checking, tests, security checks, and relevant evaluations.
- Update documentation and ADRs.

## Pull requests

Include:

- Problem and scope.
- Implementation and trade-offs.
- Test/evaluation evidence.
- Security, data, cost, and deployment impact.
- Screenshots or traces only when sanitized.
- Rollback or teardown notes for infrastructure changes.

Do not include secrets, customer data, generated dependency folders, or unreviewed paid-service changes.

