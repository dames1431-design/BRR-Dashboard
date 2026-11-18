# BRR Procurement Watch: Daily Report, 2026-11-18 (Central Time)

Run 1. This is the baseline run: the watch did not exist before today, so every item released more than three days ago is logged as a miss under the miss taxonomy, with a root cause and a control change. Full detail is in the ledgers; this report is the control surface.

## DISCOVERY CONTROL
```
Priority direct sources checked (opened on official page):   0 / 44
Priority direct sources search-snippet checked:              13 / 44
Sources inaccessible today (network allowlist):              24 / 44
Sources not checked (search budget exhausted):                7 / 44
New releases found by direct checks (released 11/04-11/18):   1   (Des Moines RFP1286-A, 11/12)
New releases found by fresh discovery (released 11/04-11/18): 2   (Ohio After School FY28 RFA 11/16; CES DYS03CES 11/12)
Active items found with older or unknown release dates:      33
Coverage misses discovered:                                  16
High-severity misses (found after an early mandatory gate):   1   (Region 9 / NMPED RFP 27008)
Serious misses (found after final deadline):                 11
Earliest newly found release:                                2026-11-16
Oldest newly found release still open:                       2026-10-16 (Newark nonpublic tutoring)
Six-month forecast trigger groups searched:                   7 of 9 (foundations/IES and networking events not run)
Known upcoming releases currently tracked (forecast ledger):  45
Direct-source lane complete:                                  NO
Fresh-discovery lane complete:                                NO  (8 of 52 planned sweeps did not run)
```
Because neither lane completed, this report makes no "no new opportunities" statement for any source. The statement that can be made: across the sources named in Section A, three releases dated inside the backfill window were found, plus thirty-three active items with older or unknown release dates.

### Why the lanes did not complete, and what changed today
1. The session's network policy allowed only seven hosts, none of them procurement portals. Every fetch of cps.bonfirehub.com, cps.edu, cpsboe.org, bidbuy.illinois.gov, isbe.net, txsmartbuy.gov, tea.bonfirehub.com, houstonisd.ionwave.net, eva, emma, infohub.nyced.org, philasd.org, detroitk12.org, michigan.gov, education.ohio.gov, sam.gov and the aggregators was refused at DNS. Evidence is therefore search-engine snippets of official pages, capped at PARTIALLY VERIFIED, except one document that was opened in full (Region 9 RFP 27008).
2. Control change: a BRR-Dashboard environment was created with forty procurement hosts allowed. The change had not propagated to this machine by the time of this report; the next run should open each roster URL directly.
3. The shared web-search budget (200 queries per turn across six lanes) ran out before Connecticut, Louisiana, Alabama, Mississippi, California, Nevada, Arizona, Colorado, Washington, Oregon, Utah, Oklahoma, Kansas, Nebraska, SAM.gov, tribal/BIE, Head Start second pass, library second pass, Texas ESC regions, foundations/IES and networking events were searched. Control change: the next run splits the direct lane into eight regional lanes run on separate turns.

## A. Source accountability
Status per named source is in `source_roster.csv` (columns last_checked, status_last_run, last_change_seen). Summary by status:

| Status | Count | Sources |
|---|---|---|
| INACCESSIBLE (network), search snippets used | 24 | CPS Bonfire, CPS procurement, CPS Board, BidBuy, ISBE RFSP, MPS procurement, ESBD, TEA Bonfire, HISD IonWave, Dallas ISD, ESC Region 4, Choice Partners, TIPS, eVA, eMMA, NYC DOE infohub, PASSPort, City Record, Hillsborough, Miami-Dade, FDOE, DC OCP, COMMBUYS, SAM.gov, BidNet |
| SEARCH-CHECKED (official-domain snippets reviewed; page not opened) | 13 | MDE grants, DPSCD (aggregator mirror), Baltimore City, Philadelphia, PA eMarketplace, Ohio DEW, Columbus, Broward, Orange, Duval, Atlanta, Memphis-Shelby, Newark |
| NOT CHECKED (search budget) | 7 | VendorNet/DPI (partial), SIGMA, Cleveland, NOLA, LAUSD, Clark County, Denver |
| Discovery/forward rows | 6 | OpenGov (site query), Bonfire site query, DemandStar, cooperatives (partial), suburban Chicago boards (not run), BidNet (blocked) |

Forty new roster rows were added today from source-expansion candidates and miss root causes (SRC-051 to SRC-090).

## B. New or active items, sorted by release date, newest first
Scores are Fit / Revenue / Ease / Time-to-action on 1-5, kept separate by rule.

| Opp | Issuer | Title | Release | Due (local / Central) | Stage | Confidence | Parcel and route | Prob | F/R/E/T |
|---|---|---|---|---|---|---|---|---|---|
| OPP-001 | Ohio DEW | Ohio After School (21st CCLC) FY28 Cohort A RFA | 2026-11-16 | 12/28 11:59 PM ET / 10:59 PM CT | grant | PARTIALLY VERIFIED | Literacy partner in an Ohio LEA/CBO application; sub/MOU | MEDIUM | 4/3/3/4 |
| OPP-002 | Des Moines PS | RFP1286-A Gr 9-12 ELL Curriculum and Implementation Support | 2026-11-12 | 12/24 (CT) | released | DISCOVERY LEAD | Implementation PD sub to publisher; thin | LOW | 2/2/2/4 |
| OPP-003 | Collaborative for Educational Services (MA) | DYS03CES Teacher Staffing, DYS/SEIS | 2026-11-12 | not shown | released | DISCOVERY LEAD | Juvenile-justice literacy staffing; lead toward CES PD buys | LOW | 2/2/2/3 |
| OPP-004 | Region 9 REC for NMPED | RFP 27008 K-3 Screening, Diagnostic, Progress Monitoring | 2026-10-23 | 11/20 3:00 PM MT / 4:00 PM CT | released | VERIFIED (RFP opened) | Component D statewide training as named sub to an assessment prime; prime not viable | LOW | 3/4/1/1 |
| OPP-005 | Pittsburgh PS | RFP-2026-0014 K-5 Literacy Universal Screening and Decision-Support System | 2026-10-21 (notice says docs 10/30) | 11/23 (ET; time not shown) | released | PARTIALLY VERIFIED | PD/coaching and comprehension-assessment sub to platform vendor | LOW | 2/3/2/5 |
| OPP-006 | Newark BOE | Nonpublic pull-out ELA/Math tutoring K-12 | 2026-10-16 | UNKNOWN | released | DISCOVERY LEAD | Prime, Intellectual Child LLC; Title I nonpublic core lane | MEDIUM | 5/2/3/5 |
| OPP-015 | TEA | PASS approved literacy tutoring provider | 2026-09-17 (notice) | rolling | vendor pool | PARTIALLY VERIFIED | Prime; K-3 tutoring billed to $400 family accounts | MEDIUM | 5/2/3/4 |
| OPP-026 | Bound Brook SD (NJ) | PD (Literacy 2-6) yearlong PD + coaching | 2026-09-28 | unknown (may be open) | released | DISCOVERY LEAD | Prime, Intellectual Classroom | MEDIUM | 5/2/3/4 |
| OPP-008 | ESC Region 7 (TX) | ICAT2628 Instructional Catalog Discount Bid | not shown | 11/19 1:30 PM CT | released | DISCOVERY LEAD | Catalog vendor, Intellectual Classroom; est. $30-35M aggregate, 2 yrs | LOW | 4/3/3/5 |
| OPP-009 | Humble ISD | RFP 2027-101 Instructional Materials pool | not shown | 12/07 per one aggregator; CONFLICT | vendor pool | DISCOVERY LEAD | Materials, Intellectual Classroom | MEDIUM | 4/2/4/4 |
| OPP-010 | Unnamed TN district (EdWeek 11/17) | Instructional vendor library | not shown | 12/10 | vendor pool | DISCOVERY LEAD | Pool placement | MEDIUM | 3/2/3/4 |
| OPP-007 | Baltimore City PS | ESSA Title I Educational Services for Eligible Non-Public Students | not shown | UNKNOWN | released | DISCOVERY LEAD | Prime, Intellectual Child LLC | MEDIUM | 5/3/3/4 |
| OPP-011 | Massachusetts DESE | 25MACISMB1 Early Literacy Tutoring Master Agreement | not shown | 12/31 (ET) | vendor pool | DISCOVERY LEAD | Statewide tutoring list, prime | MEDIUM | 5/3/3/3 |
| OPP-012 | NYC DOE | Literacy PD and Coaching MTAC (standing) | standing | 12/31 per aggregator | vendor pool | DISCOVERY LEAD | PD vendor enrollment; Intellectual Classroom or Dr. Dames | MEDIUM | 5/3/2/3 |
| OPP-013 | Fort Worth ISD | Academic/Educational Consultants and PD | not shown | 2027-01-29 CT | released | DISCOVERY LEAD | PD/coaching pool, prime | MEDIUM | 5/3/3/3 |
| OPP-014 | Arlington ISD | 27-06 Academic Educational Consultants and PD | not shown | 2027-06-01 2:00 PM CT | released | PARTIALLY VERIFIED | Annual qualifying list, prime | MEDIUM | 5/2/4/2 |
| OPP-016 | TEA | HB 1416 Ratio Waiver List 2027-28 window | likely open now | ~mid-Dec (prior year 12/12) | vendor pool | DISCOVERY LEAD | Tutoring product listing | MEDIUM | 4/2/3/4 |
| OPP-017 | Virginia DOE | High-Quality Tutoring provider approval (quarterly) | recurring | cycle dates unconfirmed | vendor pool | PARTIALLY VERIFIED | K-8 reading tutoring approval | MEDIUM | 5/2/4/3 |
| OPP-018 | Tennessee DOE | RFA ESA Service Providers FY2027 | not read | not read | vendor pool | PARTIALLY VERIFIED | ESA provider (parent-paid) | MEDIUM | 4/2/4/4 |
| OPP-019 | Missouri DESE | HDT Literacy Tutoring Qualified Vendor List | not shown | not shown | vendor pool | DISCOVERY LEAD | QVL placement feeding SLPS/KCPS | MEDIUM | 4/3/3/3 |
| OPP-021 | Youngstown CSD (OH) | Title I Services for Nonpublic Schools 2026-27 | not shown | not shown | released | DISCOVERY LEAD | Full nonpublic Title I delivery, prime | MEDIUM | 5/3/3/3 |
| OPP-022 | Milwaukee PS | 2026-27 Non-Public School Service Provider Selection | not shown | unknown | vendor pool | DISCOVERY LEAD | Approved Title I nonpublic provider (Mainstream history) | MEDIUM | 5/4/3/3 |
| OPP-027 | Wake County PSS | HDT training/coaching/implementation vendor | undated | undated | released | DISCOVERY LEAD | Teacher training for HDT literacy, Intellectual Classroom | MEDIUM | 5/3/3/3 |
| OPP-031 | NM PED | RFI: New Mexico Literacy Center | not shown | date not shown | RFI | DISCOVERY LEAD | Shape scope; Dr. Dames | MEDIUM | 4/2/4/3 |
| OPP-033 | Wayne RESA | WRESA-41-2025-2026-07 Instructional Capacity Building and CoP | not shown | not seen | released | PARTIALLY VERIFIED | PL design for coaching corps | MEDIUM | 3/3/3/2 |

Lower-probability active items (OPP-020, 023, 024, 025, 028, 029, 030, 032, 034, 035, 036) are in the ledger with the same fields. Closed-successor, award-pending and forecast-stage rows (OPP-037 to OPP-072) carry the successor route required by the no-silent-deletion rule.

## C. Material changes to previously reported items
None. Baseline run.

## D. Access gaps and alternates used
- Network: every official portal and every aggregator host was blocked (see Discovery Control). Alternate used: web-search snippets of official-domain PDFs and pages, plus aggregator snippets (Govly, Starbridge, SamSearch, Bid Banana, HigherGov, BidNet, CivicIQ, RFPSchoolWatch, governmentcontracts.us, michiganbids, EdWeek Market Brief). Per the evidence hierarchy, no aggregator item is above DISCOVERY LEAD until confirmed on the issuer page.
- Search budget: see the list above. The Texas lane ran 20 of 31 planned queries; Midwest left 16 verification queries unrun; East left Connecticut unchecked; South/West did not reach Louisiana, Alabama, Mississippi, California, the western states or SAM.gov; the discovery lane left 8 of 52 sweeps unrun; the forward lane left foundations/IES and networking events unrun.
- Login-dependent facts: Newark (EC Sourcing), Baltimore (eMMA), Hillsborough award (VendorLink), NYC (PASSPort), Humble/Cy-Fair/Fort Worth/Region 7 portals, ELC Miami-Dade portal, Ohio EDSteps eligibility, COMMBUYS. Each is flagged in the ledger.

## E. Coverage misses logged today
Sixteen rows in `ledgers/closed_miss_ledger.csv`. Each carries root cause, one concrete control change, and a successor route. The pattern: 7 of 16 are issuer omissions from the baseline roster (NM RECs, Pittsburgh, Iowa, juvenile-justice ESAs, early-childhood coalitions, NJ serial issuers, Idaho); 6 are portal-access blocks on rostered issuers (Newark, DESE/COMMBUYS, Baltimore/eMMA, Detroit, SAM.gov, Minneapolis); 2 are lane gaps (charter sweep, EdWeek alerts); 1 is a watch-did-not-exist baseline with a passed questions gate (Region 9). Control changes: 40 roster rows added, 40 hosts allowed, charter and juvenile-justice sweeps made weekly, EdWeek Market Brief alerts made a daily discovery source.

## F. Forward signals added to the forecast ledger
Forty-five rows in `ledgers/forecast_ledger.csv`, sorted by window. The nearest:
1. CPS consolidated Nov/Dec Board meeting, Thursday 2026-11-19: watch for OST RFQ 26-1224 awards and any literacy, tutoring, PD or nonpublic Title I actions. (FC-001)
2. ISBE 21st CCLC FY27 awards expected now through early 2027; CPS-partner nonprofits will subcontract OST literacy and arts residencies. (FC-002)
3. MDE 35a(2) ISD Early Literacy Coach grant opens in NexSys by end of November; 35m materials grant opens December. (FC-003, FC-004)
4. Minneapolis Title Services to Nonpublic Schools RFP is an annual November release; SY27 release may be imminent. (FC-006)
5. Polk County equitable-services RFP successor expected now through February. (FC-007)
6. Michigan PA 146 dyslexia compliance for 2027-28 and the 2026 M-STEP low (3rd-grade ELA 38.2%) put ISD PD buys in the December to June window. (FC-009)
7. NJ High-Impact Tutoring Cohort 4 NGO likely January to February 2027 with LEAs required to procure vendors. (FC-012)
8. NYC Reads middle-school completion by fall 2027 drives PD and MTSS partner selection January to June. (FC-016)
9. Detroit PSCD settlement-fund cliff forces replacement decisions February to June 2027. (FC-024)
10. CPS school-level tutoring buys during FY28 school budgeting, February to May, now that central Tutor Corps funding ended. (FC-022)

## G. Awards and subcontract routes
Seventeen rows in `ledgers/award_subcontract_ledger.csv`. Highest-value routes: Hillsborough 26111 pool awardees (unconfirmed list; verify on VendorLink or board records), Orange County pool (Catapult, One On One), Metro Nashville (Try Once, PENCIL), CPS Professional Learning pool vendors (locked to 5/31/2028; subcontract is the only route until then), NYC DYCD COMPASS lead CBOs, ISBE 21st CCLC FY27 grantees.

## H. Human-verification flags (within 7 days of a gate, with conflicting or missing information)
1. OPP-008 ESC Region 7 ICAT2628: due tomorrow 11/19 1:30 PM CT; aggregator-only; release date unknown. Decide today whether a catalog submission is feasible; otherwise log as declined with reason.
2. OPP-004 Region 9 / NMPED RFP 27008: due 11/20 4:00 PM CT; questions gate passed 11/03. Prime not viable; only route is an existing assessment-vendor relationship. If none, log as declined and pursue the awardee after 12/10 under the piggyback clause.
3. OPP-005 Pittsburgh RFP-2026-0014: due 11/23; release date conflicts (10/21 vs 10/30); time of day unknown; MBE goals unknown.
4. OPP-006 Newark nonpublic tutoring: due date unknown; opened 10/16; minimum five years Title I nonpublic experience. Open npssourcing.com today.
5. OPP-007 Baltimore City nonpublic Title I: no dates captured; listed open on BidNet.
6. OPP-016 TEA HB 1416 window: confirm whether the 2027-28 application window is open (prior year closed 12/12).
7. OPP-009 Humble 2027-101: three sources give three different deadlines.
8. OPP-037 ELC Miami-Dade: 11/12 versus 12/31 close; if 12/31 is correct this is still open.

Calendar consistency check: no impossible schedules found among dated items. Region 9's sequence (release 10/23, questions 11/03, addendum 11/09, due 11/20, award 12/10) is internally consistent.

## I. Legal-route notes
- The Intellectual Child LLC is the prime entity for Title I nonpublic equitable-services bids (Newark, Baltimore, Youngstown, Milwaukee, Minneapolis, Polk, PGCPS, CPS successor), tutoring provider approvals (TEA PASS, Virginia, Missouri, Massachusetts) and consultant pools (Fort Worth, Arlington, Region 18).
- The Intellectual Bookshop LLC d/b/a The Intellectual Classroom is the prime entity for catalog and materials vehicles (Region 7 ICAT, Humble 2027-101, Ohio intervention list) and for PD-vendor enrollments where the buyer contracts for training rather than program delivery (NYC MTAC, Wake County, Bound Brook, Buffalo, Elizabeth).
- Dr. Dames individually fits consultant slots (NYC MTAC, ISBE adolescent literacy PL sub, TEA content authoring sub, NM Literacy Center RFI).
- Subcontract routes are mapped for every closed or awarded item in Section G.
- Before any submission, the entity named on the cover letter, W-9, SAM/UEI, insurance certificate and execution page must match (see `libraries/disqualification_patterns.md`).

## J. Research baseline note
Any instructional content described in a response to these opportunities is anchored to Beyond Phonics: Making Comprehension Visible unless newer peer-reviewed research strengthens that baseline; the win-theme library records where buyers ask for an evidence base so proposals cite it directly.

## Next-run controls (carry forward)
1. Open every roster URL directly now that hosts are allowed; convert PARTIALLY VERIFIED and DISCOVERY LEAD rows to VERIFIED or correct them.
2. Run the unrun regions and sweeps on separate turns so the search budget is not shared.
3. Weekly backward audit due 2026-11-25 covering releases dated 2026-11-18 to 2026-11-25.
4. Monthly metrics report due 2026-12-18.
