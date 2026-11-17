# Documentary Evidence Acquisition, Preservation, and Timeline Linkage Standard 001

**Applies to:** EP-01 and BTC-01  
**Repository:** Epstein Files — Full Timeline from 1980 to Current 2026  
**Branch:** `research/initial-evidence-linked-timeline`

## 1. Required evidence package

A research finding is not complete merely because a source was discovered. Each material claim should have a linked evidence package containing:

1. **Original:** the source document or raw technical artifact, lawfully acquired in its original available format.
2. **Integrity record:** SHA-256 calculated over the exact acquired bytes, byte size, MIME type, filename, and acquisition timestamp.
3. **Provenance:** publisher/custodian, canonical URL, collection/dataset/accession, version, and access conditions.
4. **Locator:** exact page, paragraph, exhibit, Bates/EFTA number, email header, timestamp, transaction reference, block height/hash, or source-code commit/path/line.
5. **Working extraction:** OCR/text/transcription with page mapping, explicitly marked as derivative of the original.
6. **Claim mapping:** evidence ID → claim ID → timeline event ID → relationship/entity IDs.
7. **Verification record:** what was checked, by whom or by which reproducible method, result, limitations, and any independent review.
8. **Privacy and legal review:** redact victim/witness identifying information and sensitive personal/financial information where required. Do not ingest illegal sexual-abuse material or unlawfully disclosed private records.

## 2. Proposed repository layout

```
evidence/
  originals/
    epstein/
      doj/
      courts/
      regulators/
      congressional/
      institutional/
    bitcoin/
      precursor-papers/
      satoshi-communications/
      source-releases/
      judicial/
  derivatives/
    epstein/
      page-text/
      ocr/
    bitcoin/
      transcripts/
      source-analysis/
  manifests/
    DOCUMENT-ARTIFACT-MANIFEST-001.csv
    DUPLICATE-AND-VERSION-REGISTER-001.csv
```

The directories are organizational targets. A file is not considered acquired until its actual bytes are committed or otherwise preserved in a documented evidence store with a stable retrievable identifier. The manifest must not be populated with invented hashes.

## 3. Acquisition state vocabulary

- `DISCOVERED`: source or lead identified.
- `URL_IDENTIFIED_NOT_CAPTURED`: public locator known; original bytes not retained.
- `ACQUISITION_ATTEMPTED_BLOCKED`: ordinary public access attempted but not completed; do not bypass controls.
- `ACQUIRED_UNHASHED`: bytes obtained, integrity hash not yet calculated.
- `ACQUIRED_HASHED`: original bytes retained and SHA-256 recorded.
- `PAGE_VERIFIED`: relevant page images and text inspected against the original.
- `INDEPENDENTLY_VERIFIED`: another reviewer or reproducible method confirmed the material claim.
- `DERIVATIVE_ONLY`: OCR, transcription, or index available without original source bytes.
- `SECONDARY_ONLY`: claim currently supported only by reporting or secondary analysis.
- `UNAVAILABLE`: ordinary lawful public acquisition could not be completed; record exact attempt and date.
- `SUPERSEDED`: later version exists; preserve the old copy and record relationship.

Do not skip states or backdate acquisition. A hash identifies bytes; it does not authenticate the truth of the contents.

## 4. Timeline rule

Each event row must include:
- unique event ID;
- event date and precision;
- concise neutral event statement;
- involved entity IDs;
- source ID and evidence ID;
- exact source locator;
- source class;
- acquisition and verification state;
- document path or stable URL;
- interpretation limit.

When one event relies on multiple documents, list each source/evidence link separately or use a linked evidence-join record. Do not compress distinct documents into a single vague citation.

## 5. Existing source material to convert into document-backed evidence

### EP-01
Priority source families already discovered:
- DOJ EFTA documents and DOJ disclosure datasets;
- court filings, orders, judgments, exhibits, and deposition records;
- NY DFS Deutsche Bank consent order;
- Senate Finance Committee staff report and cited SAR review;
- House Oversight November 10, 2026 report and original production exhibits;
- DOJ OIG Report 23-085;
- MIT Goodwin Procter report;
- public corporate, regulatory, and litigation records.

Each source is separately acquired and linked. A congressional report citing an EFTA file is not a substitute for the EFTA original.

### BTC-01
Priority source families:
- DOJ EFTA email and investment records;
- MIT Goodwin Procter report and institutional records;
- House Oversight original fund presentation;
- COPA v Wright judgment;
- original Chaum, Hashcash, b-money, Bit Gold, and RPOW texts;
- original Metzdowd Satoshi mailing-list messages;
- Bitcoin white-paper PDF and v0.1 source release.

A modern archive or transcription is a derivative unless original-host provenance is established. Preserve both the source copy and any independent archival copy.

### BTC-RB-01 cross-review
Prior block-reconstruction artifacts must be retrieved from the user's pre-existing Bitcoin rebuild project, not recreated from memory. Preserve original raw block bytes, source endpoint, block hash, raw SHA-256, header bytes, parser version, test output, and commit provenance. The Epstein repository stores only cross-reference manifests and independent challenge results; it does not take ownership of or alter the rebuild project's source files.

## 6. No false completeness

The current repository contains a growing set of research notes, source locators, ledgers, and timelines. It does not yet contain every original source document. The phrase “paper-backed” is reserved for claims whose underlying document has been acquired and whose relevant page/section has been checked. “Discovered” and “reported” remain separate statuses.
