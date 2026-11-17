# Financial evidence leads — Southern Trust, Deutsche Bank and Plan D — 001

**Research date:** 2026-11-17  
**Source family:** DOJ EFTA production as reproduced in the independent corpus  
**Status:** Targeted secondary-text review. Original DOJ PDF bytes have not yet been acquired or hashed in this review.  
**Destination:** Epstein investigation repository only.

## Executive finding

Targeted discovery surfaced a cluster of financial records that can support a much more specific reconstruction of Southern Trust Company, Plan D LLC, HBRK Associates and Deutsche Bank relationships. The strongest immediate records are:

- EFTA00624906–EFTA00624908: Southern Trust invoice and adjacent Plan D promissory-note pages concerning Leon Black.
- EFTA01449196: email chain discussing a prospective $1 million wire to Southern Trust and providing Deutsche Bank wire instructions.
- EFTA01417964: 41-page Deutsche Bank email/EDD package concerning Southern Financial LLC, including AML compliance staff.
- EFTA01359500, EFTA01381149, EFTA01381246, EFTA01431991 and EFTA01477454: bank roster, balance and banker-assignment records identified in independent report indexes.
- EFTA00167059 and EFTA00168930: Deutsche Bank KYC records associated with Prytanee LLC and an art-investment structure.

These records are leads for financial reconstruction, not proof that every proposed, invoiced or instructed transfer settled.

## 1. EFTA00624906–EFTA00624908 — Southern Trust invoice and Plan D note

A 3-page reproduced PDF contains consecutive EFTA identifiers.

### Page/document EFTA00624906
- Southern Trust Company, Inc. invoice dated March 27, 2017.
- Addressee: Leon Black, c/o Elysium Management LLC.
- Amount: $10,000,000.
- Stated basis: “Amount due pursuant to Agreement Between Southern Trust Company, Inc. and Leon Black.”
- Requests payment by electronic wire transfer.
- The invoice's bank/ABA/account fields are blank in the reproduced text.

### Page/document EFTA00624907
- Promissory note dated March 27, 2017.
- Maker: Plan D LLC, a U.S. Virgin Islands LLC.
- Holder/payee: Leon Black.
- Principal: $28,500,000.
- Interest: 1.01% per annum.
- Maturity: March 26, 2018.
- Signature block identifies Jeffrey Epstein as Plan D LLC's sole member; the reproduced PDF's visual description identifies a handwritten signature and notarial acknowledgment.

### Page/document EFTA00624908
- Continuation of the promissory note's terms.

**Critical distinction:** The $10 million invoice and $28.5 million note are separate instruments appearing on consecutive EFTA pages in the same reproduced PDF. The invoice is a payment demand/receivable claim, not proof of payment. The note evidences a written debt instrument in the reproduced record, not proof of disbursement, repayment, default, forgiveness, or ultimate economic beneficiary. Do not combine the two amounts or infer a $38.5 million transfer.

Secondary PDF text source: https://epstein-data.com/pdf/EFTA00624906.pdf  
Original DOJ URL candidate (dataset mapping must be checked against the actual DOJ file response): https://www.justice.gov/epstein/files/DataSet%208/EFTA00624906.pdf

## 2. EFTA01449196 — expected $1 million wire to Southern Trust

The independent viewer's rendered text contains a September 13, 2013 email chain:
- Deutsche Bank associate Amanda Kirby supplies wire instructions for Southern Trust Company, Inc. at Deutsche Bank Trust Company Americas.
- Richard Kahn of HBRK Associates writes that they were expecting a $1,000,000 wire to the account “either today or this week” and asks whether it had arrived or was in process.
- The chain carries Deutsche Bank and SDNY production stamps.

**Classification:** contemporaneous email evidence of wire instructions and an expected transfer. It does not establish the sender account, actual debit, bank settlement, final credit, purpose, or ultimate source of the funds. It may be possible to identify the actual transfer in adjacent bank ledger/wire records; search for the exact amount, date window, originator, beneficiary account and transaction reference without exposing account numbers.

Secondary viewer: https://epstein-data.com/EFTA01449196  
Original DOJ URL candidate: https://www.justice.gov/epstein/files/DataSet%2010/EFTA01449196.pdf

## 3. EFTA01417964 — Deutsche Bank EDD package for Southern Financial LLC

The independent viewer search result identifies a 41-page email/document package with subject:
“RE: EDD package for the RID: ONB-120902 Southern Financial LLC”

A January 15, 2015 message from Deutsche Bank AML Compliance Officer Dmitri Saks states that he had not been notified of further developments in the case. The package includes account-opening and AML staff correspondence.

**Classification:** bank compliance correspondence / enhanced due diligence record. The single exposed message does not establish the package's final outcome, whether account opening was approved or rejected, which deficiencies were resolved, or whether any suspicious activity report was filed. Review the full 41 pages and associated documents before drawing a conclusion.

Secondary viewer: https://epstein-data.com/EFTA01417964  
Original DOJ URL candidate: https://www.justice.gov/epstein/files/DataSet%2010/EFTA01417964.pdf

## 4. EFTA01359500 and related Deutsche Bank records — account roster and balances

Independent research indexes identify the following records as relevant:
- EFTA01359500 — Deutsche Bank internal account-management roster.
- EFTA01381149 — bank balance record dated August 17, 2018 according to third-party index metadata.
- EFTA01381246 — bank balance record dated June 21, 2018 according to third-party report index.
- EFTA01431991 — consolidated balance record.
- EFTA01477454 — banker assignment record.

Independent analytical reports describe common Deutsche Bank relationship personnel assigned to accounts for Jeffrey Epstein and multiple corporate/trust entities, and also mention other bank clients. Those are third-party interpretations of bank documents. They must not be copied into the primary evidence ledger as established facts until each original page is inspected and the exact field/roster context is recorded.

### Specific verification questions
1. Does EFTA01359500 actually list each entity and named officer in the same table/relationship roster?
2. Are the listed officer roles primary, secondary, historical, or merely contact assignments?
3. Do the balance reports state ledger balance, available balance, market value, or another measure?
4. Are balances individual account snapshots, aggregated entity totals, or consolidated relationship totals?
5. Does EFTA01431991 reconcile to the earlier snapshot records, or is it a different reporting basis/date?
6. Does EFTA01477454 cover the same customer relationship and period as EFTA01359500?
7. Do bank ledger and wire records show actual flows between the accounts, as distinct from common management?

Do not sum balances across dates or entities without checking whether accounts are duplicates, subaccounts, trust interests or consolidated totals.

## 5. EFTA00167059 and EFTA00168930 — Prytanee LLC KYC

Independent sources identify these as Deutsche Bank KYC records associated with Prytanee LLC and an art-investment relationship. A third-party report describes a 50/50 ownership structure involving Southern Trust Company and another trust, and a manager/signatory structure.

**Handling:** the KYC file includes personal information. Do not reproduce personal addresses, dates of birth, signatures, personal contact information, tax IDs, account numbers or other sensitive identifiers. For the financial reconstruction, extract only necessary entity-level facts: legal entity, jurisdiction, account-opening date, stated ownership percentages, stated business purpose, authorized signatory roles and the exact page/document where each field appears. Record whether each field is legible in the original page image or only in OCR.

**Classification:** KYC statements are customer-provided or bank-recorded representations, not independent proof that the underlying ownership or source-of-wealth claims were true.

## 6. Financial reconstruction model

For each transaction candidate, maintain separate fields:
- transaction_id (internal stable ID)
- source_document_id and exact page
- document date and asserted transaction date
- originator name/entity (as stated)
- originator bank/account (masked in public register)
- beneficiary name/entity (as stated)
- beneficiary bank/account (masked in public register)
- amount and currency
- transaction type (wire, internal book transfer, invoice, note, fee, distribution, reimbursement, unknown)
- status (proposed, instructed, expected, initiated, settled, reversed, returned, disputed, unknown)
- source of status assertion
- bank confirmation/ledger reference
- related agreement/invoice/note
- corroborating and contradictory documents
- privacy review status
- verification status

Never treat these as interchangeable:
- invoice ≠ payment;
- wire instructions ≠ wire initiation;
- expected wire ≠ settled transfer;
- promissory note ≠ disbursement;
- account balance ≠ income or profit;
- common banker ≠ common ownership;
- KYC ownership representation ≠ verified beneficial ownership;
- related entities ≠ commingled assets.

## 7. Priority acquisition/verification queue

| Priority | EFTA | Target | Required verification |
|---|---|---|---|
| 1 | EFTA00624906–08 | Southern Trust invoice and Plan D note | Original pages, signatures, agreement referenced by invoice, payment and note funding/repayment records |
| 1 | EFTA01449196 | Expected $1m wire | Original email page, surrounding thread, bank wire/ledger evidence, actual settlement |
| 1 | EFTA01417964 | Southern Financial EDD package | All 41 pages, decision/outcome, linked KYC/EDD records, any remediation |
| 2 | EFTA01359500 | Deutsche Bank account roster | Original table/image, officer roles, full account scope |
| 2 | EFTA01381149 / 01381246 / 01431991 | Balance reports | Exact dates, balance definitions, account-level reconciliation |
| 2 | EFTA01477454 | Banker assignment record | Original roster, effective dates, exact scope |
| 2 | EFTA00167059 / 00168930 | Prytanee KYC | Entity-only fields, page-image verification, account and ownership corroboration |

## 8. Source and legal-status caution

- Third-party corpus viewers and OCR are discovery aids. DOJ originals remain the source of record.
- Civil complaints and party submissions contain allegations, not findings.
- A document appearing in a DOJ production does not authenticate every assertion in it.
- Avoid inference of criminality from account proximity, common bankers, business relationships or shared addresses.
- Protect victims and private individuals; do not publish unnecessary personal information.
- No bank account numbers or personal identifiers are reproduced in this report.

## 9. Current state

This report records source leads and a transaction-verification plan. It does not claim that the original DOJ PDFs were acquired or hashed. No wire settlement, invoice payment, promissory-note funding/repayment, or final ownership/distribution has been independently verified in this review.
