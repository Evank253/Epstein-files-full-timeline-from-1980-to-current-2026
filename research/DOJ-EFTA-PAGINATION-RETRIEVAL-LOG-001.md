# DOJ EFTA pagination retrieval log — 001

**Assessment date:** 2026-11-17  
**Scope:** Re-check of datasets 9 and 10, including numbered pagination links and Last controls.  
**Status:** First-page listing independently re-observed; subsequent pages blocked to the current retrieval client.

## Dataset 9

- Official listing: https://www.justice.gov/epstein/doj-disclosures/data-set-9-files
- First page returned 50 PDF links.
- The listing exposes numbered page links 1–9, Next, and Last.
- Last target is ?page=10674.
- Retrieval of ?page=0 succeeded and returned the same 50-link first-page listing.
- Retrieval of ?page=1 through ?page=8 returned HTTP 403.
- Retrieval of ?page=10674 returned HTTP 403.
- First-page accession identifiers are recorded in DOJ-EFTA-FIRST-PAGE-REGISTER-001.csv.

## Dataset 10

- Official listing: https://www.justice.gov/epstein/doj-disclosures/data-set-10-files
- First page returned 50 PDF links.
- The listing exposes numbered page links 1–9, Next, and Last.
- Last target is ?page=10080.
- Retrieval of ?page=10080 returned HTTP 403.
- First-page accession identifiers are recorded in DOJ-EFTA-FIRST-PAGE-REGISTER-001.csv.

## Interpretation

The large last-page indices are actual pagination targets exposed by DOJ page controls, not estimated file totals. The current retrieval client cannot fetch most non-zero pages. This does not establish that DOJ blocks all users or all lawful access methods.

The first-page register contains 100 source-listing entries across datasets 9 and 10. These are listing records only: no PDF bytes were acquired, no file SHA-256 hashes were calculated, and the PDF URL patterns in the register must be checked against actual anchor hrefs before acquisition. The official HTML page's linked PDF targets are authoritative over guessed URL patterns.

## Next steps

1. Obtain actual href targets from official listing HTML using an authorized retrieval method that respects DOJ access controls.
2. Continue pagination through official page links only; log status and timestamp for each page.
3. Do not substitute EFTA numeric ranges for observed file links.
4. Once file bytes are lawfully acquired and privacy-reviewed, calculate SHA-256 and record byte length, MIME type and acquisition timestamp.
5. Keep listing discovery, file acquisition and evidentiary verification as separate states.
