# BRR Procurement Watch: Daily Report, 2026-11-19 (Central Time)

Run 2. First run with official pages opened through the session proxy. Eight lanes ran (Illinois/Wisconsin, Michigan/Ohio/Midwest, Texas, East, South, West/Federal, fresh discovery, forward-signal gaps). Ledgers hold the detail; this report is the control surface.

## DISCOVERY CONTROL
```
Priority direct sources on roster (direct lane, SRC-001..090):   81
  Opened on the official page (CHECKED):                          23 / 81
  Host not allowed by environment (HOST NOT ALLOWED):             42 / 81
  Reachable but JS-rendered, WAF, login or form-only:             13 / 81
  Other (404 unresolved, server error):                            3 / 81
New releases dated 2026-11-02 to 2026-11-19 found by direct checks:     5  (MDE 35p; Ohio DEW Approved Assessments RFQ; HISD 27-10-28; ChildCareGroup 2026-20; ISBE EHCY)
New releases in that window found by fresh discovery / BidNet sweeps:    7  (Friendship PCS DC; East Hartford CT; CA ELOP Summer 2027; CA ASES/ELO-P pool; SC PACE Academy; DC ELA book supplier; TX PD consultants pool)
Existing rows verified on official pages this run:                      25  (VERIFIED), plus 23 corrected
Coverage misses logged this run:                                        14
  High-severity (found after an early gate):                             2  (Ohio DEW Approved Assessments RFQ; HISD 27-10-28)
  Serious (found after final deadline):                                  7
  Coverage (3+ days late, still open):                                   5
Earliest newly found release:                                   2026-11-18
Oldest newly found release still open:                          2026-03-06 (HISD 26-01-20)
Six-month forecast rows now tracked:                            74  (29 added or materially corrected today)
Direct-source lane complete:                                    PARTIAL (all 8 lanes ran; 42 sources blocked by network policy)
Fresh-discovery lane complete:                                  YES (9 sweep families, 20 queries; cooperative and tribal portals blocked)
```
"No new opportunities" is not claimed for any source. Twelve new releases were found across the sources named in `source_roster.csv`.

## A. Source accountability
Per-source status, corrected URLs and working endpoints are in `source_roster.csv` (112 rows; 22 added today). What changed in how sources are checked:
- CPS Bonfire and TEA Bonfire open through their public JSON endpoints, not the portal page.
- Houston ISD IonWave opens through the sourcing-events list link; the old roster URL was dead.
- ISBE's NOFO list and FY27 planning calendar open through SharePoint REST; the PDF the roster pointed to is gone.
- ESBD is server-rendered page by page; the lane scanned 24 pages (576 postings) by title.
- COMMBUYS bid-detail pages open by bid id; the search form does not.
- BidNet public keyword search opens; issuer and number are locked behind registration.
- Detroit posts on DemandStar, not Bonfire; Milwaukee moved its bids to Bonfire; Philadelphia's solicitations live only in an Oracle Fusion login portal; Pittsburgh uses Beacon Bid.
- JS or WAF walls with no workaround yet: eVA, eMMA, PASSPort, Hillsborough, ELC Miami-Dade, Youngstown (Apptegy bot wall), fldoe.org and doe.virginia.gov (Akamai), procurement.opengov.com.

## B. Items that need a decision this week (sorted by gate)
| Gate | Opp | Issuer | What | Route | Status |
|---|---|---|---|---|---|
| 11/19 (today) | OPP-008 | ESC Region 7 (TX) | ICAT2628 instructional catalog bid | Intellectual Classroom | DISCOVERY LEAD; host blocked; decline unless already prepared |
| 11/20 4:00 PM CT | OPP-004 | Region 9 REC / NMPED | RFP 27008 K-3 screening; D-only bids not allowed (Addendum A) | sub to assessment prime only | VERIFIED; no prime path; pursue awardees after 12/10 |
| 11/20 (questions) ; 11/29 end of day CT | OPP-077 | Friendship PCS (DC), attribution to confirm | Role-differentiated structured-literacy training development and delivery | Intellectual Child LLC prime | DISCOVERY LEAD; register on BidNet to unlock; direct fit |
| 11/23 | OPP-005 | Pittsburgh PS | K-5 literacy screener system | sub to platform vendor | PARTIALLY VERIFIED; Beacon Bid blocked |
| 11/30 | OPP-073 | Michigan MDE | 35p High Impact Tutoring grant | partner to district | VERIFIED; BRR not on the eligible-partner list this cycle |
| 11/30 | OPP-097 | SC PACE Academy (BidNet) | Structured-literacy materials, decodables, PD, intervention | Intellectual Classroom | DISCOVERY LEAD |
| 12/01 4:00 PM CT | OPP-096 | CA district (BidNet) | ASES / ELO-P provider pool | Intellectual Child LLC | DISCOVERY LEAD |
| 12/03 file-share; 12/07 6:00 AM CT (page) vs 12/04 (PDF) | OPP-076 | Ohio DEW | 2027-28 Approved Assessments RFQ, Tier 1 dyslexia screener | Intellectual Classroom (assessment) | VERIFIED; CONFLICT on deadline; only if the BRR assessment has K-6 screener subtests |
| 12/04 5:00 PM CT | OPP-083 | ChildCareGroup (TX) | Pre-service ECE teacher training cohort | Intellectual Child LLC | VERIFIED; weak fit |
| 12/04 2:00 PM CT | OPP-095 | CA district (BidNet) | ELOP Academic Summer 2027 Scholars (literacy/ELA/ELD) | Intellectual Child LLC | DISCOVERY LEAD; strong fit |
| 12/04 | OPP-099, OPP-100 | DC book supplier; TX PD consultants pool (BidNet) | books; PD pool | Bookshop; Child LLC | DISCOVERY LEAD |
| 12/07 10:00 AM CT | OPP-081 | Houston ISD | 27-10-28 SpEd instructional materials, tech and PD | Child LLC (PD) / Classroom (materials) | VERIFIED; pre-proposal and questions already passed |
| 12/04 questions; 12/18 10:00 AM CT | OPP-079 | Houston ISD | 26-10-09-B Freelance RLA Content Contributor (individuals only) | Dr. Dames individually | VERIFIED; medium fit, low effort |
| 12/10 | OPP-010 | Hamilton County Schools (TN) | Comprehensive instructional vendor library | Intellectual Classroom | PARTIALLY VERIFIED; Vendor Registry blocked |
| 12/11 10:59 AM CT | OPP-078 | East Hartford PS (CT) | K-5 core literacy program + implementation | sub to publisher | DISCOVERY LEAD |
| 12/11 4:00 PM CT | FC-003 | Michigan ISDs | 35a(2) coach grant closes; ISD PD spend follows | Intellectual Child LLC | VERIFIED |
| 12/18 | OPP-080 | Houston ISD | 26-01-20 Dyad Specialty Offerings (individuals) | Dr. Dames | scope behind login |
| 12/20 11:00 AM CT | OPP-082 | TEA | Rolling RFP #5 Tier 1 instructional materials presolicitation | Classroom or sub | PARTIALLY VERIFIED |
| 12/28 10:59 PM CT | OPP-001 | Ohio DEW | Ohio After School FY28 Cohort A RFA | Intellectual Child LLC PRIME (for-profits eligible) or partner | VERIFIED; office hours Dec 2, 9, 16 |
| 12/31 11:00 AM CT | OPP-011 | Massachusetts DESE | 25MACISMB1 early literacy tutoring master agreement | Intellectual Child LLC | VERIFIED; read Addendum III priority deadline |

## C. Material changes to previously reported items
- CPS Board: no November meeting. Next meeting December 17 (run 1 said November 19). Arts pool RFQ 26-1355 (BRR's own bid) closed November 6 and is not yet awarded; expect the December 17 or January 28 agenda.
- CPS Title I nonpublic pool 22-0824-EX2 expires August 31, 2027. Twenty vendors, Mainstream among them, NTE $100M. Successor solicitation expected February to June 2027. This is now the highest-value forecast (FC-050).
- CPS OST pool awarded October 22 (126 vendors; operational January 1, 2027; master agreements due by about February 19). Subcontract outreach window is now.
- CPS Professional Learning pool is in its final renewal to May 31, 2028; a new pool RFQ is expected late 2027.
- CPS Library Books pool ends June 30, 2027; re-bid expected March to May 2027.
- Baltimore City "open" nonpublic Title I record was a 2018 posting; the real cycle is annual in February (last: February 17 to March 5, 2025).
- Newark RFQ 10343 closed October 27; Newark runs October (ELA/Title I) and May (enrichment/PD) cycles.
- Youngstown closed May 29; Milwaukee designates providers by consultation (Catapult and Learning Exchange for 2026-27).
- Polk County: Catapult Learning won ($831,120, 7/1/2026 to 6/30/2027 with renewals). The run-1 forecast of a 2027 rebid is withdrawn.
- Houston ISD approved-vendor pools 26-04-36/46/47 take effect July 1, 2027, not 2026-27.
- TEA HB 1416 list is for computerized products only; fit dropped to 2. PASS requires one year of Texas operation for a company.
- Wake County HDT training item closed September 2025; Wayne RESA item closed August 2025; both were run-1 errors.
- Ohio After School FY28: for-profit entities are eligible applicants, so BRR can apply as prime. RFA was posted October 15, not November 16.
- Michigan 35a(2) opened November 10 and closes December 11; 35m is $50M for FY27 (not $64.4M); 35p HIT grant (new) closes November 30.
- BuyBoard 748-24 runs to October 31, 2027; the run-1 "expired" note was wrong.

## D. Access gaps and alternates used
- Network: 42 of 81 direct sources are on hosts the environment does not allow. A consolidated host list is in the lane files and is being proposed for the environment. Alternates used: BidNet public search, EdWeek Market Brief alerts, search snippets of official pages.
- Search budget: lanes used 95 of 96 allotted queries; nothing material was left unsearched because fetches carried most of the load.
- Login-dependent facts: Newark portal (credentials via Purchasing), Houston IonWave attachments, NYC Vendor Portal MTAC documents, BidNet issuer identities, Bonfire opportunity documents, Philadelphia Oracle portal, Pittsburgh Beacon Bid, Hillsborough VendorLink.

## E. Coverage misses logged today
Fourteen rows (MISS-019 to MISS-032). Root causes: issuer page not on roster (5), dead roster URL (2), portal blocked in run 1 (3), state not covered in run 1 (3), run-1 analyst error (1). Each carries one control change; the largest are the corrected portal endpoints in Section A and the 22 new roster rows.

## F. Forward signals added or corrected
Twenty-nine forecast rows added or corrected (FC-050 to FC-074 plus corrections). Nearest dated items: CPS Board December 17; MDE 35p awards after November 30; Michigan 35a(2) deadline December 11; TDOE Education Freedom Scholarship renewals open December 8; NYC supplier-diversity sessions start December 17 (MTAC session April 1, listing session March 18); Ohio After School awards February 26, 2027; Baltimore nonpublic Title I cycle February 2027; VDOE tutoring provider window January 1 to 30, 2027; TEA HB 1416 window January 4 to 8, 2027; Newark May and October cycles; CPS nonpublic Title I successor February to June 2027.

## G. Awards and subcontract routes
Ten award rows added (AWD-021 to AWD-030). The recurring name is Catapult Learning: it holds nonpublic Title I work in Milwaukee, Youngstown, Polk, NOLA, Palm Beach and sits in the CPS nonpublic and OST pools. A single subcontract conversation with Catapult reaches six buyers.

## H. Human-verification flags
1. OPP-076 Ohio DEW deadline conflict (12/07 page vs 12/04 PDF): email ApprovedAssessments@education.ohio.gov.
2. OPP-077 Friendship PCS: issuer attribution and submission method unconfirmed; questions due tomorrow.
3. OPP-057 Minneapolis nonpublic RFP: last year's release was November 20; check weekly.
4. OPP-089 CPS Arts pool award: watch December 17 agenda.
5. OPP-009 Humble ISD: three dates still conflict.
6. OPP-047 DoDEA: SAM response date typo; solicitation expected December to February.
7. OPP-031 NM PED: site returned 502 all day; retry.
8. OPP-037 ELC Miami-Dade: JS shell; confirm in a browser.

## I. Legal-route notes
- Prime routes verified this run: Ohio After School (Intellectual Child LLC, for-profits eligible); NYC MTACs R1256/R1149 (Intellectual Classroom) and R1129/R1180 arts (Intellectual Child LLC); Houston small-contractor items (Dr. Dames individually, no subcontracting allowed); TEA PASS (company needs one year of Texas operation).
- Mainstream Development Educational Group is a current CPS nonpublic Title I pool vendor. Decide before February whether BRR bids the 2027 successor as prime, under Mainstream, or both.
- Catapult subcontract conversations run through The Intellectual Child LLC.

## Next-run controls
1. Approve the host additions so the 42 blocked sources open; re-run those lanes.
2. Open the CPS Sourcing Plan and Renewals sheets (docs.google.com) and the NYC upcoming-solicitations spreadsheet.
3. Register on BidNet to unlock the seven locked issuers.
4. Weekly backward audit due 2026-11-25; monthly metrics 2026-12-18.
