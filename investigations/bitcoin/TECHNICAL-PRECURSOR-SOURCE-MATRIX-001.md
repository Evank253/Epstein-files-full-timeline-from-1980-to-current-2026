# Bitcoin Technical Precursor Source Matrix 001

**Investigation:** BTC-01 — independent Bitcoin-origin investigation  
**Review date:** 2026-11-17  
**Status:** Public source discovery and comparison design. Original artifacts have not yet been acquired, hashed, or independently reconstructed in this workstream.

## 1. Objective

Build a feature-level technical lineage for Bitcoin without assuming that conceptual influence equals direct authorship, implementation, or identity. Each precursor is analyzed by the problem it addresses and the mechanism it proposes.

## 2. Initial source matrix

| Work | Date / source | Documented mechanism | Important distinction from Bitcoin | Acquisition status |
|---|---|---|---|---|
| Chaumian e-cash | David Chaum, 1982 paper, “Blind Signatures for Untraceable Payments” | Blind signatures enable privacy-preserving digital payment tokens | Issuer/bank-based token issuance and redemption; not a permissionless public proof-of-work ledger | Primary paper source to locate and acquire |
| Hashcash | Adam Back, proposed 1997; consolidated paper dated Aug. 1, 2002 | Computational proof-of-work stamps; cost-function to throttle abuse | Originally anti-spam/denial-of-service cost mechanism, not a complete decentralized currency or consensus protocol | Paper locator found: https://32bitcoin.org/white_papers/hashcash.pdf; primary/author-hosted copy still to be verified |
| b-money | Wei Dai, November 1998 | Two proposed protocols for anonymous digital money, with distributed bookkeeping and computational money creation | Proposal was not implemented as a complete operating public blockchain; exact protocol mechanics require close reading of original text | Source locator: https://www.weidai.com/bmoney.txt (verify availability and earliest archive) |
| Bit Gold | Nick Szabo, December 29, 2005 public essay; concept described earlier | Chain of proof-of-work solutions, timestamping, property/title registry, and distributed verification | Proposal's architecture and trusted timestamp/registry assumptions differ from Bitcoin's operational consensus and UTXO system | Source locator: https://unenumerated.blogspot.com/2005/12/bit-gold.html (original site availability to verify) |
| Reusable Proof of Work (RPOW) | Hal Finney, August 15, 2004 | Hashcash work exchanged for RSA-signed reusable tokens through a server; tokens transferred and reissued | Central trusted server/security model; not Bitcoin's decentralized chain of proof-of-work | Archived original mailing-list message: https://nakamotoinstitute.org/library/rpow/ |
| Bitcoin white paper | Satoshi Nakamoto, announced October 31, 2008 | Peer-to-peer timestamped transaction chain using proof-of-work and longest-chain rule; digital signatures and block rewards | Combines several ideas into a specific network protocol and incentive design | Original announcement copy: https://satoshi.nakamotoinstitute.org/emails/cryptography/1/; verify against original Metzdowd archive and PDF bytes |
| Bitcoin v0.1 | Announced January 8, 2009 at 19:27:40 UTC | Working C++ client, peer-to-peer network, proof-of-work mining, transaction validation, issuance | Software implementation is a separate evidence layer from the paper; code authorship still needs provenance analysis | Mailing-list announcement: https://satoshi.nakamotoinstitute.org/emails/cryptography/16/; archived source mirror is discovery aid only |

## 3. Primary source leads

### Hashcash
Adam Back's 2002 paper explains that Hashcash was originally proposed in May 1997 as a mechanism to throttle systematic abuse of unmetered resources. The proof-of-work token imposes computational cost. This is a key Bitcoin precursor, but its original anti-abuse purpose should not be rewritten as if it were already a decentralized currency.

### b-money
Wei Dai's November 1998 proposal describes an anonymous digital-cash system and explicitly addresses cooperative bookkeeping and money creation. The original proposal must be read in full before assigning precise feature claims. It is a conceptual precursor, not evidence that Dai wrote Bitcoin.

### Bit Gold
Szabo's December 2005 public essay describes scarce digital bits created through costly computation and linked through a timestamped property/title structure. Similarity to Bitcoin's proof-of-work and timestamping is relevant, but differences in implementation and trust assumptions must be mapped rather than glossed over.

### RPOW
Finney's August 15, 2004 announcement describes a Hashcash-based server issuing RSA-signed reusable tokens. This demonstrates a working proof-of-work token experiment before Bitcoin. Its trusted server model is a significant architectural difference.

### Bitcoin paper and release
The October 31, 2008 mailing-list post announces a peer-to-peer electronic cash system, describes Hashcash-style proof-of-work, and links the paper. The January 8, 2009 release announcement says the first software release was available, was Windows-only, included open-source C++ code, and automatically connected to peers. The message's timestamp is January 8, 2009 19:27:40 UTC; date differences in later summaries can result from time zones.

## 4. Feature comparison framework

For each artifact, extract and compare:
1. Digital token representation and ownership.
2. Signature and authorization model.
3. Issuance and scarcity mechanism.
4. Double-spend prevention.
5. Transaction ordering and timestamping.
6. Consensus / agreement among participants.
7. Proof-of-work purpose and validation.
8. Network topology and peer discovery.
9. Incentive and fee structure.
10. Trust assumptions and central points of failure.
11. Privacy / pseudonymity.
12. Operational implementation evidence.

A feature should be marked PRESENT, PARTIAL, ABSENT, or NOT SPECIFIED, with a quotation or exact section/page locator. Do not infer absence solely because a short summary omits a feature.

## 5. Satoshi attribution firewall

These precursor authors are historically relevant because their public work forms part of the documented intellectual lineage. That does not make any of them Satoshi. Likewise, overlap in vocabulary, design concepts, coding style, or technical skill is not identity proof.

The identity inquiry requires separate evidence:
- original communications with reliable message headers;
- contemporaneous source archives and signatures;
- verifiable cryptographic signatures tied to an independently established Satoshi key;
- authenticated repository access and release history;
- corroborated records that connect a pseudonymous account to a real person.

## 6. Acquisition plan

1. Acquire original/author-hosted papers and archived original mailing-list messages where lawful.
2. Record canonical URL, earliest known publication date, retrieval timestamp, content type, byte size, and SHA-256 of bytes actually acquired.
3. Preserve original bytes separately from OCR, HTML extraction, re-hosted copies, and modern annotations.
4. Compare independent archival copies; record differences and provenance rather than selecting a preferred copy silently.
5. Acquire the original Bitcoin white-paper PDF and v0.1 source release from an authoritative or historically well-supported archive; calculate hashes locally.
6. Reconstruct selected protocol features in a controlled analysis environment only after source provenance is established.

## 7. Current conclusion

The public record supports a multi-stage technical lineage: privacy-preserving digital cash, proof-of-work cost functions, distributed money proposals, timestamped scarce digital objects, and reusable proof-of-work tokens. Bitcoin's distinctive contribution was its particular integration into an operational peer-to-peer system with a proof-of-work chain and incentive mechanism. This is a working technical hypothesis to be tested against original artifacts, not a claim that the listed precursor authors collaborated or that any one of them was Satoshi.
