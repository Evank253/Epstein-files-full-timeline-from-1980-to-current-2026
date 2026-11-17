# Independent corpus API audit and targeted source verification — 001

**Review date:** 2026-11-17  
**Destination:** This Epstein investigation repository only  
**Source class:** Independent third-party index and OCR/transcription mirror; not DOJ-authored  
**Status:** Discovery and cross-check only. No original DOJ bytes acquired or hashed in this review.

## 1. REST API independently inspected

The independent Epstein Files Research Database publishes:
- API discovery document: https://epstein-data.com/api/corpus/
- Agent instructions: https://epstein-data.com/llms.txt
- OpenAPI specification: https://epstein-data.com/api/corpus/openapi
- Full-text corpus: https://epstein-data.com/full_text_corpus
- Human-readable EFTA viewer pattern: https://epstein-data.com/EFTA00701362
- PDF mirror pattern: https://epstein-data.com/pdf/EFTA02634615.pdf

The API discovery document states that read-only search/retrieval endpoints are public, require no API key, and return JSON. The documented API includes:
- `GET /search?q=...` — full-text page search, AND/OR/NOT and quoted phrases.
- `GET /document?id=EFTA...` or path form `/document/EFTA...` — document text; optional zero-indexed page.
- `GET /metadata?id=EFTA...` — document metadata.
- `GET /count?q=...` — counts.
- `GET /emails?... ` — parsed email metadata.
- `GET /transcripts?q=...` and `/handwriting?q=...` — transcribed media and handwriting.
- `GET /entities?q=...` — independent knowledge graph.
- `GET /related?id=...` — related/near-duplicate/thread candidates.
- `GET /cross-refs?id=...` — alternate Bates/production numbers.
- `GET /dossier?id=...` — combined document package.
- `GET /document-type?id=...` — AI-classified page types.

The API's own guidance says to use API endpoints to read documents and use the human viewer URL only as a citation destination. It warns that query strings may be stripped by some clients and provides path-based alternatives. It also documents a 15-second limit for the Datasette SQL API.

## 2. Corpus totals are not stable and do not equal DOJ-only unique file count

The independent site's own pages and documentation show several different snapshots:
- Homepage/full-text page: 1,425,565 document records and 2,923,763 pages.
- API discovery JSON: 1,416,831 documents and 2,915,593 pages.
- OpenAPI description: 1,416,848 documents and 2,915,593 pages.
- The full-text page explicitly says the corpus includes all 12 DOJ datasets **plus House Oversight estate documents and FBI Vault files**.
- The database includes multiple source prefixes (EFTA, HOUSE_OVERSIGHT, FBI_VAULT and DOJ-OGR), so its aggregate document count is not a DOJ-EFTA-only count.

These are inconsistent snapshots/schema counts, not evidence of multiple DOJ productions. They must be recorded with retrieval date, endpoint and source scope. Never use the headline count as a verified number of unique DOJ original files.

The independent source's own instructions also warn:
- Extraction/search metadata is incomplete for many fields.
- Filename and attachment linkage are populated only for narrow subsets.
- Absence of metadata is not proof that a record is absent.
- OCR may contain errors; transcript material is appended to page text under a transcript delimiter and must be distinguished from verbatim page OCR.
- Its analytical reports are AI-generated and may contain errors.
- Its published license is CC BY-NC-SA 4.0; observe its noncommercial/share-alike terms when using or redistributing its derived material.

## 3. Targeted cross-check: EFTA02634615 — Carbyne warrants

A full-text PDF mirror was opened and inspected as a secondary text rendering:
https://epstein-data.com/pdf/EFTA02634615.pdf

The rendered text shows:
- Page 1 (zero-indexed page 0 in API convention): an email dated March 14, 2019, from Jeffrey Epstein to Darren Indyke, subject “Re: Carbyne warrants,” replying “Yes” to Indyke's question whether he could confirm Epstein as the controlling person of Southern Trust Company.
- The same page includes Indyke's March 12 question about whether Epstein's name should be associated with the investment, and his statement that the transferring bank was Deutsche Bank.
- Later pages reproduce Tomer Toor's March 11, 2019 email stating that the requested $3.6 million had been received in Ergo's account and that the bank was requesting controlling-person information and recommendation letters for anti-money-laundering review.
- A March 7 email reproduced in the chain states that Southern Trust had signed an additional investment agreement and transferred its $2.4 million share.

**Evidentiary classification:** The mirror text is an OCR/text rendering of an email chain and attorney statements. It is not a bank statement, wire confirmation, executed warrant, cap table, or proof that warrants were exercised. The chain supports that the lawyer reported receipt of $3.6 million in Ergo's account and that Epstein authorized disclosure of his status as Southern Trust's controlling person. It does not independently establish ultimate beneficial ownership of Carbyne shares, exact source-account debit, exact beneficiary bank credit, closing allocation, or subsequent proceeds.

**Original source check:** The DOJ URL constructed from the independent dataset map, `https://www.justice.gov/epstein/files/DataSet%2011/EFTA02634615.pdf`, resolved to DOJ's age-verification page in the current browser. This is an age-gate flow, not proof the file is unavailable. The original PDF bytes were not obtained or hashed in this review. The third-party mirror must remain labeled secondary until byte-level comparison with DOJ original succeeds.

## 4. Targeted cross-check: EFTA00167059 — Deutsche Bank KYC record

The independent mirror's rendered PDF text identifies a 16-page Deutsche Bank KYC print for a “Southern Financial Relationship,” with case status “Approved,” dated July 30, 2019 and bearing a DB-SDNY production stamp. The first pages describe a Prytanee LLC expense account and identify Southern Trust Company and a separate trust as 50% owners of the account holder. The record includes detailed personal data and a Rule 6(e) confidentiality footer in the rendered pages.

**Handling rule:** Do not reproduce or propagate personal identifiers, residential addresses, dates of birth, tax identifiers, account numbers, signatures or other sensitive personal data. Any further analysis must use only necessary corporate/account-structure fields, with privacy review and page-level checks against the original. Do not assume the KYC document itself is a public bank-authored final determination beyond what its fields actually state. It is a produced record, not proof that every representation was accurate.

This record is a potential financial reconstruction source because it contains bank onboarding and beneficial-ownership fields. It should be queued for controlled, page-specific verification, not bulk copied into a public-facing narrative.

## 5. EFTA-to-dataset mapping discovered

The independent forensic library publishes this EFTA range map and DOJ URL template:
- Dataset 1: EFTA00000001–EFTA00003158
- Dataset 2: EFTA00003159–EFTA00003857
- Dataset 3: EFTA00003858–EFTA00005586
- Dataset 4: EFTA00005705–EFTA00008320
- Dataset 5: EFTA00008409–EFTA00008528
- Dataset 6: EFTA00008529–EFTA00008998
- Dataset 7: EFTA00009016–EFTA00009664
- Dataset 8: EFTA00009676–EFTA00039023
- Dataset 9: EFTA00039025–EFTA01262781
- Dataset 10: EFTA01262782–EFTA02205654 (the independent missing-EFTA report gives a different terminal number in one table; reconcile before using as a boundary)
- Dataset 11: EFTA02205655–EFTA02730264
- Dataset 12: EFTA02730265–EFTA02731783

The independent report itself notes inter-dataset gaps and DS9 Bates/page-count anomalies. These ranges are discovery aids, not an accession manifest. Do not fill numeric gaps by inventing file records; compare actual official listing links, production concordance and original files.

## 6. Revised inventory architecture

Maintain three distinct layers:

1. **Official source inventory:** DOJ collection/listing page, actual link href, source filename, dataset, observed listing page, retrieval status, retrieval timestamp.
2. **Independent discovery index:** API record ID, EFTA identifier, independent corpus/database/table, extraction timestamp, page count, file size, PDF/viewer URL, OCR/transcript status and metadata completeness.
3. **Verified accession:** original DOJ URL, acquired byte count, MIME, SHA-256, page count, privacy review, original-file status and exact page locators.

A third-party document viewer, PDF mirror, API record, OCR text or AI classification must never be silently promoted to an original DOJ accession.

## 7. Immediate next work

1. Use the API's read-only search and document endpoints for targeted discovery and retrieval, preserving exact endpoint, response timestamp and response metadata.
2. Start with already identified high-priority EFTA references and financial/corporate records; do not crawl 1.4 million records indiscriminately.
3. For each target, compare independent metadata and page text with the DOJ original after age verification through the public site.
4. Acquire eligible original files only after privacy screening; hash the actual bytes.
5. Add exact page-level citations to the evidence ledger and link to claims/events/entities only after review.
6. Reconcile the database's changing aggregate counts and source prefixes before reporting corpus totals.
7. Treat analytical reports, AI summaries, entity graph edges, flight reconstructions and semantic-search results as leads, not primary evidence.

## 8. Current result

The independent corpus API is now documented as a usable read-only discovery and text-retrieval channel. A targeted Carbyne warrant email chain was re-inspected, and a potentially relevant bank KYC record was identified with strict privacy handling. No original DOJ files were acquired or SHA-256 hashed during this review. No external tool or infrastructure state was changed.
