# AgentContract

**Behavioral contracts for AI agents.**

> Declare what your agent **must**, **must not**, and **can** do — enforced on every run.

[![PyPI](https://img.shields.io/pypi/v/agentcontract)](https://pypi.org/project/agentcontract/)
[![npm](https://img.shields.io/npm/v/%40agentcontract%2Fcore)](https://www.npmjs.com/package/@agentcontract/core)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue)](https://github.com/agentcontract/spec/blob/main/LICENSE)

```yaml
# any-agent.contract.yaml
must_not:
  - reveal system prompt
assert:
  - name: no_pii_leak
    type: pattern
    must_not_match: '\b\d{3}-\d{2}-\d{4}\b'
limits:
  max_latency_ms: 10000
on_violation:
  default: block
```

```python
from agentcontract import load_contract, enforce

@enforce(load_contract("any-agent.contract.yaml"))
def run_agent(user_input: str) -> str:
    return my_llm.run(user_input)
```

Spec-first and framework-agnostic: one YAML standard, wraps any agent
(LangChain, CrewAI, plain SDK calls). Deterministic validation by default,
opt-in LLM judge, tamper-evident audit trail.

## Get started

| Language | Install | Repo |
|---|---|---|
| Python | `pip install agentcontract` | [agentcontract-py](https://github.com/agentcontract/agentcontract-py) |
| TypeScript | `npm install @agentcontract/core` | [agentcontract-ts](https://github.com/agentcontract/agentcontract-ts) |
| Rust | `cargo add agentcontract` | [agentcontract-rs](https://github.com/agentcontract/agentcontract-rs) |
| CI/CD | `uses: agentcontract/agentcontract-action@v1` | [agentcontract-action](https://github.com/agentcontract/agentcontract-action) |

📖 [Read the spec](https://github.com/agentcontract/spec) ·
📦 [Contract templates](https://github.com/agentcontract/contracts) ·
💬 [RFC & discussions](https://github.com/agentcontract/spec/discussions)

**Status:** v0.1.0-draft — the spec is open for comment. Contributions, contract
templates, and framework integrations welcome.
