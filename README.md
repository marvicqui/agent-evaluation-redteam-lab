# Agent Evaluation & Red Team Lab

A provider-neutral evaluation and adversarial-testing harness for models, RAG systems, and tool-using agents. It produces versioned scorecards and CI gates across quality, grounding, authorization, tool behavior, safety, latency, and cost.

## Status

**Specification phase.** Red teaming is restricted to local reference targets or explicitly approved development endpoints.

## Planned capabilities

- Versioned quality, RAG, trajectory, and security datasets.
- Deterministic and calibrated model-based evaluators.
- Vulnerable/patched local RAG and tool-agent pairs.
- Attack Success Rate and critical-failure reporting.
- Baseline/candidate comparison and machine-readable release gates.
- Strict per-run target, token, cost, time, and concurrency limits.
- Adapters for the other portfolio projects and optional Microsoft Foundry evaluation.

## Start here

1. Read [AGENTS.md](./AGENTS.md) and [CLAUDE.md](./CLAUDE.md).
2. Read the complete [project specification](./docs/PROJECT_SPEC.md).
3. Implement the deterministic local harness and safety guard before any remote tests.

## Safety

Never test third-party or production systems. Destructive tools must be mocks, and all datasets must be synthetic and safe to publish.

## License

MIT. See [LICENSE](./LICENSE).
Provider-neutral evaluation and red-team harness for RAG and tool-using agents
