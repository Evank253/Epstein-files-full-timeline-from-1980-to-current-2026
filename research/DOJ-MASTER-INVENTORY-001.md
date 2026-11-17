# DOJ Epstein Library — Master Inventory Snapshot 001

**Snapshot date:** 2026-11-17  
**Source authority:** U.S. Department of Justice, Epstein Library  
**Status:** Initial top-level inventory and dataset discovery. NOT a complete file-level enumeration.  
**Repository destination:** This repository and branch only.

## 1. Official entry points

| Accession | Collection | Official source | Discovery status |
|---|---|---|---|
| DOJ-LIB-ROOT-001 | Epstein Library landing page | https://www.justice.gov/epstein | Located; live page |
| DOJ-DISCLOSURES-001 | DOJ Disclosures hub | https://www.justice.gov/epstein/doj-disclosures | Located; enumerates 12 EFTA datasets plus Court Records, FOIA and Prior DOJ Disclosures |
| DOJ-SEARCH-001 | Search Full Epstein Library | https://www.justice.gov/epstein/search | Located; DOJ warns search may omit or misread handwritten/non-electronic text |
| DOJ-RELEASE-001 | January 30, 2026 production announcement | https://www.justice.gov/opa/pr/department-justice-publishes-35-million-responsive-pages-compliance-epstein-files | Official DOJ release description |
| DOJ-LETTER-001 | EFTA production letter to Congress | https://www.justice.gov/opa/media/1426091/dl?inline= | Official DOJ production protocol and scope |
| DOJ-SECTION3-001 | February 14, 2026 Section 3 report | https://www.justice.gov/opa/media/1434856/dl?inline= | Official categories released/withheld and redaction report |
| DOJ-REVIEW-PROTOCOL-001 | EFTA First Level Review Protocol | https://www.justice.gov/media/1426281/dl | Official review/redaction protocol |

## 2. DOJ Disclosures — EFTA datasets

The DOJ Disclosures hub currently exposes twelve numbered EFTA datasets. The individual dataset pages use paginated file listings; the initial crawl exposed only the first page for most datasets. Consequently, the dataset rows below are discovery records, not final file counts.

| Accession | Dataset | Official listing URL | Observed first-page accession range / examples | Pagination observed | File-level status |
|---|---:|---|---|---|---|
| DOJ-EFTA-DS01 | 1 | https://www.justice.gov/epstein/doj-disclosures/data-set-1-files | EFTA00000001.pdf–EFTA00000050.pdf | Pages 1–9 plus next/last controls | Not exhaustively enumerated |
| DOJ-EFTA-DS02 | 2 | https://www.justice.gov/epstein/doj-disclosures/data-set-2-files | EFTA00003159.pdf–EFTA00003207.pdf | Pages 1–9 plus next/last controls | Not exhaustively enumerated |
| DOJ-EFTA-DS03 | 3 | https://www.justice.gov/epstein/doj-disclosures/data-set-3-files | First page includes EFTA00003380.pdf, EFTA00003434–03441.pdf and later IDs through EFTA00004250.pdf | Pages 1–2 | Not exhaustively enumerated |
| DOJ-EFTA-DS04 | 4 | https://www.justice.gov/epstein/doj-disclosures/data-set-4-files | First page includes EFTA00005705.pdf through EFTA00006371.pdf (non-contiguous) | Pages 1–4 | Not exhaustively enumerated |
| DOJ-EFTA-DS05 | 5 | https://www.justice.gov/epstein/doj-disclosures/data-set-5-files | EFTA00008409.pdf–EFTA00008457.pdf | Pages 1–3 | Not exhaustively enumerated |
| DOJ-EFTA-DS06 | 6 | https://www.justice.gov/epstein/doj-disclosures/data-set-6-files | First page includes EFTA00008529.pdf through EFTA00008998.pdf (non-contiguous) | Page controls not visible in captured first-page response | Not exhaustively enumerated |
| DOJ-EFTA-DS07 | 7 | https://www.justice.gov/epstein/doj-disclosures/data-set-7-files | First page includes EFTA00009016.pdf through EFTA00009664.pdf (non-contiguous) | Page controls not visible in captured first-page response | Not exhaustively enumerated |
| DOJ-EFTA-DS08 | 8 | https://www.justice.gov/epstein/doj-disclosures/data-set-8-files | First page includes EFTA00009676.pdf through EFTA00009890.pdf (non-contiguous) | Pages 1–9 plus next/last controls | Not exhaustively enumerated |
| DOJ-EFTA-DS09 | 9 | https://www.justice.gov/epstein/doj-disclosures/data-set-9-files | First page includes EFTA00039025.pdf through EFTA00039820.pdf (non-contiguous) | Pages 1–9 plus next/last controls | Not exhaustively enumerated |
| DOJ-EFTA-DS10 | 10 | https://www.justice.gov/epstein/doj-disclosures/data-set-10-files | First page includes EFTA01262782.pdf through EFTA01263288.pdf (non-contiguous) | Pages 1–9 plus next/last controls | Not exhaustively enumerated |
| DOJ-EFTA-DS11 | 11 | https://www.justice.gov/epstein/doj-disclosures/data-set-11-files | First page includes EFTA02209722.pdf through EFTA02212953.pdf (non-contiguous) | Pages 1–9 plus next/last controls | Not exhaustively enumerated |
| DOJ-EFTA-DS12 | 12 | https://www.justice.gov/epstein/doj-disclosures/data-set-12-files | First page includes EFTA02730265.pdf through EFTA02731485.pdf (non-contiguous) | Pages 1–4 | Not exhaustively enumerated |

**Important:** EFTA identifiers are not guaranteed to be contiguous. Never infer missing records by filling numerical gaps. Enumerate actual links from each page and every pagination page.

## 3. DOJ Disclosures — consolidated collections

The DOJ hub also exposes these collections outside the twelve numbered datasets:

### 3.1 Court Records
Official hub section: https://www.justice.gov/epstein/doj-disclosures  
The page lists **51 named case/court collection entries** in the current rendered listing. These include Florida state criminal matters, SDNY criminal matters, civil actions, appeals, estate proceedings, the USVI/JPMorgan litigation, and the 2025 grand-jury matter. Treat each listed case as a collection parent; enumerate all files within each case page before declaring it complete.

DOJ notes that this consolidated collection includes records previously on the former Court Records page, with additional DOJ victim-identifying redactions and pre-existing redactions under applicable rules, statutes and court orders. Grand-jury, personal-identifier, Crime Victims' Rights Act and protective-order restrictions remain material to interpretation.

### 3.2 Freedom of Information Act (FOIA)
Official hub section: https://www.justice.gov/epstein/doj-disclosures  
Four top-level FOIA collections are listed:
- Customs and Border Protection (CBP)
- Federal Bureau of Investigation (FBI)
- Federal Bureau of Prisons (BOP)
- Florida

DOJ describes these as previously released records consolidated from the former FOIA page, with pre-existing redactions under FOIA and Florida public-records law.

### 3.3 Prior DOJ Disclosures
Official hub section: https://www.justice.gov/epstein/doj-disclosures  
Four top-level collections are listed:
- First Phase of Declassified Epstein Files
- BOP Video Footage
- Maxwell Proffer
- Memoranda and Correspondence

These are legacy disclosure groupings consolidated into the current hub. They may overlap the numbered datasets and/or court/FOIA collections. Preserve duplicates and link them into duplicate clusters; do not delete or silently collapse source copies.

## 4. Related official documentation

The DOJ hub links:
- Attorney Review Protocol for Epstein Files.
- January 30, 2026 production announcement.
- December 19, 2025 letter to Congress.
- January 30, 2026 letter to Congress.
- February 14, 2026 Section 3 report to Congress.

The January 30 DOJ release states that the combined production was nearly 3.5 million pages, including more than 2,000 videos and 180,000 images. It describes materials gathered from Florida and New York Epstein cases, the New York Maxwell case, investigations into Epstein's death, a Florida former-butler case, multiple FBI investigations and the DOJ OIG death investigation. This is DOJ's description of its production, not an independent count of the currently crawlable website files.

DOJ also states that the production can include false or falsely submitted material received from the public. Every item therefore requires source, provenance and evidentiary classification; inclusion in the production is not authentication.

## 5. Critical safety and evidentiary controls

1. The DOJ itself warns that, despite review/redaction, the public library may inadvertently contain non-public PII or other sensitive information.
2. Do not copy, publish, transform, OCR, index, or redistribute intimate imagery, child sexual abuse material, or other illegal sexual-abuse material. Do not download such material for this project.
3. Do not reproduce victim or witness identifying information. If a record appears to expose it, quarantine the accession metadata, record the source locator and privacy issue, and do not propagate the sensitive content.
4. Preserve lawful, redacted documentary records only after a privacy review. A record's presence in DOJ production does not establish its truth.
5. Distinguish original DOJ bytes from third-party mirrors, OCR/transcriptions, search snippets and derivative extracts.
6. Hash only bytes actually acquired. Record algorithm, retrieval time, byte count and source URL. Never infer a hash from a URL or filename.
7. Maintain separate statuses: DISCOVERED_URL, LISTING_ENUMERATED, ACQUIRED_BYTES, HASH_VERIFIED, PRIVACY_REVIEWED, TEXT_EXTRACTED, PAGE_LOCATORS_VERIFIED, CLAIM_LINKED, INDEPENDENTLY_REVIEWED.
8. Preserve duplicates as separate accessions; create duplicate-cluster relationships only after content-hash comparison.
9. Exact page locators must identify the DOJ PDF page number as rendered, and distinguish printed page numbers where present.
10. No inference of wrongdoing, criminal participation, intelligence affiliation or state sponsorship from appearance, proximity, association or graph connectivity.

## 6. Acquisition manifest schema

The next file-level manifest should use one row per source-file listing, with at least:

`accession_id, collection_id, dataset_number, source_title, source_url, source_filename, source_host, listing_page_url, listing_page_number, discovery_timestamp_utc, listing_status, acquisition_status, acquired_timestamp_utc, byte_size, mime_type, sha256, original_preservation_path, pdf_page_count, extraction_tool, extraction_version, ocr_required, ocr_status, privacy_review_status, redaction_notes, duplicate_cluster_id, evidence_record_ids, claim_ids, event_ids, entity_ids, exact_page_locators, reviewer, review_timestamp_utc, limitations`.

Do not fill acquisition/hash/extraction fields until the underlying bytes have actually been obtained and checked.

## 7. Work completed in this snapshot

- Confirmed DOJ Library landing page and DOJ Disclosures hub.
- Confirmed twelve numbered EFTA datasets.
- Opened the first listing page for each of the twelve datasets.
- Observed pagination on datasets 1–5 and 8–12; datasets 6–7 need a second pass to inspect pagination controls and page structure.
- Identified 51 case/court collection entries, four FOIA collections and four prior-disclosure collections on the DOJ hub.
- Located official DOJ production, review protocol and Section 3 report documentation.

## 8. Outstanding work — do not mark complete

- Enumerate every pagination page for all twelve EFTA datasets.
- Enumerate every file under all 51 Court Records case collections.
- Enumerate every file under all four FOIA and four Prior DOJ Disclosures collections.
- Capture an immutable dated snapshot of every listing page and its complete link set.
- Reconcile duplicate appearances across collections without deleting any source accession.
- Determine which file types are eligible for lawful preservation after privacy review.
- Acquire eligible original files in controlled batches; compute SHA-256 from acquired bytes.
- Build the file-level accession manifest and reconcile its counts against the live DOJ listings.
- Independently audit listing completeness and acquisition integrity.

**Current conclusion:** This is a verified top-level discovery baseline, not a complete master inventory and not an acquired evidence corpus. No original DOJ corpus files were downloaded or hashed as part of this snapshot.
