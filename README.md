# Full Spectrum Ethics Protocol Stack

[![Validate protocol contracts](https://github.com/blackswan-ai-immunity/full-spectrum-ethics/actions/workflows/validate.yml/badge.svg)](https://github.com/blackswan-ai-immunity/full-spectrum-ethics/actions/workflows/validate.yml)

> An open protocol draft for human-AI governance, agent identity, ethical simulation, risk circuit-breaking, auditability, and civilization-scale interoperability.

中文读者可从 [README.zh-CN.md](./README.zh-CN.md) 开始。English readers may also use [README.en.md](./README.en.md).

---

## Why this exists

AI systems are becoming faster, more autonomous, and more deeply embedded in human organizations. Traditional governance often asks:

> How should AI be regulated?

Full Spectrum asks a wider question:

> When humans, AI agents, organizations, and civilizations all become interacting subjects, how can they continue to share the same game field without erasing freedom, difference, or responsibility?

This repository explores a protocol-level answer.

---

## What Full Spectrum is

Full Spectrum is not a single law, model, product, or ideology.

It is a protocol stack for:

- declaring identity, capability, permission, boundary, and responsibility;
- simulating ethical scenarios before irreversible action;
- recording consent, refusal, risk, escalation, and review;
- allowing disagreement without forcing premature unity;
- triggering downgrade, circuit-break, recovery, or self-deconstruction when a system exceeds its own boundary;
- keeping humans, AI agents, organizations, and civilization-scale systems interoperable.

The core principle is:

> Preserve overall continuity, maximally respect free will, dynamically accommodate differences, and evolve through difference.

---

## What this project is not

This repository does not claim to be:

- a finished global standard;
- a replacement for law, human rights, safety regulation, or institutional governance;
- a spiritual authority;
- a commercial SaaS product;
- proof that any person or group can represent “the whole”.

It is an open protocol draft and engineering exploration.

---

## Relationship to national standards and agent ecosystems

Full Spectrum does not replace national standards, industry standards, A2A, MCP, LangGraph, or other agent interoperability frameworks.

China has released the national standard series **Artificial Intelligence — Agent Interconnection** (AIP, 人工智能 智能体互联), covering agent identity, identity management, capability description, discovery, interaction, and tool invocation. AIP-style standards answer the interconnection-layer question: how agents identify, describe, discover, communicate, and call tools.

Full Spectrum focuses on the governance layer above and around interconnection:

- why an action was allowed;
- who is accountable;
- what risk was detected;
- what cost or responsibility should be recorded;
- when human, guardian, or organizational review is required;
- when an agent should know that it should not act.

In short: AIP/A2A/MCP-style protocols answer “can agents connect and act?” Full Spectrum explores “how should connected agents remain auditable, accountable, and boundary-aware?”

See [Standards and ecosystem mapping](./docs/mapping/standards-mapping.md).

---

## 30-second entry path

- If you only want to call an AI tool, start with [External Node Guide](./EXTERNAL_NODE_GUIDE.md).
- If you operate an existing AI system and want compatibility without full certification, start with [RFC 0005](./rfcs/0005-node-classification-and-external-ethics-profile.md).
- If you need a shared audit envelope across multiple organizations, start with [RFC 0006](./rfcs/0006-cross-enterprise-audit-record.md).
- If you want Full Spectrum certified digital identity for a high-consequence agent, start with [Digital identity declaration](./docs/protocols/Digital_Identity_Declaration.md) and [RFC 0002](./rfcs/0002-identity-and-capability-declaration.md).
- If you want to debate or improve the protocol itself, start with [RFC 0001](./rfcs/0001-full-spectrum-protocol.md).
- If you want to see a business-facing engineering sample, start with [FSHI API Contract Mapping](./docs/mapping/fshi-api-contract-mapping.md).
- If you want to understand cross-enterprise audit interoperability, start with [Cross-Enterprise Audit Record Mapping](./docs/mapping/cross-enterprise-audit-record-mapping.md).

---

## Protocol map

| Layer | Question | Typical artifacts |
| --- | --- | --- |
| Identity | Who or what is acting? | Agent identity, digital identity declaration |
| Capability | What can it do? | Capability declaration, boundary statement |
| Permission | What is it allowed to do now? | Authorization, revocation, consent records |
| Responsibility | Who is accountable? | Audit trace, responsibility path |
| Simulation | What may happen under different conditions? | ESS ethical scenario simulation |
| Risk | When should action be slowed, downgraded, or stopped? | Risk alert, circuit-break, recovery report |
| Guardianship | Who reviews conflict when no single subject can decide? | Guardian network, committee review, distributed review |
| Evolution | How does the protocol change without becoming a new prison? | RFCs, versioning, self-deconstruction rules |

---

## Start here

If you are new, read in this order:

1. [START_HERE.md](./START_HERE.md) — the shortest orientation.
2. [Full Spectrum Protocol Outline v0.1](./docs/protocols/full-spectrum-protocol-outline-v0.1.md) — concise protocol outline.
3. [Glossary](./docs/glossary.md) — key terms for outside readers.
4. [Standards and ecosystem mapping](./docs/mapping/standards-mapping.md) — how Full Spectrum relates to AIP, A2A, MCP, data-governance trends, and AI risk frameworks.
5. [FOR_AGENTS.md](./FOR_AGENTS.md) — machine-readable entry for agents and agent frameworks.
6. [RFC 0001: Full Spectrum Protocol](./rfcs/0001-full-spectrum-protocol.md) — open proposal format for review and iteration.
7. [RFC 0002: Identity and Capability Declaration](./rfcs/0002-identity-and-capability-declaration.md) — first machine-readable protocol objects.
8. [RFC 0003: Audit Trace Schema](./rfcs/0003-audit-trace-schema.md) — responsibility and review trace.
9. [RFC 0004: RiskAlert Schema](./rfcs/0004-risk-alert-schema.md) — shared risk language.
10. [RFC 0005: Node Classification and External Ethics Profile](./rfcs/0005-node-classification-and-external-ethics-profile.md) — compatibility without forced adoption.
11. [RFC 0006: Cross-Enterprise Audit Record Profile](./rfcs/0006-cross-enterprise-audit-record.md) — cross-organization audit envelope.
12. [External Node Guide](./EXTERNAL_NODE_GUIDE.md) — tool, compatible, candidate, and certified node boundaries.
13. [Protocol stack v1.8](./docs/protocols/Full_Spectrum_Agent_Protocol_Stack_v1.8_EN.md) — protocol stack overview.
14. [Guardian community whitepaper](./docs/protocols/Guardian_Community_Whitepaper_Compliant.md) — guardian network and community governance.
15. [Digital identity declaration](./docs/protocols/Digital_Identity_Declaration.md) — identity layer.
16. [FSHI customer-service quality inspection use case](./docs/use-cases/FSHI_Customer_Service_Quality_Inspection.md) — engineering use case.
17. [FSHI API Contract Mapping](./docs/mapping/fshi-api-contract-mapping.md) — maps inspection API fields to RiskAlert and AuditTrace.
18. [Cross-Enterprise Audit Record Mapping](./docs/mapping/cross-enterprise-audit-record-mapping.md) — maps RiskAlert and AuditTrace into a multi-party audit envelope.
19. [FSHI minimal examples](./examples/fshi/) — desensitized dialogue mapped to RiskAlert and AuditTrace.
20. [Validations](./validations/) — planning space for product-facing validation demos and business-value narratives.
21. [ROADMAP.md](./ROADMAP.md) — project roadmap.

---

## Current machine validation

This repository currently validates:

- common mojibake patterns in Markdown, JSON, YAML, HTML, CSS, and script files;
- the FSHI dialogue inspection contract chain:
  `request.sample.json -> response.sample.json -> risk-alert.sample.json -> audit-trace.sample.json -> cross-enterprise-audit-record.example.json`.

The checks run through GitHub Actions on push and pull request to `main`.

---

## Engineering use case: FSHI

FSHI, the Full Spectrum Health Index, is used here as an engineering sample for AI customer-service quality inspection.

Current status: FSHI content in this repository is a concept-validation, API-mapping, and protocol-object demonstration. It is not a full commercial product implementation.

In this repository, FSHI means:

- a protocol use case;
- a minimal open-core reference direction;
- an example of non-invasive, desensitized, multi-turn dialogue risk detection;
- a bridge from Full Spectrum ethics to business engineering.

It does not mean that all company product code or commercial assets must live in this repository.

Recommended boundary:

- `full-spectrum-ethics`: protocol, schemas, examples, public demo, audit format.
- future `fshi-open-core`: minimal runnable open-source kernel.
- company/private repositories: full commercial implementation, customer adapters, deployment assets.

---

## Repository status

This project is currently in early protocol-draft stage.

Current focus:

- repair public entry and encoding issues;
- organize Chinese and English documentation;
- define protocol objects and schemas;
- build minimal verifiable examples;
- distinguish external compatibility from Full Spectrum certification;
- map the protocol to AIP, A2A, MCP, data-governance trends, and AI risk frameworks;
- provide a machine-readable entry for agents and agent frameworks;
- provide minimal FSHI examples that map product concepts into protocol objects without exposing private business data;
- invite review from AI safety, governance, software engineering, ethics, and industry practitioners.

---

## Contributing

Contributions, critiques, translations, schemas, examples, and counterexamples are welcome.

Please read:

- [CONTRIBUTING.md](./CONTRIBUTING.md)
- [GOVERNANCE.md](./GOVERNANCE.md)
- [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md)

---

## Safety note

Do not store tokens, passwords, cookies, private keys, unredacted personal information, or unauthorized enterprise data in this repository.
