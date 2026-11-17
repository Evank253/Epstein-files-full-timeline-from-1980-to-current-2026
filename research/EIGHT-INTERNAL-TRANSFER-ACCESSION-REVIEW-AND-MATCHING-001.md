# Eight internal-transfer accession review and debit/credit matching — 001

**Review date:** 2026-11-17  
**Destination:** Authorized Epstein investigation repository only  
**Source status:** Public DOJ locator leads plus independent OCR/indexes and an AI-generated secondary report.  
**Acquisition status:** Original DOJ PDF bytes were not downloaded in this review; no SHA-256 hashes or byte-level verification are claimed.

## 1. Executive result

The eight requested EFTA references are not yet eight independently verified, settled transactions. The independent report labels them as internal-transfer records, but the accessible source material reveals a mixture of:
- statement-page/accession references;
- monthly account-statement PDFs that contain multiple transaction lines;
- transfer-request descriptions;
- document identifiers whose counterpart account or matching credit is not yet established.

The most useful immediate finding is that the 2013 records sit in a run of Jeffrey E. Epstein Deutsche Bank primary-account statements. Independent indexes identify EFTA01482271 as a statement for 2013-03-30 through 2013-04-30, and EFTA01528427 as a 17-page April 2013 statement containing two internal-transfer lines. EFTA01528444 is identified as a 15-page May 2013 statement containing other transaction activity, including a book transfer to Jet Ops LLC; the internal-transfer line attributed to it must be located on the actual page before assigning that counterparty.

No debit/credit pair among the eight has yet been matched to a receiving-account statement. Treat all eight as unmatched transfer candidates.

## 2. Identifier-by-identifier findings

### EFTA01482260 — reported March 18 “Internal Transfer of Funds, As Requested”
- Independent report index: describes the record as an internal transfer dated 03/18 and “As Requested”.
- Adjacent public archive search results identify EFTA01482259 as a one-page continuation of Jeffrey Epstein's primary Deutsche Bank statement for 2013-03-01 through 2013-03-29. The OCR on that adjacent page shows two “Internal Transfer of Funds As Requested” entries dated 03/01, but those are not automatically the same event as the 03/18 entry attributed to EFTA01482260.
- An adjacent archive record EFTA01482261 is titled “Funds transfer request (March 11 2013)” and reproduces a continuation of the same March statement; it shows later March transactions. This indicates that the surrounding accession sequence contains statement continuation pages and a separate transfer-request record/copy.
- **Not established:** amount, origin/destination account, transfer direction, whether the request was executed, and receiving credit.
- Priority: obtain the actual DOJ PDF whose first-page Bates identifier covers EFTA01482260 and identify its page-level Bates range; inspect the preceding/following statement and request pages.

### EFTA01482271 — April 5 “Internal Transfer of Funds, As Requested”
- Independent report index: describes the record as an internal transfer dated 04/05.
- Independent document search identifies EFTA01482271 as a Jeffrey Epstein primary-account transaction-detail statement for 2013-03-30 through 2013-04-30. Search-index text shows the transaction table begins around 04/03.
- **Not established:** exact transfer amount, counterparty account, direction, posting status, or matching credit.
- Priority: inspect the original statement page and the adjacent transaction rows; then search the receiving account statement for same date/amount.

### EFTA01482474 — “Internal Funds Transfer”
- Independent AI-generated report lists this identifier as an internal funds transfer, without date, amount, account, counterparty or debit/credit designation.
- **Not established:** all transaction-level details.
- Priority: locate the DOJ PDF and identify the actual Bates page; extract surrounding table rows and statement period before creating a transaction record.

### EFTA01482494 — “Internal Funds Transfer”
- Independent AI-generated report lists this identifier as an internal funds transfer, without date, amount, account, counterparty or debit/credit designation.
- **Not established:** all transaction-level details.
- Priority: same as EFTA01482474. Do not infer it belongs to the same account or statement period solely from numeric proximity.

### EFTA01482500 — “Internal Funds Transfer”
- Independent AI-generated report lists this identifier as an internal funds transfer, without date, amount, account, counterparty or debit/credit designation.
- **Not established:** all transaction-level details.
- Priority: same as EFTA01482474. Numeric proximity is not proof of a shared transfer or account.

### EFTA01482650 — “Internal Funds Transfer - JEFFREY E EPSTEIN”
- Independent AI-generated report lists this identifier with a Jeffrey Epstein descriptor.
- The descriptor may identify a named party or a transaction narrative; it does not by itself identify the sending account, receiving account, amount, or whether the item is a debit or credit.
- **Not established:** transfer direction, amount, account ownership, execution/settlement, or matching entry.
- Priority: inspect original image and transaction table; establish which field the name appears in.

### EFTA01528427 — April 2013 statement / internal-transfer entries
- Independent search index identifies a 17-page Dataset 10 record dated 2013-04-30 and describes it as an account statement.
- OCR search result for the DOJ PDF URL shows:
  - statement transaction rows include “04/18 Internal Transfer of Funds” and “04/24 Internal Transfer of Funds”;
  - both are associated in the extracted text with “As Requested” wording;
  - the statement also contains unrelated items including Chase card payments, a Fedwire debit to Zorro Development Corp., and an American Express ACH payment.
- The snippet does not reliably preserve the table-column alignment. The amounts visible nearby (including $49,475.35, $2,837.94, $102,758.01, $26,041.18 and $111.29) cannot safely be assigned to the two internal-transfer lines without the original page image.
- **Not established:** which of the two internal-transfer lines corresponds to the specific accession EFTA01528427, exact amount, counterparty, debit/credit, and matching credit. EFTA01528427 appears to be a multi-page statement PDF; it should not be treated as one transfer.
- Priority: inspect all 17 pages and preserve the exact page-level Bates identifiers for the 04/18 and 04/24 rows. Locate matching receiving-account statements.

### EFTA01528444 — May 2013 statement / internal-transfer lead
- Independent search index identifies a 15-page Dataset 10 statement dated 2013-05-31.
- Its OCR snippet includes 05/28 Fedwire activity, 05/29 Fedwire to Zorro Development Corp., an American Express ACH payment, and a 05/30 book transfer to Jet Ops LLC. The independent AI report separately labels EFTA01528444 as an “Internal Transfer”.
- The book transfer to Jet Ops LLC is a distinct transaction description and must not be conflated with the internal-transfer label. The exact internal-transfer row and its amount are not exposed in the search snippet.
- **Not established:** exact date, amount, counterparty, direction, settlement or matched credit for the specific internal-transfer item.
- Priority: inspect the 15-page statement and identify the precise page and row for the reported internal transfer; separately record the Jet Ops book transfer if relevant.

## 3. Critical distinction: EFTA number versus transaction number

An EFTA accession/Bates identifier identifies a page or the beginning of a produced file, not necessarily one unique bank transaction. A single monthly statement PDF may contain multiple transaction rows and multiple consecutive Bates page numbers. Therefore:
- Do not create one transaction record for every EFTA identifier automatically.
- First resolve the PDF's starting Bates number, total page count and the exact page containing the relevant row.
- Record the transaction as a row-level event with its own stable internal transaction ID.
- Link that event to the document accession and exact Bates page.
- If one statement contains two transfer rows, create two transaction records and link both to the same source PDF/page as appropriate.

## 4. Debit/credit matching protocol

A transfer is considered matched only when the source and receiving records agree on enough independent fields:
1. Same transaction date or documented posting/value-date offset.
2. Same amount and currency.
3. Debit and credit signs are consistent with direction.
4. Origin and destination account identifiers match (masked in public artifacts).
5. Internal transfer reference, transaction ID or bank trace matches where available.
6. Statement opening/closing balances reconcile with the transaction.
7. Reversals, corrections, duplicate copies and pending/returned status are checked.

A matching amount and date alone is a candidate match, not conclusive proof. If one side is redacted, record the match as partial and state which fields are unavailable.

## 5. Transaction ledger status

| EFTA reference | Current description | Date known from index | Amount | Direction | Counterparty | Matched credit |
|---|---|---|---|---|---|---|
| EFTA01482260 | Internal transfer, as requested | 2013-03-18 (secondary report) | Unknown | Unknown | Unknown | No |
| EFTA01482271 | Internal transfer, as requested | 2013-04-05 (secondary report) | Unknown | Unknown | Unknown | No |
| EFTA01482474 | Internal funds transfer | Unknown | Unknown | Unknown | Unknown | No |
| EFTA01482494 | Internal funds transfer | Unknown | Unknown | Unknown | Unknown | No |
| EFTA01482500 | Internal funds transfer | Unknown | Unknown | Unknown | Unknown | No |
| EFTA01482650 | Internal funds transfer; Epstein name in descriptor | Unknown | Unknown | Unknown | Unknown | No |
| EFTA01528427 | Internal transfer row(s) in April 2013 statement | 2013-04-18 and 2013-04-24 rows visible in OCR; exact Bates-row mapping pending | Unknown | Unknown | Unknown | No |
| EFTA01528444 | Internal-transfer lead in May 2013 statement | May 2013 statement; exact row date pending | Unknown | Unknown | Unknown | No |

## 6. Related records for follow-through

The independent inter-entity report also identifies these as separate transfer candidates:
- EFTA01482909
- EFTA01482935
- EFTA01482950
- EFTA01482967
- EFTA01483035
- EFTA01483039

That report asserts some transfers originate from Epstein's personal Deutsche Bank account and lists partial destination account identifiers. This is a high-value lead, but the source pages and destination-account ownership records must be inspected before treating the reported network as verified. Do not reproduce full account numbers in public output. A separate Morgan Online Administration Tool record family is cited by the report as identifying an asset account associated with Southern Trust; verify the actual records before concluding that Southern Trust assets were liquidated into a personal account.

## 7. Source limitations and reliability

- The independent inter-entity report is explicitly AI-generated and warns that it may contain errors.
- Independent document-search snippets and archive transcriptions are OCR/search aids, not the original DOJ PDF.
- A third-party archive may label an accession as a duplicate or title match; verify the original file and Bates range before deciding whether it is a duplicate.
- The DOJ PDF URLs are discoverable from the official Dataset 10 path pattern, but the browser retrieval used in this review did not return the PDF bytes.
- No original PDF page images were reviewed in this step.
- No original DOJ file bytes, MIME types, file sizes or SHA-256 values were acquired.
- No debit/credit pair has been confirmed.

## 8. Priority next action

Acquire the original Dataset 10 statement PDFs through an authorized public-access browser path, starting with the monthly statements covering March, April and May 2013. For each, capture original bytes and hash, then visually inspect the relevant statement page(s), extract exact transaction rows, and search the other Deutsche Bank account statements for matching credits. Only then promote an item from “unmatched candidate” to “partially matched” or “matched”.

This report is a source-review and transaction-matching status record, not a conclusion that the eight transfers settled or that any named recipient acted improperly.
