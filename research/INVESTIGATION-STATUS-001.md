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
