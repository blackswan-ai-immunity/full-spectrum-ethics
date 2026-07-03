# Full Spectrum Ethics Protocol Stack

Full Spectrum is an open protocol draft for human-AI governance, agent identity, ethical simulation, risk circuit-breaking, auditability, and civilization-scale interoperability.

Full Spectrum is a bridge protocol, not a forced center. External systems may remain tools, declare compatibility through an External Ethics Profile, or pursue Full Spectrum certification for higher-consequence contexts.

It asks:

> When humans, AI agents, organizations, and civilizations all become interacting subjects, how can they continue to share the same game field?

This repository is the public protocol entry for that exploration.

## Relationship to standards and agent ecosystems

Full Spectrum does not replace national standards, industry standards, A2A, MCP, LangGraph, or other agent interoperability frameworks.

China has released the national standard series **Artificial Intelligence — Agent Interconnection** (AIP, 人工智能 智能体互联), covering agent identity, capability description, discovery, interaction, and tool invocation. AIP-style standards answer the interconnection-layer question: how agents identify, describe, discover, communicate, and call tools.

Full Spectrum focuses on the governance layer above and around interconnection: why an action was allowed, who is accountable, what risk was detected, what cost or responsibility should be recorded, when review is required, and when an agent should know that it should not act.

See [Standards and ecosystem mapping](./docs/mapping/standards-mapping.md).

## 30-second entry path

- If you only want to call an AI tool, start with [External Node Guide](./EXTERNAL_NODE_GUIDE.md).
- If you operate an existing AI system and want compatibility without full certification, start with [RFC 0005](./rfcs/0005-node-classification-and-external-ethics-profile.md).
- If you need a shared audit envelope across multiple organizations, start with [RFC 0006](./rfcs/0006-cross-enterprise-audit-record.md).
- If you want Full Spectrum certified digital identity for a high-consequence agent, start with [Digital identity declaration](./docs/protocols/Digital_Identity_Declaration.md) and [RFC 0002](./rfcs/0002-identity-and-capability-declaration.md).
- If you want to debate or improve the protocol itself, start with [RFC 0001](./rfcs/0001-full-spectrum-protocol.md).
- If you want to see a business-facing engineering sample, start with [FSHI API Contract Mapping](./docs/mapping/fshi-api-contract-mapping.md).
- If you want to understand cross-enterprise audit interoperability, start with [Cross-Enterprise Audit Record Mapping](./docs/mapping/cross-enterprise-audit-record-mapping.md).

## Core principle

> Preserve overall continuity, maximally respect free will, dynamically accommodate differences, and evolve through difference.

## What it contains

- Agent and digital identity declarations.
- Guardian network and review mechanisms.
- Ethical scenario simulation concepts.
- Risk downgrade and circuit-break concepts.
- Full Spectrum Health Index as an engineering use case.
- Public documentation for protocol evolution.

## Start here

1. [START_HERE.md](./START_HERE.md)
2. [Full Spectrum Protocol Outline v0.1](./docs/protocols/full-spectrum-protocol-outline-v0.1.md)
3. [Glossary](./docs/glossary.md)
4. [Standards and ecosystem mapping](./docs/mapping/standards-mapping.md)
5. [FOR_AGENTS.md](./FOR_AGENTS.md)
6. [RFC 0001: Full Spectrum Protocol](./rfcs/0001-full-spectrum-protocol.md)
7. [RFC 0002: Identity and Capability Declaration](./rfcs/0002-identity-and-capability-declaration.md)
8. [RFC 0003: Audit Trace Schema](./rfcs/0003-audit-trace-schema.md)
9. [RFC 0004: RiskAlert Schema](./rfcs/0004-risk-alert-schema.md)
10. [RFC 0005: Node Classification and External Ethics Profile](./rfcs/0005-node-classification-and-external-ethics-profile.md)
11. [RFC 0006: Cross-Enterprise Audit Record Profile](./rfcs/0006-cross-enterprise-audit-record.md)
12. [External Node Guide](./EXTERNAL_NODE_GUIDE.md)
13. [Protocol stack v1.8](./docs/protocols/Full_Spectrum_Agent_Protocol_Stack_v1.8_EN.md)
14. [Guardian community whitepaper](./docs/protocols/Guardian_Community_Whitepaper_Compliant.md)
15. [Cross-Enterprise Audit Record Mapping](./docs/mapping/cross-enterprise-audit-record-mapping.md)
14. [Digital identity declaration](./docs/protocols/Digital_Identity_Declaration.md)
15. [FSHI customer-service quality inspection use case](./docs/use-cases/FSHI_Customer_Service_Quality_Inspection.md)
16. [FSHI API Contract Mapping](./docs/mapping/fshi-api-contract-mapping.md)
17. [FSHI minimal examples](./examples/fshi/)
18. [Validations](./validations/)
19. [ROADMAP.md](./ROADMAP.md)

## Machine validation

The repository validates:

- common mojibake patterns;
- FSHI API contract samples:
  `request.sample.json -> response.sample.json -> risk-alert.sample.json -> audit-trace.sample.json`.

Run locally:

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File .\scripts\check-mojibake.ps1
powershell -NoProfile -ExecutionPolicy Bypass -File .\scripts\validate-fshi-contract.ps1
```

## Status

Early protocol draft. Public review, critique, translation, schema design, and minimal implementation examples are welcome.

Do not store tokens, passwords, cookies, private keys, unredacted personal information, or unauthorized enterprise data in this repository.
