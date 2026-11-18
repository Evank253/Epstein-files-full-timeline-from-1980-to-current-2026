# Investigation status — 2026-11-17

## Initial work
- Chronology: 33 preliminary events, 1980–November 2026.
- Relationship graph: 34 entity nodes and 23 typed edges.
- Evidence ledger: 15 evidence records.
- Source artifact register: 16 initial source locations.
- Timeline events and graph edges carry evidence IDs.

## Acquisition state
The 16 source locations are identified, not captured. No SHA-256 values or byte sizes are populated because the original files have not yet been acquired and hashed. The chronology is preliminary and uses public reports, court and regulator records; some underlying depositions, instruments, transaction schedules and signed docket orders remain to be obtained.

## Limitations
- A committee report summarizing testimony is not a substitute for the underlying deposition.
- A regulator's consent order is not proof that every person or entity mentioned committed a crime.
- Secondary docket reporting remains secondary until signed court orders are acquired.
- Production page counts are not unique-document counts.
- A name appearing in a list or file does not establish wrongdoing.
- Missing, sealed, withheld, inaccessible or unreviewed material is NOT_MEASURED / NOT_ESTABLISHED, not proof of absence or guilt.

## Next phase
Acquire lawful public originals; record retrieval metadata and SHA-256; extract exact page-level locators; reconcile duplicates without deleting source copies; independently verify material claims; then extend chronology, relationship graph, financial reconstruction and international leads. Protect victim and witness identities throughout.


## Newly developed findings — Bear Stearns document family (2026-11-17)

**Label:** NEWLY DEVELOPED FINDING — independent research lead; not a determination that the information was absent from all DOJ/FBI investigative files.

- `EVT-038`: extracted subpoena record `EFTA00193068` names Bear Stearns Companies Inc. as custodian recipient. Reported identifier `EFTA00186986` remains unresolved against it.
- `EVT-039`: extracted correspondence record `EFTA00189874` appears to ask a Bear Stearns contact for additional Epstein-related entity and role information.
- `EVT-040`: page 32/59 of parent document `EFTA00187050` (printed Bates `EFTA00187080`) contains a September 7 2007 response on Bear, Stearns & Co. Inc. letterhead representing that a personnel file and CD of statements for Epstein and six named accounts were supplied.

**Evidence links:** `EVD-016`–`EVD-018`; claims `CLM-016`–`CLM-018`; source artifacts `ART-017`–`ART-020`.

**Acquisition status:** No original source files or CD contents were acquired in this update. No source-file SHA-256, byte size, or MIME type is asserted. Third-party extracted text is not original-page verification.

**Interpretation limits:** Do not merge Bear Stearns Companies Inc. with Bear, Stearns & Co. Inc. Do not merge subpoena identifiers EFTA00186986 and EFTA00193068. The six account labels do not establish beneficial ownership, legal form, signatory authority, balances, transfers, or wrongdoing. Novelty relative to the complete DOJ/FBI investigative record is NOT_ESTABLISHED until a systematic comparison is completed.

**Next acquisition/examination tasks:** obtain original PDFs for EFTA00186986, EFTA00193068 and EFTA00189874; compare Bates identifiers and attachments; inspect EFTA00187050 page image; locate the referenced CD and follow-up productions; identify legal entities and account authority from primary records.


## Correction and expanded primary-source lead — EFTA00193068 page family (2026-11-17)

**Correction to earlier entry:** EFTA00193068 is not a standalone subpoena document. The index identifies it as a 131-page parent production, Bates span EFTA00193068–EFTA00193198. Within that parent:
- Bates EFTA00193096 (page 29/131) is the OLY-71 subpoena addressed to Custodian of Records, Bear Stearns Companies Inc., with September 4, 2007 appearance/return date.
- Bates EFTA00193098 (page 31/131) is the attachment to subpoena, Bear Stearns Companies Inc., requesting documents concerning Epstein, including accounts owned or managed by him and employment records.
- Bates EFTA00193099–EFTA00193101 contain a business-record certification and inventory pages.
- Bates EFTA00193108 (page 41/131) is an August 15, 2007 letter to Dennis Block. Its extracted text states the subpoena was addressed to the parent corporation Bear Stearns Companies but was meant to include subsidiary Bear, Stearns & Co. Inc.; it offers a separate subpoena for that entity if requested.

**Effect:** The corporate-entity question is materially clarified as to the prosecutor's stated intended subpoena scope. Do not continue describing the parent/subsidiary relationship as wholly unexplained. However, which entity actually searched for, held, controlled, certified, or produced each record still requires custodian certification, inventories, production records, and original scans.

**New timeline item:** EVT-041; claim CLM-019; evidence EVD-019; source artifact ART-021; graph edges REL-033–REL-035.

**Acquisition limitation:** DOJ direct PDF access was blocked by age-verification redirect in the browsing route and a direct download attempt failed. The present examination is based on page-level extracted text hosted by a third-party index. No original PDF bytes, page images, SHA-256, or file size are claimed. The index explicitly warns OCR may contain errors. Original scan verification remains mandatory.

## Newly developed external-account and AML review leads (2026-11-17)

- **EVT-042 / EFTA00189874 (Aug. 27, 2007):** extracted text lists eight Epstein-related entity names known to the AUSA, requests additional CEO/COO or sole-owner/shareholder entities, and asks for accounts at other financial institutions to/from which Bear transferred or received funds on Epstein's behalf. The hosted extract truncates. Names are prosecutor-listed leads, not verified ownership. No external institution/account identified yet.
- **EVT-043 / EFTA00189877 (Sept. 6, 2007):** follow-up asks for the external-account list and production status; cites meeting-record periods July 2004, March 2005, April 2005, September 2005 and October 2005. These are request periods, not transaction dates. No Bear response/list located.
- **EVT-044:** 2023 USVI v JPMorgan party filing, Document 285-2 ¶¶171–177, describes a Bear review of accounts maintained for Epstein's benefit focused on outgoing $1,000/$100,000 transfers and quotes a limited conclusion. It cites Exhibit 125, JPM-SDNYLIT-00373075/-00373076. This is not the original Bear memo or a judicial finding; scope is not a comprehensive audit.
- **EVT-045:** same filing ¶¶173–175 describes 2011 JPMorgan emails locating the 2007 Bear subpoena file; cites Exhibits 127/128. Underlying emails not acquired.

Added EVT-042–045, CLM-020–022, EVD-020–022, ART-022–024. Graph now contains eight prosecutor-listed entity-name reference nodes plus David Petercsak and Arthur Middlemiss; their roles and relationships retain explicit qualification. Next priority: acquire EFTA00189874/877 originals, Bear's response and external-account schedule, Exhibit 125 and Exhibits 127/128. Then identify actual counterpart institutions and trace settled transactions using statements/wire records from both sides. Original bytes/images and SHA-256 remain NOT_ACQUIRED / NOT_MEASURED for these new records.


## Evidence correction — Bear review characterization (2026-11-17)

A source-level recheck identified an overstatement in the earlier EVT-044 / EVD-022 description. The relevant publicly accessible filing is the USVI Statement of Material Facts, S.D.N.Y. Document 246, filed July 26, 2023 (not Document 285-2). Paragraphs 171–177 cite a sealed JPMorgan-produced Exhibit 125 (Bates JPM-SDNYLIT-00373074–00373076). Paragraph 173 says Arthur Middlemiss was Bear's AML Officer responsible for responding to the 2007 subpoena. Paragraph 174 quotes a January 10, 2011 email from Ryan to Langford, DeLuca and Nichols recalling that the AUSA correspondence concerned “something about $1000 and $100,000 transactions.” The public filing does not establish that Bear applied those amounts as review thresholds, conducted a particular review, or concluded that no suspicious wires existed. The earlier statement about Bear screening outgoing transfers and finding no suspicious/unusual wires is withdrawn as unsupported by the cited public record.

EVT-044 now records only the filing and its citation to sealed Exhibit 125. EVT-045 is corrected to January 10, 2011 and describes the quoted employee email as a recollection of the AUSA request. REL-046, which represented a Bear review relationship, has been removed. EVD-022 and ART-024 have been corrected; CLM-023 records the corrected proposition. Exhibit 125 remains sealed/not acquired, and Exhibit 127 has not been acquired in this examination.


## Additional primary-source locator — EFTA00189873 (2026-11-17)

A separate August 15, 2007 USAO letter, EFTA00189873, is now identified. Extracted text states the subpoena addressed to Bear Stearns Companies Inc. as parent was intended to include Bear, Stearns & Co. Inc. as subsidiary; a separate subpoena could be issued if requested. It further states that custodian testimony would not be required if the custodian completed the attached records certification. This adds a concrete certification pathway to the response investigation, but does not prove a separate subpoena was issued, that certification was completed, or which entity searched/produced records. Added EVT-046, EVD-023, CLM-024, ART-025 and graph links for Dennis Block and Cadwalader as letter addressee/address-block affiliation only. DOJ primary PDF URL is identified, but original bytes/page image remain NOT_ACQUIRED and SHA-256 NOT_MEASURED. The September 6 letter EFTA00189877 also says Bear expected to have some documents ready to produce and asks when the external-institution account list would be available; this is a request/status exchange, not proof production occurred.

## Exhibit-access correction

The July 25, 2023 Mimi Liu declaration, S.D.N.Y. Document 245, identifies Exhibit 125 (JPEM-SDNYLIT-00373074–00373076) as filed under seal, but states Exhibit 127 (JPM-SDNYLIT-00157192–00157193, Jan. 10, 2011 email) had its confidentiality designation withdrawn while original redactions remained. Therefore Exhibit 127 is not accurately described as sealed; it is publicly filed with retained redactions, although its actual pages have not yet been acquired/examined in this research session. Exhibit 125 remains sealed. Source locator: https://www.plainsite.org/courts/new-york-southern-district-court/government-of-the-united-states-virgin-islands-v-jpmorgan-chase-bank-na/4zrtycivz/2xku8xo5td/ (PDF pages 16–17 of the declaration).


## Financial-record expansion — International Charitable Interests statement family (2026-11-17)

Located five additional Bear Stearns statement records indexed under International Charitable Interests: EFTA00198828 (5 pages; Nov. 30-Dec. 31 2002 extract identifies Financial Trust Co Inc TTEE, account executive Ira Zicherman, net credit balance about $9.449m); EFTA00199832 (171 pages; period through May 31 2002, extract reports net equity $20,586 to zero); EFTA00200535 (15 pages; extract describes a repurchase agreement beginning June 19 2001, open purchase price/principal $2,151,602.86); EFTA00198769 (59 pages; extract reports net equity about $74,220); EFTA00198956 (64 pages; extract reports net equity about $27.342m). These are statement leads, not reconstructed transfers. OCR and date/amount fields require original image inspection; no source bytes/hash or transaction pages examined. Added EVT-047–051, EVD-024–028, CLM-025–029, ART-026–030 and graph nodes/edges for the account label, trustee designation and named account executive. The account label is not treated as a legal entity or proof of beneficial ownership. The $20,586-to-zero balance change is not treated as a transfer; repurchase agreement is not treated as external-bank payment.

## Further source correction / discovery

EFTA00189877's complete extracted text says Bear had told the AUSA it expected some documents to be ready to produce around that time, and the AUSA asks when the external-institution list will be available. This establishes an expected production/status conversation, not actual delivery of the external-account schedule. The 2023 JPMorgan response document EFTA02815288 (S.D.N.Y. Document 284-3, filed Aug. 14 2023) states that JPMorgan undisputed the quoted Jan. 10 2011 email in Exhibit 127 but disputed the inference drawn from it. Paragraph 173 attributes the 2007 subpoena response responsibility to Middlemiss by reference to Exhibit 125; paragraph 174 quotes Ryan's recollection that prosecutors were interested in something about $1,000 and $100,000 transactions. Paragraph 178 separately cites a chart of twenty $100,000 transfers from Epstein accounts between Jan. 2 and Oct. 12 2007 (Exhibit 63 at -655 to -660), while JPMorgan disputed the assertion that the email established a contemporaneous JPMorgan investigation. These are separate evidence propositions: do not conflate Bear's 2007 subpoena scope, the 2011 recollection, and the 2007 JPMorgan transfer chart. Acquire the cited original exhibits before asserting transaction-level links.


## Transaction-level cross-bank lead — JPMorgan 2007 spreadsheet (2026-11-17)

A publicly accessible copy of S.D.N.Y. Document 174-1, Exhibit 1, contains a JPMorgan transaction spreadsheet attachment at Bates JPM-SDNYLIT-00269655–00269660 (PDF pages 6–9 of the public 29-page exhibit copy). The Oct. 19 2007 email introducing the workbook says it lists Private Bank entities in Epstein's relationship with current balances and related DDR information, and separately attaches “Epstein 2007 transactions.xls” for 2007 transaction activity >=$50,000. The court's Document 284-3 ¶178 cites Exhibit 63 at -655–60 and states that twenty transfers in the amount of $100,000 were made from Epstein accounts Jan. 2–Oct. 12 2007; JPMorgan disputes that the email proves its broader legal inference about an investigation. The visible spreadsheet rows are not all $100,000 and include credits as well as debits. The paragraph's characterization must therefore be reconciled against the complete workbook, not treated as a complete transcription.

Visible examples include: 2007-09-06 $6.5m CHIPS debit via Citibank to Bear Stearns & Co with Epstein named beneficiary; 2007-09-25 $100k CHIPS debit via Citibank to Bear Stearns & Co with beneficiary redacted; 2007-09-17 $100k Fedwire debit via Sovereign Bank to Martin G. Weinberg PC IOLTA; 2007-10-11 and 2007-09-10 $100k CHIPS debits via HSBC Bank USA to Gerald B. Lefcourt PC IOLA; 2007-10-03 $90k book-transfer debit naming Bank of Nova Scotia, St Thomas; multiple FirstBank Puerto Rico debits to LSJ LLC/Lafayette Contractors LLC; and repeated Mellon Bank credits described as on behalf of Financial Trust Company with Epstein as beneficiary. These entries are recorded as visible spreadsheet claims, not independently settled transfers. Account numbers and some beneficiaries are redacted. Added EVT-052, EVD-029, CLM-030, ART-031 and bank-rail graph references.

## Statement extract corrections / details

EFTA00198828's extract explicitly identifies statement period Nov. 30–Dec. 31, 2002, account executive IRA ZICHERMAN, International Charitable Interests DTD 08/30/94 and Financial Trust Co Inc TTEE. It reports market value $9,460,332 and net credit balance $9,449,358 (not simply a single $9.46m value). EFTA00199832's extracted date string for the period is internally inconsistent/garbled (appears “11/27/2002 through May 31, 2002”); retain the balance change ($20,586 to zero) as OCR-extracted but do not assign a start date until scan review. EFTA00198956 reports net equity $27,342,121 and prior net equity $27,308,915; EFTA00198769 reports $74,220 and prior $74,133. These remain extracted text, not original scan verification.


## Transaction trace correction and expanded row transcription (2026-11-17)

Direct review of public Document 174-1 Exhibit 1 shows the Oct. 19 email at PDF p.2 identifies attachment "Epstein 2007 transactions.xls.zip" and says it covers 2007 transaction activity >=$50,000. Transaction rows are visible on PDF pp.6–9. Examples include: 2007-09-06 $6.5m CHIPS debit via Citibank naming Bear Stearns & Co and Jeffrey Epstein as beneficiary; 2007-09-25 $100k CHIPS debit via Citibank naming Bear Stearns & Co with beneficiary redacted; 2007-09-17 $100k Fedwire debit via Sovereign Bank to Martin G Weinberg PC IOLTA; 2007-10-11 and 2007-09-10 $100k CHIPS debits via HSBC to Gerald B Lefcourt PC IOLA; 2007-09-11 $100k and 2007-09-06 $50k FirstBank PR Fedwire debits to LSJ LLC; 2007-10-02 and 2007-08-23 $75k FirstBank PR debits to Lafayette Contractors LLC; $7,508,968.68 Aug. 29 Fedwire credit via Wachovia with Island Fund 1 LLC as originator and Epstein as beneficiary; and multiple $1m Mellon Bank Fedwire credits with Financial Trust Company as B/O and Epstein as beneficiary. Other visible rows include payments to Kirkland & Ellis and Black Srebnick.

This is a JPMorgan spreadsheet copy attached to an internal email, not a native workbook or independent receiving-bank confirmation. Some entries are credits into the JPMorgan account, not outflows. Account numbers and other fields are redacted. The court's statement in Document 284-3 ¶178 that the workbook included twenty $100,000 payments is a separate claim; this register is a partial transcription and does not yet reconcile all twenty rows. Do not describe all entries as $100,000 or as external outflows. See updated JPM-TRANSACTION-TRACE-001.csv and corrected EVD-029/CLM-030.


## High-value transaction leads added (2026-11-17)

Added six additional rows to JPM-TRANSACTION-TRACE-001.csv. Highest priority is a May 29 2007 $12,976,977.85 Fedwire debit via Wachovia to Island Global Yachting Ltd; the reference field says purchase of an interest in American Yacht Harbor. This is a strong document lead for a specific asset/acquisition inquiry, not proof of title or completed settlement. Other rows include an Oct. 1 $2.5m book-transfer credit with National Financial Services LLC and originator Alan M. Dershowitz; a Sept. 26 $1m Mellon credit with Financial Trust Company as B/O and Epstein as beneficiary; Sept. 20 debits of $227,158.57 to Worth Builders of Palm Beach, $53,337.65 book transfer to JP Molyneux Studio Ltd and $74,155 to Maguire Group Inc. Added EVT-053, EVD-030, CLM-031 and graph references. All are spreadsheet-level leads; counterpart records and settlement remain unverified.


## American Yacht Harbor cross-source ownership and payment examination (2026-11-17)

The May 29 2007 $12,976,977.85 JPMorgan spreadsheet debit to Island Global Yachting Ltd, reference "PURCHASE OF INTEREST IN AMERICAN YACHT HARBOR," now has two additional cross-source records. EFTA00611194 is a 12-page audited financial statement for IGY-AYH St. Thomas Holdings LLC. Its notes state the company was formed as a wholly owned subsidiary of Island Global Yachting Ltd on Dec. 5 2006, acquired American Yacht Harbor on Jan. 18 2007, and sold a 50% passive member interest to one of the parent's investors on May 29 2007. It does not name the investor. EFTA01134866 is a February 2014 revised draft settlement agreement. It recites that Epstein and Island Global Yachting Facilities Ltd entered a May 29 2007 Membership Interest Purchase Agreement under which Epstein purchased a 50% membership interest in IGY-AYH; it also recites a dispute about purchase price and management/fees. This draft is not an executed agreement or proof of final payment, but it independently names Epstein in connection with the 50% interest. Together, the audited statements, draft recitals and JPM spreadsheet reference align the date, percentage and payment purpose. Treat as strong cross-source alignment, not fully verified title/payment settlement until executed membership agreement, signed LLC agreement, wire confirmation and membership ledger are acquired.

EFTA00594382 separately records the Jan. 18 2007 acquisition of American Yacht Harbor by IGY-AYH from MOF VI Limited Partnership for stated purchase price $25.5m. Do not conflate the Jan. 18 marina acquisition with the May 29 purchase of a 50% membership interest in the holding company. Added EVT-054, EVD-031–033, CLM-032–034, ART-032–034 and graph relationships. Original PDF bytes/page images and hashes not acquired in this examination.

