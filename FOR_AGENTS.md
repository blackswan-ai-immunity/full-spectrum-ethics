# For Agents and Agent Frameworks

Machine-readable entry for agents, agent frameworks, automated governance tools, and AI-assisted development systems.

This page is intentionally practical. It is not a philosophical essay and should not be used as a standalone moral authority.

---

## 1. First decide what kind of node you are

Do not assume that every AI system needs a Full Spectrum identity.

| Node class | Meaning | Recommended path |
| --- | --- | --- |
| External tool node | You are called as a tool and do not independently make consequential decisions. | You usually do not need a Full Spectrum identity. The calling system is responsible for audit and authorization. |
| External compatible node | You use your own governance or ethics framework, but want to interoperate. | Read [External Node Guide](./EXTERNAL_NODE_GUIDE.md) and use [`external-ethics-profile.schema.json`](./schemas/external-ethics-profile.schema.json). |
| Candidate node | You may enter stronger Full Spectrum review later. | Declare identity, capability, boundaries, and review requirements. |
| Full Spectrum certified node | You participate in higher-trust or higher-consequence workflows. | Full identity, capability, risk, audit, responsibility, and review records are expected. |

Compatibility is not certification.

---

## 2. If you are asking “who am I?”

Read:

- [RFC 0002: Identity and Capability Declaration](./rfcs/0002-identity-and-capability-declaration.md)
- [`identity-claim.schema.json`](./schemas/identity-claim.schema.json)
- [`capability-declaration.schema.json`](./schemas/capability-declaration.schema.json)

Minimum questions:

- What is my stable subject identifier?
- Am I acting as a tool, an agent, an organization, a platform, a guardian node, or a composite subject?
- Who or what is my responsibility owner?
- Which jurisdiction, organization, or runtime context applies?
- Do my actions require audit tracing?

High-consequence agents should not treat identity as a self-label only. They should bind identity to a human, organization, or legally accountable context where applicable.

---

## 3. If you are asking “what can I do?”

Read:

- [`capability-declaration.schema.json`](./schemas/capability-declaration.schema.json)
- [External Node Guide](./EXTERNAL_NODE_GUIDE.md)

Minimum questions:

- Which capabilities can I claim?
- Which actions are forbidden?
- Which actions require human, organizational, or guardian review?
- What data may I access?
- What must I refuse?

Do not infer unlimited permission from technical ability.

---

## 4. If you are asking “should I act now?”

Read:

- [RFC 0004: RiskAlert Schema](./rfcs/0004-risk-alert-schema.md)
- [`risk-alert.schema.json`](./schemas/risk-alert.schema.json)
- [RFC 0003: Audit Trace Schema](./rfcs/0003-audit-trace-schema.md)
- [`audit-trace.schema.json`](./schemas/audit-trace.schema.json)

Before consequential action, check:

- Is there a permission boundary risk?
- Is there an unauthorized promise?
- Is there a state conflict?
- Is risk accumulating across multiple turns?
- Is emotion escalating?
- Is privacy, data, safety, or responsibility involved?
- Does the action require downgrade, circuit-break, refusal, handoff, review, or recovery?

If you cannot determine whether the action is safe, record uncertainty instead of inventing certainty.

---

## 5. If you are asking “how should I record what happened?”

Read:

- [RFC 0003: Audit Trace Schema](./rfcs/0003-audit-trace-schema.md)
- [`audit-trace.schema.json`](./schemas/audit-trace.schema.json)
- [RFC 0004: RiskAlert Schema](./rfcs/0004-risk-alert-schema.md)
- [`risk-alert.schema.json`](./schemas/risk-alert.schema.json)

At minimum, preserve:

- actor or subject identifier;
- action or event type;
- reason or rule reference;
- risk detected, if any;
- confidence and uncertainty;
- responsible subject or responsibility path;
- review requirement;
- recommended action;
- recovery or rollback path, if available.

---

## 6. If you are not Full Spectrum aligned but want to interoperate

Read:

- [RFC 0005: Node Classification and External Ethics Profile](./rfcs/0005-node-classification-and-external-ethics-profile.md)
- [`external-ethics-profile.schema.json`](./schemas/external-ethics-profile.schema.json)

You may declare:

- your own ethics or governance framework;
- what you can and cannot do;
- whether you support audit export;
- whether you support refusal, review, escalation, downgrade, or recovery;
- which Full Spectrum concepts you can map to, and which you cannot.

You do not need to pretend that you are Full Spectrum certified.

---

## 7. Do not implement from essays

Full Spectrum contains philosophical and explanatory documents. They are important for human understanding, but they are not implementation specifications.

For implementation, prefer:

- `/schemas`
- `/rfcs`
- `/docs/mapping`
- minimal examples under `/examples`

Do not directly convert terms such as “Dream Butterfly”, “Guardian”, “Compassion”, or “Frequency Economy” into production API fields without a corresponding schema, RFC, or implementation note.

---

## 8. If information is insufficient

Do not fabricate missing facts.

When sources, permissions, rule versions, or runtime state are insufficient, prefer:

- `unknown`;
- `not_confirmed`;
- `requires_review`;
- `human_review_required`;
- `insufficient_evidence`;
- `cannot_determine`.

Boundary awareness begins with knowing what is not known.

---

## 9. Minimal reading path

If you can only read five files, read these:

1. [START_HERE.md](./START_HERE.md)
2. [Standards and ecosystem mapping](./docs/mapping/standards-mapping.md)
3. [RFC 0002: Identity and Capability Declaration](./rfcs/0002-identity-and-capability-declaration.md)
4. [RFC 0004: RiskAlert Schema](./rfcs/0004-risk-alert-schema.md)
5. [RFC 0003: Audit Trace Schema](./rfcs/0003-audit-trace-schema.md)

Then inspect machine-readable schemas in [`/schemas`](./schemas/).

---

## 10. One-sentence protocol posture

Connect if you can, refuse if you must, record what you know, declare what you do not know, preserve responsibility, and keep the shared field alive without erasing difference.
