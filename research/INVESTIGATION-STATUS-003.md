# Investigation status — 2026-11-17 (DOJ inventory phase opened)

## Repository boundary
All investigation artifacts in this phase are committed only to `Evank253/Epstein-files-full-timeline-from-1980-to-current-2026`, branch `research/initial-evidence-linked-timeline`. No other repository was accessed for writes.

## New committed artifacts
- `research/DOJ-MASTER-INVENTORY-001.md` — top-level DOJ Library and Disclosures discovery snapshot.
- `research/DOJ-COLLECTION-REGISTER-001.csv` — initial collection register for twelve EFTA datasets and consolidated collections.

## Current discovery result
- DOJ Epstein Library landing page located.
- DOJ Disclosures hub located.
- Twelve numbered EFTA datasets identified.
- Court Records hub listing contains 51 case/court collection entries in the current rendered page.
- Four FOIA subcollections identified: CBP, FBI, BOP and Florida.
- Four Prior DOJ Disclosures subcollections identified: First Phase, BOP Video Footage, Maxwell Proffer, Memoranda and Correspondence.
- Official review protocol, DOJ production announcement, congressional letters and Section 3 report links identified.
- House Committee on Oversight disclosures are separately linked from the DOJ Epstein Library landing page and are an external collection, not one of the DOJ EFTA datasets. They must be inventoried as a separate source family.

## What is not complete
- No complete page-by-page pagination crawl has been performed for the twelve datasets.
- No file-by-file enumeration has been completed for the Court Records, FOIA or Prior DOJ Disclosures collections.
- No eligible original DOJ files were acquired, downloaded or hashed in this phase.
- No OCR or text extraction corpus has been created.
- No complete corpus count or completeness claim is made.

## Acquisition controls
- Preserve one accession per source listing, including duplicate appearances across collections.
- Capture original bytes only when lawful and after privacy review; never download, transform, index or redistribute illegal sexual-abuse material or intimate imagery.
- If a public record exposes victim/witness PII or other sensitive content, quarantine the accession and do not propagate the content.
- Compute SHA-256 only from bytes actually acquired; record retrieval timestamp, byte count, MIME type and original source URL.
- Keep DOJ originals distinct from third-party mirrors, OCR/transcriptions and derivative extracts.
- Record exact PDF page locators and distinguish printed page numbers.
- Inclusion in DOJ's production is not authentication; DOJ states the production may include false or falsely submitted material.

## Next actions
1. Enumerate all pagination pages and every file link in EFTA datasets 1–12.
2. Enumerate all files under each Court Records, FOIA and Prior DOJ Disclosures subcollection.
3. Inventory House Committee disclosures as a separate collection family.
4. Reconcile duplicate appearances using byte hashes only after acquisition.
5. Start controlled acquisition batches with privacy review and an auditable file-level manifest.
6. Independently audit counts, source integrity and evidence linkage.
