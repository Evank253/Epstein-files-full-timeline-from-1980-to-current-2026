# Bitcoin Precursor Technical Comparison — Primary-Text Findings 001

**Investigation:** BTC-01  
**Review date:** November 17, 2026  
**Status:** Original public mailing-list archive and primary-text transcriptions reviewed online. No source bytes were downloaded locally or SHA-256 hashed in this workstream.

## 1. Evidence hierarchy used

1. Original contemporaneous mailing-list archive (Metzdowd) for Satoshi's October 31, 2008 announcement and January 8, 2009 v0.1 release.
2. Original author text for b-money and Bit Gold where available; the Satoshi Nakamoto Institute and Bitcoin Institute pages are treated as archival/transcription repositories and discovery aids unless their original-host provenance is independently established.
3. Academic publication record for Back's 2002 Hashcash paper.
4. Contemporaneous RPOW announcement text by Hal Finney, preserved by an archival library; original mailing-list source still to be cross-checked.

## 2. Primary-text findings

### BTC-TECH-001 — Hashcash (Adam Back)

**Source:** Adam Back, “Hashcash — A Denial of Service Counter-Measure,” August 2002.  
**Discovery/record:** University of Bologna APICe publication entry, https://apice.unibo.it/bin/view/Publication/HashcashPaper2002

The publication record states Hashcash was originally proposed in May 1997 to throttle systematic abuse of unmetered resources such as email and anonymous remailers. The 2002 paper describes CPU cost-function tokens used as proof-of-work, with interactive and non-interactive variants.

**Technical finding:** Hashcash supplies a reusable proof-of-work concept for imposing computational cost. Its documented original purpose was anti-abuse/denial-of-service countermeasure, not a complete currency, distributed transaction ledger, or consensus protocol.

**Open verification:** Obtain the paper PDF from the publisher/author-hosted location, preserve and hash it, and compare with archival copies. Do not treat the university metadata page as the paper bytes.

### BTC-TECH-002 — b-money (Wei Dai, November 1998)

**Source:** Wei Dai, “b-money,” November 1998. Archival text: https://nakamotoinstitute.org/library/b-money/; author external link shown on the page: https://www.weidai.com/bmoney.txt

The text explicitly proposes two protocols:
- Protocol 1: every participant maintains a separate database of pseudonymous account balances. Money is created through computational solutions; signed broadcasts transfer balances; negative balances are rejected; contracts can reserve collateral and use arbitration (¶¶20–30 of the archival text).
- Protocol 2: account databases are maintained by a subset of participants called servers. Participants verify processing with a randomly selected subset; servers post deposits subject to fines/rewards and periodically publish/commit to databases (¶¶31–34).
- Appendix A discusses an alternative money-creation mechanism based on negotiated supply quotas, bids, and computational work (¶¶35–43).

**Technical finding:** b-money explicitly addresses pseudonymous digital money, computational issuance, signed transfers, replicated or server-maintained balances, and contract enforcement. Its second protocol relies on a subset of servers and a trust/deposit mechanism. The text does not specify Bitcoin's operational proof-of-work chain consensus, block structure, or longest-chain selection mechanism.

**Open verification:** Acquire the author's original text from weidai.com and earliest available archive captures; compare exact content and date.

### BTC-TECH-003 — Bit Gold (Nick Szabo, December 2005)

**Source:** Nick Szabo, “Bit gold,” Unenumerated, dated December 29, 2005 in archival captures. Archival text and original-source locator: https://bitcoin-institute.pages.dev/entries/web-document/nick-szabo/2005-12-29-bit-gold/ and https://unenumerated.blogspot.com/2005/12/bit-gold.html

The text describes:
- costly computational bit strings generated from challenge strings;
- proof-of-work;
- distributed timestamping;
- a distributed property-title registry;
- the latest created string serving as the next challenge;
- ownership verification through an unforgeable chain of title/signatures;
- valuation by checking challenge bits, proof-of-work, and timestamp;
- concern that different computer architectures could produce work at radically different costs.

**Technical finding:** Bit Gold combines proof-of-work, timestamping, linked challenge generation, and a distributed title registry. The described ownership model relies on a chain-of-title registry; it is not identical to Bitcoin's replicated transaction/block ledger and longest-chain consensus.

**Date caution:** The current live blog may display a later date. The archival source notes 2007 captures dated December 29, 2005. Treat that as an archival date attribution and preserve the underlying archive capture before making a stronger provenance claim.

### BTC-TECH-004 — Reusable Proof of Work (Hal Finney, August 15, 2004)

**Source:** Hal Finney, “RPOW — Reusable Proofs of Work,” August 15, 2004. Archival text: https://nakamotoinstitute.org/library/rpow/

Finney describes a system that accepts Hashcash proof-of-work and issues RSA-signed reusable tokens. Tokens can be transferred and exchanged for new RPOW tokens. The server's security model used an IBM 4758 secure cryptographic coprocessor, with signed attestation of the software configuration and source-code comparison.

**Technical finding:** RPOW is a working proof-of-work-backed token system and an important implementation precursor. Its trust model centers on a remote server and tamper-evident hardware/attestation, unlike Bitcoin's peer-to-peer validation and replicated proof-of-work chain.

**Open verification:** Acquire the original August 15, 2004 mailing-list message and original code/documentation from the historical rpow.net archive if lawfully available. The archival library page alone is not a complete source-code acquisition.

### BTC-TECH-005 — Bitcoin white-paper announcement (October 31, 2008)

**Primary source:** Metzdowd Cryptography Mailing List, original archived message:
https://www.metzdowd.com/pipermail/cryptography/2008-October/014810.html

The original archive records the message as posted Friday, October 31, 2008 at 14:10 EDT, by the pseudonymous sender Satoshi Nakamoto. It states:
- the system is peer-to-peer and has no trusted third party;
- double-spending is prevented by a peer-to-peer network;
- there is no mint or other trusted party;
- new coins use Hashcash-style proof-of-work;
- the same proof-of-work powers the network against double-spending;
- transactions are timestamped in an ongoing chain of hash-based proof-of-work;
- nodes may leave and rejoin, accepting the longest proof-of-work chain.

**Technical finding:** This is a contemporaneous public announcement of the integrated Bitcoin design. It explicitly acknowledges Hashcash-style proof-of-work while describing a distinct role for that work: both issuance and securing the transaction-ordering chain.

**Time normalization:** Metzdowd displays 14:10 EDT; the Satoshi Nakamoto Institute transcription displays 18:10 UTC. These are the same instant, not conflicting dates.

### BTC-TECH-006 — Bitcoin v0.1 release announcement (January 8, 2009)

**Primary source:** Metzdowd Cryptography Mailing List, original archived message:
https://www.metzdowd.com/pipermail/cryptography/2009-January/014994.html

The message is dated January 8, 2009 at 14:27:40 EST. It describes a Windows-only first release with open-source C++ code, automatic peer connections, proof-of-work mining, a 21-million-coin issuance schedule with halving every four years, and a 120-block maturity delay for generated coins. It describes sending to an online recipient via IP/public key or to an offline recipient via a Bitcoin address derived from a public key.

**Technical finding:** The release announcement provides evidence that Bitcoin had progressed beyond a paper proposal to runnable software. It documents early implementation choices, but does not by itself establish who authored each source file or who controlled the pseudonymous sender account.

**Time normalization:** Metzdowd's 14:27:40 EST corresponds to 19:27:40 UTC in the Satoshi Nakamoto Institute transcription.

## 3. Feature-level comparison — initial findings

| Feature | Hashcash | b-money | Bit Gold | RPOW | Bitcoin white paper / v0.1 |
|---|---|---|---|---|---|
| Computational proof-of-work | Present | Present in issuance proposal | Present | Present | Present |
| Digital money/token | Not original core purpose | Present | Proposed | Present | Present |
| Signed transfer | Not a currency transfer system | Present | Chain-of-title signatures | Token transfer / reissue | Digital signatures / transactions |
| Double-spend prevention | Not a complete currency mechanism | Balance/ledger protocol | Registry/title-chain model | Server/token redemption model | Peer-to-peer proof-of-work chain |
| Global transaction ordering | Not specified | Not specified as Bitcoin-style chain | Timestamping and linked challenge | Server-mediated token exchange | Timestamped chain |
| Consensus mechanism | Not specified | All participants or selected servers | Distributed services/registry | Trusted server with secure coprocessor | Longest proof-of-work chain |
| Peer-to-peer network | Not required by original anti-abuse use | Anonymous broadcast / server variant | Distributed timestamp/title services | Client-server architecture | Explicit peer-to-peer network |
| Issuance | Work stamp | Computational work / quota auction | Costly bits | Hashcash exchanged for RPOW | Block rewards and scheduled halvings |
| Central trust point | Depends on verifier/challenge context | Protocol 2 has servers | Attempts to distribute trust among services | Attested RPOW server | No mint or central server in stated design |
| Working implementation evidenced by source reviewed | Hashcash system/experiments described | Proposal | Proposal | Working beta server described | v0.1 release announced |

**Classification caution:** “Not specified” means the cited text does not define the feature; it does not prove no related idea existed elsewhere. The table compares the cited versions, not every later extension or historical implementation.

## 4. Technical synthesis — provisional

The documents show a sequence of partially overlapping ideas, not a single already-complete Bitcoin design:
- Hashcash: computational cost as proof-of-work.
- b-money: pseudonymous account-based digital money and computational issuance.
- Bit Gold: scarce proof-of-work objects, timestamping, linked challenges, and title registry.
- RPOW: a functioning reusable proof-of-work token system secured through a trusted, attested server.
- Bitcoin: a peer-to-peer transaction system that integrates proof-of-work into a continuously extended timestamped chain, uses the chain to order transactions and address double-spending, and couples issuance to block production.

This synthesis is a comparison of published designs and release messages. It does not establish direct collaboration, undocumented influence, or the real-world identity of Satoshi Nakamoto.

## 5. Next technical work

1. Acquire and hash the original Hashcash PDF, b-money text, Bit Gold archival capture, RPOW source/documentation, Bitcoin white-paper PDF, and v0.1 source archive.
2. Reproduce the b-money and Bit Gold protocols from their original text in a formal state-machine specification, preserving their different trust models.
3. Extract Bitcoin v0.1 source code and map its transaction validation, block construction, proof-of-work, difficulty adjustment, peer discovery, wallet/key handling, and issuance logic to the white paper.
4. Compare the implementation with the white paper to identify design details omitted from the paper.
5. Only after acquisition, build a provenance graph connecting each source artifact, message, code version, and feature claim.

## 6. Satoshi identity firewall

The technical similarities above are not identity evidence. The source texts do not prove that Back, Dai, Szabo, Finney, or any other precursor author was Satoshi. The inquiry remains open and requires direct, independently corroborated attribution evidence.
