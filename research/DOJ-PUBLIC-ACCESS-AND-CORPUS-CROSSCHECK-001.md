# DOJ public-access correction and independent corpus cross-check — 001

**Date:** 2026-11-17  
**Repository:** Epstein investigation repository only  
**Status:** Corrective research note; no original DOJ files acquired in this step.

## 1. Correction to prior access characterization

The DOJ Epstein Library and DOJ Disclosures are publicly accessible government resources, subject to the site's age gate and its stated privacy/redaction limitations. The HTTP 403 responses encountered when following numbered pagination links came from the retrieval interface used in this investigation session. They do not establish that DOJ restricted public access, that the records are unavailable, or that the user lacks lawful access.

The correct description is:

**Public DOJ records; pagination requests failed through the current retrieval interface.**

The official DOJ dataset 9 page is accessible and exposes 50 first-page PDF links plus numbered pagination links and a Last control. The official DOJ Disclosures hub lists all twelve datasets and consolidated Court Records, FOIA and Prior DOJ Disclosures collections.

## 2. Official source confirmation

- DOJ Epstein Library: https://www.justice.gov/epstein
- DOJ Disclosures: https://www.justice.gov/epstein/doj-disclosures
- Dataset 9: https://www.justice.gov/epstein/doj-disclosures/data-set-9-files
- Dataset 10: https://www.justice.gov/epstein/doj-disclosures/data-set-10-files

The official DOJ landing page states the library was last updated September 11, 2026 at the time of this review. DOJ warns that search may fail or be unreliable for handwritten or otherwise non-electronic text. DOJ also warns that sensitive information may inadvertently remain in the public production despite review and redaction.

## 3. Independent full-text corpus discovered

An independent third-party research database, Epstein Files Research Database (epstein-data.com), describes a full-text corpus with:
- 1,425,565 document records;
- 2,923,763 pages;
- records across all 12 DOJ datasets, House Oversight estate documents and FBI Vault files;
- document metadata including EFTA number, dataset, total pages, extraction timestamp, file size, document classification and source PDF URL where available.

Its documents table states one row per document and provides a REST API for structured search. The database also labels itself independent and not affiliated with DOJ, and warns users to verify claims against source documents.

This is a potentially useful **secondary discovery and reconciliation index**, not an official DOJ inventory, not a substitute for DOJ source listings, and not evidence that 1,425,565 unique DOJ files exist. The total spans multiple source families, may include duplicates, and is an index count rather than a count of DOJ-only originals.

Official DOJ URLs embedded in the third-party records may accelerate source locator resolution. Every such locator must be checked against the actual official DOJ response and actual downloaded bytes before being promoted to an acquired source record.

## 4. Proposed use of the independent index

Use only as a discovery aid:
1. Search by exact EFTA accession or source family.
2. Capture the third-party record identifier, extraction timestamp, page count, file size and any official DOJ PDF URL.
3. Label all metadata as third-party extracted metadata.
4. Verify the PDF URL and accession against the official DOJ page or direct DOJ file response.
5. Acquire the original from DOJ only; compute SHA-256 from the bytes actually acquired.
6. Compare the independently indexed page count and file size with the acquired original, where available.
7. Preserve mismatches, duplicate candidates and extraction errors as unresolved audit records.
8. Never treat third-party OCR, AI classification, sender fields, dates or document summaries as primary evidence without checking the original.

## 5. Acquisition and privacy rules

- Public availability does not remove the need for privacy review.
- Do not download, reproduce, OCR, index or redistribute illegal sexual-abuse material or intimate imagery.
- Quarantine any record that appears to expose victim/witness identifying information or other sensitive content and do not propagate that content.
- Preserve eligible redacted documentary originals and their metadata where lawful.
- Maintain distinct statuses for discovered, listing-enumerated, acquired, hashed, privacy-reviewed, extracted, page-verified and independently reviewed.
- Do not invent counts or hashes; no original DOJ file bytes were acquired in this assessment.

## 6. Current conclusion

The previous wording implying that DOJ's public access was itself blocked was inaccurate. DOJ's resources are public; the 403 is a limitation of the retrieval interface used here. An independent secondary full-text index may provide a way to cross-check and accelerate discovery at scale, but the official DOJ source remains authoritative for original acquisition and the investigation's source-of-record status.
