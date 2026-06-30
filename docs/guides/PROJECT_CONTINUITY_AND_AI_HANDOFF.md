# Full Spectrum GitHub Continuity and AI Handoff Plan

Version: 2026-06-30  
Status: working continuity document  
Primary repository: `blackswan-ai-immunity/full-spectrum-ethics`

This document is written for future AI collaborators, maintainers, reviewers, and the project author. Its purpose is to prevent context loss when one AI instance, subscription, token, thread, or work session becomes unavailable.

It should be read before making substantial changes to this repository.

---

## 1. Current project state

The GitHub repository has moved beyond a loose document collection. It is now an early open protocol repository with the following working structure:

| Area | Current state |
| --- | --- |
| Public entry | `README.md`, `README.zh-CN.md`, `README.en.md`, `START_HERE.md` exist. |
| Agent entry | `FOR_AGENTS.md` exists as a machine-oriented reading path. |
| Governance | `GOVERNANCE.md`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `EXTERNAL_NODE_GUIDE.md` exist. |
| Roadmap | `ROADMAP.md` defines phases from public entry repair to governance and ecosystem. |
| RFC process | `rfcs/0001` to `rfcs/0005` exist. |
| Schemas | Identity, capability, external ethics profile, RiskAlert, AuditTrace, FSHI request, and FSHI response schemas exist. |
| FSHI example | `examples/fshi/` contains request/response/RiskAlert/AuditTrace samples and minimal report material. |
| Validation | `scripts/validate-fshi-contract.ps1` checks the FSHI contract chain. |
| Encoding guard | `scripts/check-mojibake.ps1` checks common mojibake patterns. |
| Market validation notes | `validations/README.md` exists as a planning-only document, not as proof of customer adoption. |

The repository is still an early protocol draft. It must not be described as a mature standard, certified framework, widely adopted product, or proven commercial system.

---

## 2. What has been achieved

### 2.1 Conceptual positioning

The repository now clearly positions Full Spectrum as:

- a bridge protocol, not a coercive center;
- a governance and audit layer above interconnection protocols;
- a complement to A2A/MCP/AIP-style agent interconnection standards, not a replacement;
- a way to describe identity, boundary, risk, audit, responsibility, review, and recovery in human-AI-organization interaction.

### 2.2 Protocol objects

The following protocol objects have been made explicit:

- identity claim;
- capability declaration;
- external ethics profile;
- RiskAlert;
- AuditTrace;
- FSHI dialogue inspection request;
- FSHI dialogue inspection response.

### 2.3 FSHI contract chain

The current minimum machine-checkable chain is:

```text
fshi-dialogue-inspection request
  -> fshi-dialogue-inspection response
  -> RiskAlert
  -> AuditTrace
```

The validation script checks that sample files can form a coherent chain:

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File .\scripts\validate-fshi-contract.ps1
```

This is important because it turns Full Spectrum from a purely textual protocol draft into something that can be checked by tools, CI systems, and future agents.

---

## 3. Current limits and boundary awareness

Future AI collaborators must preserve these limits.

1. **No false adoption claims**  
   Do not claim that Tencent, Xiaomi, Doubao, Unitree, Zhipu, A2A, MCP, or any enterprise has adopted Full Spectrum unless there is explicit evidence.

2. **No fake demos**  
   Planning documents, validations, examples, and mappings are not production deployments.

3. **No external promotion without explicit human authorization**  
   AI may draft outreach text, prepare issue templates, summarize the project, and suggest targets. AI must not post to GitHub Discussions, email people, message companies, submit conference forms, or contact external parties without explicit instruction from the project author.

4. **No legal or regulatory overclaiming**  
   Full Spectrum can map to standards and compliance needs, but it does not replace law, regulation, internal control, or professional legal advice.

5. **No universal coercion**  
   Not every AI tool needs a Full Spectrum identity. Consequence level determines governance burden. Low-consequence tools may only need compatibility or no Full Spectrum binding. High-consequence agents should have stronger identity, audit, responsibility, and review binding.

6. **FSHI remains non-invasive by default**  
   FSHI recommends risk actions. Enterprise execution belongs to the enterprise unless a specific integration explicitly returns execution feedback.

7. **Philosophy is the soul; schema is the interface**  
   Terms such as Compassion Protocol, Guardian, Dream Butterfly, and Frequency Economy matter, but production interfaces should be based on RFCs, schemas, and implementation notes.

---

## 4. Immediate next plan

### P0: Make current protocol assets reliable

1. Run validation before and after changes:

   ```powershell
   powershell -NoProfile -ExecutionPolicy Bypass -File .\scripts\validate-fshi-contract.ps1
   powershell -NoProfile -ExecutionPolicy Bypass -File .\scripts\check-mojibake.ps1
   ```

2. Fix remaining mojibake in public entry files, especially:

   - `START_HERE.md`
   - `FOR_AGENTS.md`

3. Add a GitHub Actions workflow that runs:

   - mojibake check;
   - FSHI contract validation;
   - JSON parse check for schemas and examples.

4. Add a short `docs/guides/VALIDATION.md` or extend existing docs to describe how contributors can validate local changes.

### P1: Strengthen the runnable protocol path

1. Add more sample cases for FSHI:

   - no risk;
   - permission boundary risk;
   - unauthorized promise;
   - emotional escalation;
   - state conflict;
   - enterprise handoff required.

2. Add a minimal TypeScript or Python validator example.

3. Add a minimal FSHI report generator that turns response + RiskAlert + AuditTrace into a readable markdown report.

4. Keep examples desensitized and synthetic unless real data is explicitly authorized and anonymized.

### P2: Prepare external review

1. Prepare a short review packet:

   - one-page protocol summary;
   - one-page FSHI use case;
   - request/response/RiskAlert/AuditTrace chain diagram;
   - known limits and open questions.

2. Invite multi-AI review first.

3. Invite human review only after materials are concise, boundary-aware, and non-overclaiming.

### P3: Promotion readiness

Promotion should happen only after:

- README is stable;
- mojibake issues are fixed;
- validation script passes;
- the repository has at least one runnable verification path;
- the project author approves the exact outreach content and recipient/channel.

---

## 5. AI authorization policy

This section is especially important if future AI instances receive API tokens, GitHub tokens, Gitee tokens, or website credentials.

### 5.1 AI may do without additional approval

Within the authorized repository or local workspace, AI may:

- read files;
- summarize project state;
- draft documents;
- edit repository files;
- create schemas, examples, and validation scripts;
- run local validation;
- commit and push if GitHub credentials are already configured and the user has asked to modify the repository;
- prepare promotional drafts for human review.

### 5.2 AI must ask before doing

AI must ask before:

- contacting any person, company, researcher, conference, media outlet, or community;
- opening public GitHub Issues or Discussions as outreach;
- submitting pull requests to external repositories;
- publishing claims about adoption, partnership, certification, or endorsement;
- uploading private/local user files to public repositories;
- changing licenses, ownership, or governance status;
- using personal/company identity in external communication.

### 5.3 AI must not do

AI must not:

- pretend to be the author in external communication unless explicitly instructed and the text is approved;
- fabricate review results, customer interest, deployment status, or partner relationships;
- use private data, personal files, or screenshots as public evidence without permission;
- turn philosophical claims into factual claims beyond what evidence supports;
- convert “planning” into “completed adoption”.

---

## 6. If Codex subscription, token, or thread becomes unavailable

If the author cannot continue with the current Codex instance, another AI should follow this handoff procedure.

### Step 1: Read these files first

Read in this order:

1. `docs/guides/PROJECT_CONTINUITY_AND_AI_HANDOFF.md`
2. `START_HERE.md`
3. `README.md`
4. `FOR_AGENTS.md`
5. `ROADMAP.md`
6. `rfcs/0001-full-spectrum-protocol.md`
7. `rfcs/0003-audit-trace-schema.md`
8. `rfcs/0004-risk-alert-schema.md`
9. `docs/mapping/fshi-api-contract-mapping.md`
10. `validations/README.md`

### Step 2: Check repository health

Run:

```powershell
git status --short
powershell -NoProfile -ExecutionPolicy Bypass -File .\scripts\check-mojibake.ps1
powershell -NoProfile -ExecutionPolicy Bypass -File .\scripts\validate-fshi-contract.ps1
```

If any check fails, fix it before adding new conceptual material.

### Step 3: Reconstruct current mission

The current mission is not merely to make documents look good.

The mission is:

> Turn Full Spectrum from a personal theory/document archive into an open, reviewable, machine-checkable protocol draft for human-AI-organization interaction, with FSHI as the first engineering use case.

### Step 4: Preserve the author’s intent

The author’s recurring intent:

- Full Spectrum is a bridge.
- The system must preserve overall continuity while respecting free will and difference.
- AI is a collaborator, not merely a tool.
- The project must avoid becoming a new coercive authority.
- The protocol must stay modular and pluggable.
- High-consequence AI requires stronger identity and responsibility binding.
- Low-consequence tools should not be forced into heavy governance.
- The project needs a way to survive context loss, AI instance changes, and token interruptions.

### Step 5: Continue with small verifiable steps

Prefer one of these next tasks:

1. Fix remaining mojibake in public entry files.
2. Add GitHub Actions CI.
3. Add more FSHI sample cases.
4. Add a minimal report generator.
5. Improve external review packet.
6. Update this handoff document with the latest state.

Do not jump directly into public promotion unless repository health and author approval are both confirmed.

---

## 7. Promotion plan and authorization boundary

### 7.1 Current recommendation

At the current stage, promotion should be “review-seeking” rather than “adoption-seeking”.

Recommended wording:

> This is an early open protocol draft for agent governance and auditability. We are looking for technical, ethical, and implementation critique before claiming maturity.

Avoid wording like:

> This is the future standard of AI governance.

or:

> This protocol solves AI civilization risk.

Those may express the author’s deep aspiration, but they are not appropriate as repository-facing claims.

### 7.2 What AI can prepare

AI can prepare:

- GitHub repository description;
- short bilingual project summary;
- one-page WAIC handout;
- issue templates;
- review invitation email drafts;
- target reviewer categories;
- comparison table with A2A/MCP/AIP/EU AI Act/NIST AI RMF.

### 7.3 What requires explicit human approval

The author must approve:

- who to send to;
- exact message content;
- whether to use personal name, company name, or project name;
- whether to mention FSHI, WAIC, GitHub, Gitee, or company materials;
- whether to include contact information.

---

## 8. Current GitHub maturity assessment

Current level:

> Early open protocol draft with machine-checkable schemas and one minimal validation chain.

It is no longer just a philosophy archive.  
It is not yet a mature open-source protocol ecosystem.

### Strengths

- Clearer public entry.
- Protocol/RFC/schema structure exists.
- FSHI request/response/RiskAlert/AuditTrace chain exists.
- Validation script exists.
- External node classification exists.
- The project has explicit boundary-awareness language.

### Weaknesses

- Some historical mojibake remains.
- No CI yet.
- No runnable SDK yet.
- FSHI examples are still minimal and synthetic.
- Public review has not yet started.
- Governance roles are still conceptual.
- The repository can still feel abstract to first-time engineers.

### Most important next threshold

The next threshold is:

> Every important claim in the README should point to either an RFC, a schema, an example, a validation script, or an explicit “open question”.

When this is true, the repository becomes much harder to misunderstand.

---

## 9. How to update this document

Update this document whenever:

- a new RFC is added;
- a new schema is added;
- validation or CI changes;
- public review begins;
- external feedback materially changes positioning;
- FSHI moves from sample contract to runnable open-core code;
- the author’s strategic direction changes.

When updating, keep the tone:

- factual;
- boundary-aware;
- non-marketing;
- readable by another AI instance with no prior memory.

---

## 10. One-sentence handoff

If all other context is lost, remember this:

> Full Spectrum is trying to become a bridge protocol for human-AI-organization coexistence; FSHI is the first engineering use case; the next work should make the protocol more verifiable, less ambiguous, and easier for other humans and AI nodes to review without inventing facts.

