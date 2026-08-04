# Security policy

## Project status

This is an educational portfolio and reference implementation. It is not a production service and must not be connected to customer or employer environments without a separate security review and explicit authorization.

## Data policy

- Use synthetic or public data only.
- Do not submit personal, confidential, regulated, employer, or customer information.
- Do not include real credentials, subscription IDs, tenant IDs, resource identifiers, access tokens, or connection strings in issues, commits, logs, screenshots, traces, or evaluation artifacts.

## Reporting a vulnerability

Do not open a public issue containing exploit details or secrets. Use GitHub private vulnerability reporting when enabled, or contact the repository owner privately through their published GitHub contact method.

Include:

- Affected component and version/commit.
- Reproduction using synthetic data.
- Expected and observed behavior.
- Impact and suggested mitigation.

## Safe testing

- Test only repository-owned local targets or explicitly approved Azure development resources.
- Never target third-party or production systems.
- Replace destructive tools with mocks.
- Apply strict token, cost, tool-call, time, concurrency, and scope limits.
- Stop testing if real secrets or data are encountered.

## Supported versions

Only the current `main` branch is maintained during the portfolio phase.

