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

