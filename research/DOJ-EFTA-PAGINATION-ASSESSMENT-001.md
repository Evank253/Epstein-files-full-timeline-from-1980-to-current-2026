# DOJ EFTA dataset pagination assessment — 001

**Assessment date:** 2026-11-17  
**Authority:** Official DOJ Epstein Library dataset listing pages  
**Scope:** Pagination controls and first-page listing structure for EFTA datasets 1–12.  
**Status:** Partial assessment. Last-page targets were discovered from DOJ pagination controls, but the web retrieval layer returned HTTP 403 for those target pages. No full pagination crawl or complete file enumeration is claimed.

## 1. Observed pagination

| Dataset | First page listing | Pagination observation | Last-page target from DOJ control | Retrieval result |
|---:|---|---|---:|---|
| 1 | 50 file links observed | Numbered pages 1–9, ellipsis, Next, Last | `?page=62` | HTTP 403 |
| 2 | 50 file links observed | Numbered pages 1–9, ellipsis, Next, Last | `?page=11` | HTTP 403 |
| 3 | 50 file links observed | Pages 1–2, Next, Last | `?page=1` | Not fetched in this assessment |
| 4 | 50 file links observed | Pages 1–4, Next, Last | `?page=3` | Not fetched in this assessment |
| 5 | 50 file links observed | Pages 1–3, Next, Last | `?page=2` | Not fetched in this assessment |
| 6 | 13 file links observed | No numbered page controls or next/last controls in returned page | Not shown | First-page listing only; single-page status not independently confirmed |
| 7 | 17 file links observed | No numbered page controls or next/last controls in returned page | Not shown | First-page listing only; single-page status not independently confirmed |
| 8 | 50 file links observed | Numbered pages 1–9, ellipsis, Next, Last | `?page=220` | HTTP 403 |
| 9 | 50 file links observed | Numbered pages 1–9, ellipsis, Next, Last | `?page=10674` | HTTP 403 |
| 10 | 50 file links observed | Numbered pages 1–9, ellipsis, Next, Last | `?page=10080` | HTTP 403 |
| 11 | 50 file links observed | Numbered pages 1–9, ellipsis, Next, Last | `?page=6633` | HTTP 403 |
| 12 | 50 file links observed | Pages 1–4, Next, Last | `?page=3` | Not fetched in this assessment |

**Interpretation:** The Last controls reveal large pagination depths for datasets 1, 8, 9, 10 and 11. The values are zero-based page query parameters exposed by the official site links; they are not file counts. With 50 links on an observed first page, these listings may represent very large numbers of records, but no total file count should be calculated until page semantics, final-page size, and duplicate behavior are verified.

## 2. Retrieval limitation

The web retrieval service returned HTTP 403 when following the official Last-page links for datasets 1, 2, and 8–11. This is a retrieval-layer access failure, not evidence that the DOJ pages or records do not exist. The official listing pages themselves were accessible and exposed the pagination targets.

The assessment does not attempt to bypass access controls, age gates, rate limits or other technical restrictions. Continue through lawful, official access methods and preserve any failure response as an acquisition limitation.

## 3. First-page structure observations

- Datasets 1, 2, 3, 4, 5, 8, 9, 10, 11 and 12 exposed 50 PDF links in the page response reviewed.
- Dataset 6 exposed 13 PDF links in the returned page.
- Dataset 7 exposed 17 PDF links in the returned page.
- EFTA identifiers are visibly non-contiguous in several datasets. Numeric gaps must not be treated as omitted files.
- The listing pages carry DOJ's privacy warning: inadvertent non-public PII or sensitive material may remain despite review and redaction.

## 4. Next enumeration protocol

1. Use official DOJ listing pages and their pagination links; do not infer filenames or fill EFTA-number gaps.
2. Record every page URL, retrieval timestamp, HTTP status, and exact set of linked file URLs.
3. For pages that return 403, record the failure and pursue an authorized alternate official access method; do not silently skip them.
4. Enumerate all files under Court Records, FOIA and Prior DOJ Disclosures as separate collection families.
5. Do not acquire or process illegal sexual-abuse material or intimate imagery. Quarantine records with exposed victim/witness PII and do not propagate sensitive content.
6. Compute hashes only after eligible original bytes are lawfully acquired.
7. Independently compare enumerated listing counts with DOJ's stated production scope; page count and production-page count are different measures.

## 5. Current conclusion

Pagination depth is much larger than the initial first-page inventory implied. In particular, DOJ pagination exposes last-page indices of 10,674 for dataset 9 and 10,080 for dataset 10. These are page indices, not verified file totals. The evidence-corpus inventory remains incomplete, and no original corpus files were acquired or hashed in this assessment.
