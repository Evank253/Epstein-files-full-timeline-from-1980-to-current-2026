# DOJ and public-record corpus acquisition plan

**Status:** Planned ingestion architecture; no claim that the full DOJ corpus has been downloaded.  
**Repository:** Epstein public-record investigation only.

## Primary official collections
- DOJ Epstein Files Library: https://www.justice.gov/epstein
- DOJ Disclosures: https://www.justice.gov/epstein/doj-disclosures
- DOJ OIG Report 23-085: https://oig.justice.gov/sites/default/files/reports/23-085.pdf
- House Oversight majority staff report (2026-11-10): https://oversight.house.gov/wp-content/uploads/2026/11/A-Review-of-the-Federal-Governments-Mishandling-of-the-Jeffrey-Epstein-and-Ghislaine-Maxwell-Criminal-Investigations_OGR-Maj-Report.pdf
- NY DFS Deutsche Bank consent order: https://www.dfs.ny.gov/system/files/documents/2020/07/ea20200706_deutsche_bank_consent_order.pdf
- Senate Finance Committee staff report (2026-08-04): https://www.finance.senate.gov/wp-content/uploads/2026/11/wyden_wall_street_epstein_report.pdf

## Corpus design
Create one accession record per original file, not per webpage or dataset. Preserve dataset name, EFTA/accession number, original filename, original URL, publisher, publication/filing date, retrieval timestamp, byte size, MIME type, SHA-256, page count, OCR/text extraction version, redaction state, privacy review, duplicate cluster, and related claims/events/entities.

Suggested directories:
- `corpus/doj/<dataset>/<accession>/original/` — lawfully redistributable original files only.
- `corpus/doj/<dataset>/<accession>/metadata.json` — provenance and capture metadata.
- `corpus/doj/<dataset>/<accession>/extracted/` — text/OCR and page-level locators, never replacing originals.
- `corpus/court/<jurisdiction>/<case>/` — dockets, orders, pleadings, exhibits and transcripts.
- `corpus/regulator/<agency>/` — consent orders, examination findings and enforcement records.
- `corpus/congress/<committee>/` — reports, letters, hearing transcripts and exhibits.
- `corpus/other-public/<publisher>/` — credible secondary sources, clearly typed as secondary.
- `research/ledgers/` — timeline, claims, evidence, source artifacts, entities, relationships, transactions and duplicate clusters.

## Ingestion sequence
1. Enumerate DOJ library datasets and all public accession/file links; save a dated enumeration snapshot.
2. Download only lawfully accessible, non-prohibited material. Respect site terms, rate limits and access controls; do not bypass restrictions.
3. Save immutable original bytes before parsing. Compute SHA-256 locally from the bytes actually acquired. Never infer a hash from a URL or third-party mirror.
4. Record redirects, retrieval time, response status, content type, filename, byte size and source URL.
5. Extract text with page-level locators; store OCR as a derivative and label OCR confidence. For handwritten material, retain page image references and human transcription status.
6. Deduplicate by cryptographic hash while retaining every source copy and its provenance. Near-duplicate clustering is a separate, reviewable operation.
7. Run privacy review before publishing derivative text or images. Exclude victim PII, intimate imagery, illegal sexual-abuse material, and unnecessary sensitive details.
8. Extract claims only after source review. Each claim links to one or more evidence records and exact locators.
9. Build entity and financial edges only from explicit source support. Record source wording and uncertainty.
10. Independently verify high-impact claims and all financial amounts, corporate ownership and alleged misconduct.
11. Publish ingestion batches with manifest, validation report, unresolved items and change log.

## Completeness accounting
Track at least:
- datasets enumerated / datasets known;
- source links discovered / links tested;
- files acquired / files identified;
- files failed / files withheld / files inaccessible;
- bytes captured and SHA-256 computed;
- PDFs parsed / pages extracted / OCR pages / OCR failures;
- duplicate clusters and unique byte-identical artifacts;
- records privacy-reviewed / quarantined / excluded;
- claims and graph edges linked to primary evidence;
- unresolved or conflicting items.

A page count is not a document count; a file count is not a unique-record count; a link is not an acquisition. Publish completeness as measured counts with denominators and timestamp, never as “all files” unless enumeration and acquisition have been independently reconciled.
