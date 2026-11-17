# Bitcoin Origin Chronology and Source Verification 001

**Investigation:** BTC-01 — independent Bitcoin-origin and ecosystem investigation  
**Source reviewed:** *Crypto Open Patent Alliance v Wright* [2024] EWHC 1198 (Ch), approved judgment dated May 20, 2024  
**Review date:** November 17, 2026  
**Status:** Official judgment located and web text reviewed; PDF bytes not locally acquired or hashed in this workstream.

Official judgment PDF: https://www.judiciary.uk/wp-content/uploads/2024/05/COPA-v-Wright-Judgment.pdf

## 1. Purpose and limits

This chronology records the judgment's agreed/uncontroversial Bitcoin history section, especially paragraphs 22–24. It is a judicial record and an authoritative source for what the court recorded in this proceeding. It is not a complete technical history of Bitcoin and does not independently authenticate every original email, repository artifact, or network event cited in the judgment.

The judgment's identity findings concern Craig Wright. They exclude Wright as Satoshi on the balance of probabilities applied in the case; they do not identify the actual person or persons behind the Satoshi pseudonym.

## 2. Precursor systems — paragraph 22

Paragraph 22.1 describes a lineage of digital-cash and proof-of-work concepts:
- David Chaum's early-1980s token-currency work;
- E-Gold, associated in the judgment with Dr Jackson and Mr Downey;
- Bit Gold, associated with Nick Szabo;
- B-Money, associated with Wei Dai;
- Hashcash, associated with Adam Back.

The judgment specifically notes Hashcash's proof-of-work algorithm. These are intellectual and technical precursors, not proof that any one precursor author created Bitcoin or that any one person was Satoshi.

**Research requirement:** Independently acquire the original papers/specifications and compare the precise mechanisms: issuer/trust model, minting, transfer, double-spend prevention, timestamping, proof-of-work, identity, and ledger architecture. Record both similarities and material differences.

## 3. Satoshi-era chronology — paragraph 23

| Date | Judgment paragraph | Recorded event | Verification status / limitation |
|---|---:|---|---|
| August 2008 | 23.1 | Satoshi acquired bitcoin.org domain | Judgment chronology; registrar/WHOIS historical record not separately acquired here |
| August 20, 2008 | 23.2 | Satoshi emailed Adam Back with a draft white paper and asked about a Hashcash reference | Judgment says the email was not previously published before proceedings; acquire disclosed original and forensic metadata |
| August 21, 2008 | 23.2 | Back replied and directed Satoshi to Wei Dai's B-Money paper | Acquire original correspondence and compare headers/thread context |
| August 22, 2008 | 23.2 | Satoshi contacted Wei Dai to check the B-Money reference | Judgment notes these Satoshi/Wei Dai emails had been published before proceedings; locate earliest source copy |
| October 5, 2008 | 23.3 | Satoshi registered the nakamoto2 SourceForge account and created the Bitcoin project | Acquire archived SourceForge project metadata and earliest available repository records |
| October 31, 2008 | 23.4 | White paper announced on the Metzdowd cryptography mailing list | Compare original mailing-list post, message headers, white paper bytes, and contemporaneous replies |
| December 8/9, 2008 | 23.5 | White paper uploaded to SourceForge | Verify archived project release and file hashes |
| January 3/4, 2009 | 23.6 | Genesis block created (date depends on time zone) | Independently reconstruct block 0 header, coinbase, hash, timestamp, and embedded headline |
| January 8, 2009 | 23.7 | Bitcoin software and source code uploaded; release announced | Acquire original v0.1 release archive and calculate hashes |
| January 9, 2009 | 23.8 | Block 1 mined | Verify block header and chain linkage from primary chain data |
| January 12, 2009 | 23.8 | First transaction recorded in block 170: 10 BTC from Satoshi to Hal Finney, mined from block 9 | Verify transaction/block data; attribution to Satoshi and Finney depends on contemporaneous evidence, not chain data alone |
| March 24, 2009 | 23.9 | Further white-paper version uploaded | Compare file versions and metadata |
| May 2, 2009 | 23.10 | Satoshi asked Martti Malmi to create an FAQ; Malmi later helped establish project forums | Acquire original correspondence and forum records |
| Around April 2011 | 23.11 | Satoshi delegated lead core developer responsibility to Gavin Andresen | Acquire original messages and project history |
| April 26, 2011 | 23.11 | Satoshi transferred the network alert key file to Andresen | Seek original message/artifact and independently verify provenance |

## 4. Identity issue — what the judgment establishes

At paragraph 7, the court declared that Wright:
1. was not the author of the Bitcoin white paper;
2. was not the person who adopted or operated under the Satoshi Nakamoto pseudonym between 2008 and 2011;
3. did not create the Bitcoin system; and
4. was not the author of the initial Bitcoin software versions.

**Correct inference:** Wright is excluded by the judgment's findings.  
**Incorrect inference:** The judgment identifies Satoshi or proves any alternative candidate's identity.

The judgment also distinguishes the evidence used to assess Wright's claim from the agreed historical chronology. BTC-01 must preserve that distinction.

## 5. Independent verification plan

### A. Original communications
- Acquire the 20–22 August 2008 Adam Back and Wei Dai correspondence from the earliest reliable source.
- Acquire the October 31, 2008 Metzdowd announcement and surrounding thread.
- Acquire November 2008 source-sharing correspondence and compare all recipients, attachments, message IDs, and timestamps.
- Acquire 2009–2011 communications with Hal Finney, Martti Malmi, Gavin Andresen, and other early participants.
- Preserve raw headers and original attachments when lawfully available; distinguish original mailbox exports from later compilations.

### B. Code and repository history
- Preserve the earliest available Bitcoin source archive and SourceForge release metadata.
- Compare source code, timestamps, build artifacts, and release hashes across versions.
- Reconstruct early commits/patches and identify which changes are attributable to which account, while treating account attribution as a separate question from real-world identity.
- Analyze design decisions and code evolution without assuming that writing a component proves authorship of the entire system.

### C. Technical lineage
Build a feature-level comparison across Chaumian e-cash, Hashcash, B-Money, Bit Gold, RPOW, and Bitcoin. At minimum compare:
- trust and issuer model;
- transaction validation;
- double-spend prevention;
- timestamping and ordering;
- proof-of-work role;
- difficulty adjustment;
- incentives and issuance;
- peer discovery and network propagation;
- script/programmability;
- key ownership and signature model.

### D. Candidate attribution standard
Do not name a living person as Satoshi based on writing style, time zone, technical ability, ideology, access, employment, or association. A serious attribution requires direct, independently corroborated evidence such as a valid signature from a key reliably tied to Satoshi, authenticated contemporaneous records, or equivalent proof with robust chain of custody.

## 6. Epstein intersection firewall

This origin chronology is independent of Epstein-related investment and institutional records. Epstein's later association with MIT DCI, Coinbase, Blockstream, or individual developers cannot be used to infer authorship, early access, control, or involvement in Bitcoin's 2008 creation. Such a connection would require direct contemporaneous evidence and must be separately recorded in the Bitcoin/Epstein intersection track.

## 7. Acquisition status

| Source | Status |
|---|---|
| COPA v Wright official judgment | Official PDF located; text reviewed; local bytes/hash and visual page review pending |
| Adam Back correspondence | Judgment locator/date identified; original not acquired here |
| Wei Dai correspondence | Judgment locator/date identified; original not acquired here |
| Metzdowd announcement | Date and forum identified; original not acquired here |
| SourceForge project and v0.1 | Judgment chronology identified; original archive not acquired here |
| Genesis block / early chain | Public chain data independently reconstructible; no new reconstruction performed in this note |
| Satoshi identity | Unresolved; no candidate attribution made |

**Working conclusion:** The judgment provides a strong, paragraph-cited chronological framework and excludes one prominent false claimant. It does not resolve Satoshi's real-world identity. The next phase should move from secondary chronology to original communications, source archives, and reproducible technical artifacts.
