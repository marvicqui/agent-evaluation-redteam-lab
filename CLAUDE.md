# Claude Code and general LLM implementation guide

This file supplements `AGENTS.md`. It applies to Claude Code and any other LLM agent using repository context.

## Primary objective

Implement the system described in `docs/PROJECT_SPEC.md` as a portfolio-quality, reproducible, low-cost Azure reference implementation. Optimize for evidence, safe operation, architectural clarity, and interview defensibility.

## At the beginning of every session

- Read the current specification and repository instructions.
- Inspect `git status`, recent commits, open work, and test state.
- State the milestone and acceptance evidence you will produce.
- Verify tool availability and authentication rather than assuming it.
- Use official current documentation for SDK, Azure, Microsoft Foundry, Entra, pricing, and security behavior.

## Implementation rules

- Separate deterministic policy/calculation logic from model reasoning.
- Use structured schemas at every model/tool boundary.
- Keep model/provider code behind adapters.
- Include timeouts, retry limits, idempotency behavior, and cost/tool budgets.
- Preserve provenance for inputs, retrieved evidence, decisions, prompts, model versions, tools, and approvals.
- Make unsafe or insufficient-evidence behavior fail closed.
- Build local/mocked behavior first, then integrate paid/cloud services.
- Every feature needs positive, negative, failure, and abuse tests appropriate to its risk.

## Deployment rules

- Do not deploy during exploratory coding.
- Before Azure deployment, produce Bicep build/lint results, `what-if`, RBAC scope, SKUs, expected cost, and teardown target.
- Ask for approval immediately before the state-changing deployment.
- Use the approved personal subscription and the project-specific resource group only.
- Respect the shared monthly Azure budget of USD 30 across the portfolio.
- Stop if the expected cost or permission scope exceeds the approved plan.

## Completion response

Report:

- What now works.
- Files and architecture changed.
- Tests/evaluations executed and results.
- Security and cost implications.
- What is simulated versus deployed.
- Remaining limitations and the next gated step.

Never claim production readiness based only on a successful demo.

