# Investigation Agent Assignment and Evidence-Isolation Protocol 001

**Case:** Epstein public-record investigation  
**Status:** Agent roles defined; this document does not claim that autonomous agents have been launched or that any agent performed research.  
**Repository boundary:** This repository and branch only.

## 1. Operating principle

The Epstein investigation remains the primary, ongoing case investigation. Adding a Bitcoin-origin investigator is an additive assignment—not a change in priority, scope, or direction of the Epstein investigation.

The two investigations proceed concurrently and independently. Neither agent may redirect the other's workload, merge evidence ledgers, or treat a cross-reference as proof of a substantive relationship.

## 2. Investigation agents

### Agent EP-01 — Epstein Main Case Investigator

**Mission:** Continue the broader Epstein investigation across the established case scope, including chronology, people and organizations, legal proceedings, financial records, communications, institutional relationships, and other evidence categories already in the parent investigation.

**Authorized evidence workspace:**
- `research/` — parent-case records, timelines, claims, source registers, financial research, and case findings.
- Existing parent-case evidence IDs and registers.

**Responsibilities:**
- Continue existing work without reducing attention because the Bitcoin workstream exists.
- Maintain the main case timeline and evidence ledger.
- Investigate people and entities in context; distinguish appearance, association, allegation, and proven conduct.
- Refer a Bitcoin-specific artifact to BTC-01 only when it has genuine Bitcoin relevance.
- Preserve parent-case findings and unresolved questions independently.

### Agent BTC-01 — Bitcoin Origin and Ecosystem Investigator

**Mission:** Conduct the Bitcoin-specific workstream, including the independent history and authorship question, Bitcoin's technical origins, early development, developer communications, institutional funding, and Epstein-related cryptocurrency investments or relationships.

**Authorized evidence workspace:**
- `investigations/bitcoin/` — Bitcoin-specific timeline, evidence ledger, questions, source notes, and findings.

**Responsibilities:**
- Investigate Satoshi Nakamoto's identity question independently of assumptions about Epstein.
- Reconstruct the documented technical and historical lineage of Bitcoin.
- Examine the Epstein intersection as a bounded sub-question, not as the presumed explanation for Bitcoin's creation.
- Keep fund-level, entity-level, and personal investments distinct.
- Send only substantiated cross-investigation leads to the link register.

## 3. Independent review roles

The following review functions apply to both investigations. They are separate analytical passes, not claims that additional autonomous agents have been started.

### Review A — Blind Independent Reinvestigation

A second investigator receives the source corpus and a neutral question set, without being given the lead investigator's conclusion. It independently reconstructs the relevant chronology and claims, then records agreements, omissions, and disagreements.

### Review B — Impartial Cross-Examination

A separate review pass tests each material conclusion for:
- unsupported assumptions;
- missing or contradictory source material;
- mistaken identity or entity resolution;
- timeline inconsistencies;
- alternative explanations;
- overstatement of certainty;
- failure to distinguish primary evidence from secondary reporting.

The review must preserve disagreement rather than force consensus.

## 4. Evidence separation and cross-linking

1. Epstein main-case evidence remains in the parent-case registers and `research/` records.
2. Bitcoin-specific evidence remains in `investigations/bitcoin/`.
3. Each workstream maintains its own timeline, evidence ledger, claim status, and unresolved questions.
4. Do not copy a claim into the other workstream as an established fact merely because the same person, company, or source appears in both.
5. A shared source may be referenced by stable evidence ID in both workstreams, but each workstream must independently explain its relevance and limits.
6. Only explicit, source-supported intersections are entered in `research/INTER-INVESTIGATION-LINK-REGISTER-001.md`.
7. A cross-link means “relevant to both inquiries,” not “caused by,” “controlled by,” “coordinated with,” or “proof of wrongdoing.”
8. If a source's relevance is uncertain, retain it in its originating investigation and mark the possible cross-link as unresolved.

## 5. Handoff contract

Every agent or review pass must hand off:
- investigation ID and scope;
- exact source identifier and source locator;
- acquisition and verification status;
- exact page, message ID, timestamp, docket, or record location;
- extracted claim, with quotation kept brief and accurate;
- evidence class (primary, official institutional, judicial, secondary reporting, independent index/OCR, or analysis);
- confidence and limitations;
- contradictory or disconfirming evidence;
- proposed destination file and any cross-link rationale.

No agent may claim that a source was downloaded, hashed, visually inspected, or independently verified unless the corresponding action was actually completed and recorded.

## 6. Authority and safety boundaries

- Public, lawfully accessible sources only.
- No unauthorized access, credential misuse, bypass, or private-data exfiltration.
- Protect victims and witnesses; do not publish identifying or intimate details.
- No agent may expand its own scope or alter the other investigation's evidence classification.
- No conclusion of guilt, authorship, control, intelligence affiliation, or coordination from association or graph proximity alone.
- The human investigator retains final authority over scope, interpretation, and publication.

## 7. Current assignment status

| Role | Scope | Workspace | Status |
|---|---|---|---|
| EP-01 | Main Epstein case | `research/` | Existing investigation continues |
| BTC-01 | Bitcoin origin and Epstein/crypto intersection | `investigations/bitcoin/` | Separate workstream defined |
| Review A | Blind independent reinvestigation | Separate review outputs to be registered | Defined; not launched |
| Review B | Impartial cross-examination | Separate review outputs to be registered | Defined; not launched |

**Important:** This is an assignment and separation protocol. It records how parallel investigation work should be organized; it is not evidence that multiple agents have executed tasks or that the Bitcoin investigation should take precedence over the Epstein main case.
