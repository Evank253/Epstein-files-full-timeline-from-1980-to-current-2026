# Three-Track Investigation Directive and Reciprocal Cross-Examination Protocol 001

**Effective:** 2026-11-17  
**Repository receiving all investigation records:** `Evank253/Epstein-files-full-timeline-from-1980-to-current-2026`  
**Branch:** `research/initial-evidence-linked-timeline`

## 1. Purpose

The investigation now consists of three coordinated but separately governed tracks. They may exchange source-backed questions, test results, and gap reports, but they must not merge their original purposes, evidence populations, conclusions, or repositories.

## 2. The three tracks

### EP-01 — Epstein primary investigation
**Location:** `research/`  
**Primary mandate:** Continue the full Epstein public-record investigation, including chronology, people and entities, legal proceedings, financial records, communications, institutions, and documented relationships.

EP-01 remains the primary case investigation and is not displaced by either Bitcoin track.

### BTC-01 — Epstein/Bitcoin connection and Bitcoin creator investigation
**Location:** `investigations/bitcoin/`  
**Mandate A:** Establish Epstein's documented connections to cryptocurrency, Bitcoin organizations, developers, funding, and related financial activity.
**Mandate B:** Independently reconstruct Bitcoin's technical and documentary origins and investigate the identity of Satoshi Nakamoto.

These are two objectives within BTC-01, but their evidence classes remain distinguishable: Epstein-intersection evidence versus general Bitcoin-origin evidence. A historical Bitcoin artifact is not automatically Epstein evidence.

### BTC-RB-01 — Independent Bitcoin reconstruction and block-verification project
**Location:** The user's pre-existing Bitcoin rebuild repository, which is external to this case repository and is **read-only for this investigation**.

**Mandate:** Independently reconstruct Bitcoin source-code behavior, block/header/transaction data, hashes, Merkle structures, SegWit identifiers, validation rules, and reproducible tests. Its existing source files, code, data, branches, commits, and project scope are not to be edited by this Epstein investigation.

BTC-RB-01 may receive source references and gap reports from BTC-01 and EP-01. It may independently challenge BTC-01's Bitcoin technical claims and may supply reproducible technical findings that BTC-01 can use to test historical interpretations. Neither side may silently overwrite the other's records.

**Repository locator status:** Prior conversation records identify a GitHub repository search result named `Evank253/Bitcoin` on branch `Python-3`, but GitHub currently reports that repository as empty. This has not been established as the actual repository containing the user's prior rebuild artifacts. The actual source repository remains to be positively located. No write was made to it. The prior BFBI/TMR/MUT findings below are recorded as prior-work leads pending source-repository reacquisition and independent re-verification.

## 3. Separation and reciprocal exchange

1. EP-01, BTC-01, and BTC-RB-01 each keep their own original purpose, evidence set, chronology, tests, claims, conclusions, and unresolved questions.
2. Cross-examination does not mean evidence migration. It means one track supplies a challenge, reproducibility request, source lead, or discrepancy for the other track to answer in its own record.
3. Every exchange receives a stable cross-review ID and records: originating track, receiving track, source/evidence ID, exact claim tested, test method, result, limitation, and disposition.
4. A BTC-RB-01 result may corroborate a Bitcoin technical fact, expose a gap, or falsify an interpretation. It does not establish Epstein involvement or Satoshi's real-world identity.
5. An EP-01 or BTC-01 discovery may suggest a new test for BTC-RB-01, but no change is made to the rebuild project without the user's separate authorization in that project.
6. BTC-RB-01's code output is not automatically historical source evidence. Record the input block/source, software version, environment, command, output, and reproducibility.
7. Shared references must point to immutable source identifiers, not copy unqualified conclusions.
8. If the tracks disagree, preserve both results and the reason for disagreement. Do not force consensus.
9. EP-01 remains primary in investigative priority. BTC-01 and BTC-RB-01 are additive parallel tracks.
10. Human investigator retains final authority over scope, interpretation, and publication.

## 4. Prior Bitcoin reconstruction findings to cross-examine

These are carried forward from earlier user work and prior conversation records. They are **not newly verified in this repository** and must not be represented as independently re-run in this round.

| Prior-work ID | Previously recorded work | Recorded result / status | Required cross-examination |
|---|---|---|---|
| RB-LEAD-001 | BFBI-001 reconstruction of Bitcoin blocks 975384 and 975386 | Both described as independently acquired/reconstructed with raw-header match and SHA-256d verification; source artifacts and complete run logs must be retrieved from the rebuild project | Re-run from original raw block bytes; compare header serialization, endianness, target, PoW, and block hash |
| RB-LEAD-002 | Block 975386 raw block | Previously recorded size 1,677,602 bytes; block hash `00000000000000000001cb010aa776bc252e5ee418e44fbab795f4b0e46de1c2`; raw SHA-256 `869ef20cb76aab7ae3ca93bc0d75cfe0a5819f1413fc874162153e7f1372cf6b`; nonce 2746705566; nBits `0x1701e5ac`; header and PoW pass previously reported | Reacquire exact bytes, independently recompute SHA-256, parse 80-byte header, decode compact target, verify PoW |
| RB-LEAD-003 | Block 974829 header-builder work | Previously recorded header builder 7/7 and difficulty 8/8; full block was not verified | Preserve limited scope; obtain test vectors and determine what remains unverified |
| RB-LEAD-004 | TMR-001 | Stream parser; raw transactions to TXIDs/WTxIDs and Merkle-root reconstruction | Compare with canonical consensus serialization and independently selected blocks |
| RB-LEAD-005 | MUT-001 | CVE-2012-2459 Merkle-tree mutation shield | Test against original Bitcoin Core behavior and mutation vectors; document exact threat model |
| RB-LEAD-006 | SegWit transaction reconstruction | TXID/WTxID distinctions recorded as part of prior technical work | Reconstruct witness-stripped serialization and witness transaction serialization independently |

No prior result is promoted to verified solely because it appears in this table. Source repository artifacts, test vectors, raw block files, and logs are required.

## 5. Evidence and document standard

Every material finding in EP-01 and BTC-01 must be backed by a document or reproducible primary technical artifact, not only a discovery note or URL.

For documentary evidence, retain:
- original document bytes when lawful and publicly accessible;
- stable source URL and publisher/custodian;
- retrieval timestamp and access conditions;
- filename, media type, byte size, and SHA-256 of the bytes actually acquired;
- document date and relevant page/paragraph/line/footnote;
- exact extraction/transcription linked to the original page;
- redaction/privacy review;
- duplicate relationships and version differences;
- source class and authentication status.

A URL, search snippet, OCR index, news article, or assistant summary is not the original document. If only a locator or secondary report is available, say so explicitly and keep the claim at that evidence level.

For technical evidence, retain raw input bytes, parser/version, environment, command or procedure, expected result, actual result, hash, and independent reproduction.

## 6. Timeline and evidence presentation

- `research/TIMELINE-001.csv` remains the main Epstein chronology.
- `investigations/bitcoin/TIMELINE-001.csv` remains the Bitcoin-specific chronology, with separate Epstein-intersection and Bitcoin-origin events clearly classified.
- BTC-RB-01 technical milestones are recorded in a dedicated read-only cross-examination register in this repository, not by editing the rebuild repository.
- Every timeline event must point to one or more evidence IDs and an exact document locator.
- Each timeline should expose the document link and evidence status so a reader can move from event → claim → evidence ledger → actual source document.
- When a source file has not yet been acquired, the timeline must say `URL_IDENTIFIED_NOT_CAPTURED` or the applicable status; it must not imply the document is attached.

## 7. Repository boundary

All new investigation paperwork, source registers, timeline changes, and cross-review reports are committed only to the authorized Epstein investigation repository and branch above. The pre-existing Bitcoin rebuild repository is not modified. No other engineering repository is modified.

## 8. Current operational status

The three-track structure is now documented. BTC-RB-01 has not been launched as an autonomous agent; it is a defined independent workstream pending exact repository identification and retrieval of its existing artifacts. No source-code changes or data changes are made to that project by this directive.
