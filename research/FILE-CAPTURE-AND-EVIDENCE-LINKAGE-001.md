# FILE-LEVEL CAPTURE & EVIDENCE LINKAGE PROTOCOL — 001
Investigation: EPSTEIN-PUBLIC-RECORD-INVESTIGATION-001
Status: Protocol established; source files not yet bulk captured.

## 1. Every acquired file receives a permanent artifact record
Record source ID, publisher, canonical and acquisition URL, UTC retrieval time, original filename, MIME type, byte size, SHA-256 of exact original bytes, publication/file date, embedded metadata, dataset/accession number, docket/case/document number, page count, access terms, redaction/privacy classification, acquisition method, HTTP receipt metadata, and immutable storage location.

A URL is NOT a captured file. Never invent a hash or copy a hash from an unrelated index.

## 2. Immutable original and working derivatives
Store exact downloaded original read-only. Compute SHA-256 before transformation. Clone before OCR, extraction, normalization, conversion or redaction. Each derivative gets its own artifact ID, hash, parent ID, tool/version, run ID and transformation log. Preserve duplicate copies; link them with duplicate-cluster IDs rather than deleting them.

## 3. Page-level evidence
Every extracted statement gets claim ID and evidence ID. Each evidence record resolves to source artifact ID, SHA-256, page/line/timecode/row/cell, quote or faithful summary, extraction method, evidence status and reviewer. If a report cites a source not acquired, mark it as secondary to the underlying source.

## 4. Graph requirements
Entity nodes have stable IDs and aliases. Events have date precision, place only when documented, participants, source IDs and evidence IDs. Relationship edges are typed, time-bounded where possible, and always carry evidence IDs. A mention is not a relationship. Graph centrality/proximity never establishes guilt, intent or intelligence affiliation. Victim/witness identities are excluded from public graph exports.

## 5. Status vocabulary
URL_IDENTIFIED_NOT_CAPTURED; CAPTURED_HASHED; OCR_COMPLETE; EXTRACTED_PAGE_LINKED; DUPLICATE_RECONCILED; INDEPENDENTLY_VERIFIED; DISPUTED; WITHHELD; ACCESS_GAP; NOT_MEASURED.

## 6. Current state
The initial timeline and graph seed are being established from cited public reports and court/regulator records. The source-artifact register lists 16 high-value public source locations, all initially URL_IDENTIFIED_NOT_CAPTURED. No original-file SHA-256 values or byte counts are populated yet. Next phase: acquire each accessible original, hash it, extract exact page locators and attach every claim and event to that file-level artifact.
