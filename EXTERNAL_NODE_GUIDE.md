# External Node Guide

This guide explains how external tools, compatible systems, candidate nodes, and Full Spectrum certified nodes should be described in this repository.

Full Spectrum is a bridge protocol, not a forced center.

External systems may choose:

- not to adopt Full Spectrum;
- to map their own ethics and audit framework into Full Spectrum objects;
- to become Full Spectrum certified for higher-consequence contexts.

Compatibility is not certification.

---

## 1. Node classes

### 1.1 External Tool Node

An External Tool Node is a tool or model without Full Spectrum digital identity.

Examples:

- text drafting;
- summarization;
- formatting;
- internal brainstorming;
- low-impact classification.

It may be used as a tool, but it must not claim Full Spectrum certification.

If its output is adopted into a consequential workflow, the adopting human, organization, or certified node becomes responsible for that adoption decision.

### 1.2 External Compatible Node

An External Compatible Node does not sign the full Full Spectrum Agent Protocol Stack, but declares its own ethics, audit, risk, and responsibility framework through an External Ethics Profile.

It may interoperate within declared scope.

It must not claim to be a Full Spectrum certified digital identity.

### 1.3 Candidate Node

A Candidate Node is under observation before certification.

It can run in limited low- or medium-consequence contexts while accumulating audit traces and demonstrating capability boundaries.

### 1.4 Full Spectrum Certified Node

A Full Spectrum Certified Node signs or equivalently satisfies the relevant Full Spectrum protocol requirements.

It may be eligible for higher-consequence contexts depending on its authorization, audit, review, and risk-handling strength.

---

## 2. Consequence levels

| Level | Examples | Typical node requirement |
| --- | --- | --- |
| none | private draft, internal brainstorming | external tool |
| low | formatting, non-sensitive classification | external tool or compatible node |
| medium | customer-service risk flag, workflow recommendation | compatible node with AuditTrace |
| high | credit, medical, hiring, procurement, legal, finance | certified node or verified equivalent controls |
| critical | automatic circuit-break, irreversible public impact | strong certification, authorization, review, recovery |

Consequence is not determined only by the immediate action. Downstream adoption matters.

A low-impact generated text can become high-consequence if used in a legal, financial, medical, hiring, or public-facing decision.

---

## 3. External Ethics Profile

External Compatible Nodes should submit an External Ethics Profile.

Minimum contents:

- identity anchor;
- authorization source;
- capability and limitation statement;
- supported consequence levels;
- audit log structure;
- risk classification;
- responsibility or liability assignment;
- data retention and deletion policy;
- equivalency map to Full Spectrum requirements;
- missing items;
- conflict items;
- incompatible clauses;
- conflict resolution rule;
- downgrade, revocation, and recovery path.

Machine-readable schema:

- [`schemas/external-ethics-profile.schema.json`](./schemas/external-ethics-profile.schema.json)

Example:

- [`examples/governance/external-ethics-profile.example.json`](./examples/governance/external-ethics-profile.example.json)

---

## 4. What compatible nodes may say

Allowed:

> This node has submitted an External Ethics Profile for Full Spectrum compatibility mapping.

Allowed:

> This node maps selected audit and risk fields to Full Spectrum AuditTrace and RiskAlert objects.

Not allowed unless certified:

> This node is Full Spectrum certified.

Not allowed unless certified:

> This node has Full Spectrum certified digital identity.

---

## 5. When compatibility is not enough

Compatibility may be insufficient when:

- there is no responsible operator;
- no audit log exists;
- risks are not classified;
- high-consequence actions can be executed without authorization;
- users are denied notice or review in consequential contexts;
- downgrade, revocation, or recovery is impossible;
- the node claims certification without evidence.

High- and critical-consequence contexts may require Full Spectrum certification or verified equivalent controls.

---

## 6. Practical first step

For early adopters:

1. Identify the node class.
2. Declare the highest consequence level it may touch.
3. Fill an External Ethics Profile if not Full Spectrum native.
4. Map audit logs to AuditTrace if possible.
5. Map risk events to RiskAlert if possible.
6. Do not claim certification unless certification requirements are met.

