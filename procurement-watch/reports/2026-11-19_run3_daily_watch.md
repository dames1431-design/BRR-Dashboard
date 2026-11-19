# BRR Procurement Watch: Daily Report, 2026-11-19 evening (Central Time), Run 3

Run 3 was the first pass with unrestricted network access. Eight lanes opened official portals directly, including JSON endpoints behind Bonfire, IonWave, DemandStar, BoardDocs, Legistar and SharePoint that earlier runs could not reach.

## DISCOVERY CONTROL
```
Priority direct sources on roster (SRC-001..112, direct lane):      98
  Opened on the official page or official API (CHECKED):             62 / 98
  Reachable but walled (JavaScript, login, firewall, bot challenge):  32 / 98
  Unreachable or other (TLS reset, proxy 502, server 502, not pulled):  4 / 98
New releases dated 2026-11-02 to 2026-11-19 found by direct checks:          7  (DPSCD 27-0090; Choice Partners 27/006SG and 27/007SG; MA DESE 27TALRJ1; LR5 2027-012; New Caney 149.26-2; Abilene #001)
New releases in that window found by discovery / aggregators:                3  (York City books; OCPS RFP26033; KIPP DC ELA book supplier)
Open items found with earlier release dates:                                 4  (Fulton 143-27; Hempstead 2027.01; LIFE Academy; DPSCD RFI-27-0009)
Existing rows verified on official pages this run:                          31
Coverage misses logged this run:                                            14
  High-severity (found after an early gate):                                  0
  Serious (found after final deadline):                                       5
  Coverage (3+ days late, still open):                                        9
Earliest newly found release:                                       2026-11-17
Oldest newly found release still open:                              2026-07-01 (DPSCD RFI-27-0009)
Six-month forecast rows now tracked:                                        92  (18 added, 29 corrected)
Direct-source lane complete:                                                YES (all 98 attempted; 34 walled or unreachable, each named)
Fresh-discovery lane complete:                                              YES (aggregators, cooperatives, tribal, foundations)
```
"No new opportunities" is not claimed for any source. Fourteen new releases were found.

## A. Source accountability
Per-source status, corrected URLs and working endpoints are in `source_roster.csv` (142 rows; 30 added today). What changed:
- Working machine-readable endpoints recorded for CPS, TEA, Milwaukee, Fulton, Atlanta, Dallas, Austin, Fort Bend, St. Louis, Clark County, Utah, Tacoma and Region One (Bonfire JSON); Houston, Fort Worth, Regions 13/18/11, Allied States and New Caney (IonWave); Detroit (DemandStar agency API, contracts API, BoardDocs API); Houston ISD board (Legistar API); ISBE (SharePoint REST); CPS Buying Plan (CSV export); NYC upcoming solicitations (xlsx); SCBO online edition; Govly and Starbridge buyer pages.
- Walls with no automation path: Finalsite and Apptegy bot challenges (Hillsborough, Duval, ELC Miami-Dade, Youngstown, Kansas City, Hempstead, Humble), OpenGov portals, Ivalua (OhioBuys, eMMA), eVA, PASSPort, Beacon Bid, Oracle supplier portals (Philadelphia, Nashville), Colbi SecureBids, Bid Locker, KIPP DC Quickbase, VendorLink, BidNet abstracts, and Akamai or Cloudflare firewalls on fldoe, doe.virginia.gov, lausd, cde.ca.gov, azed, MSDE, education.mn.gov, aisd.net, TIPS, Equalis, BoardDocs for Illinois suburbs.
- Unreachable today: procurement.dadeschools.net and elcmanatee.org (TLS reset), dpsk12.bonfirehub.com and hcde.ionwave.net and ips.bonfirehub.com (proxy 502), web.ped.nm.gov (server 502).

## B. Decisions this week, sorted by gate
| Gate | Opp | Issuer | What | Route | Status |
|---|---|---|---|---|---|
| 11/20 questions; 11/30 | OPP-077 | KIPP DC (corrected from Friendship) | Role-differentiated structured-literacy training modules | Intellectual Child LLC prime or sub to platform | PARTIALLY VERIFIED; Quickbase portal sign-in |
| 11/21 decide; 11/24 10:00 AM CT | OPP-108 | Lexington-Richland Five (SC) | SPED PD and job-embedded coaching, on-site only, to 2031 | Dr. Dames / Intellectual Child LLC | VERIFIED; hard-copy sealed bid; experience minimums struck |
| 11/23 4:00 PM CT | OPP-091 | ISBE | FY27 EHCY NOFO (ROE/district applicants; tutoring allowable) | subcontract to applicant | VERIFIED |
| 11/30 1:00 PM CT | OPP-097 | PACE Academy (SC) | Structured-literacy materials, decodables, PD, intervention; vendor-neutral; CSI funds | Intellectual Classroom / Child LLC | VERIFIED; time conflict 2 vs 4 PM ET |
| 11/30 | OPP-073 | Michigan MDE | 35p HIT grant (eligible partners only) | partner | VERIFIED; BRR not on list |
| 11/30 questions; 12/04 | OPP-099 | KIPP DC | ELA book supplier (distributor scale) | Bookshop LLC | PARTIALLY VERIFIED; fit 2 |
| 12/01 4:00 PM CT | OPP-096 | CA district (BidNet locked) | ASES / ELO-P provider pool | Intellectual Child LLC | DISCOVERY LEAD |
| 12/02 questions; 12/09 2:00 PM CT | OPP-117 | New Caney ISD (TX) | Contracted PD pool (literacy, SPED, bilingual, EC, MTSS) | Intellectual Child LLC prime | VERIFIED; low-bar pool |
| 12/03 file share; 12/07 6:00 AM CT | OPP-076 | Ohio DEW | Tier 1 dyslexia screener list RFQ | Intellectual Classroom | VERIFIED; only with K-6 subtests |
| 12/04 | OPP-118 | Abilene ISD (TX) | Instructional PD pool | Intellectual Child LLC prime | PARTIALLY VERIFIED |
| 12/04 2:00 PM CT | OPP-095 | CA district (BidNet locked) | ELOP Academic Summer 2027 Scholars (literacy/ELA/ELD) | Intellectual Child LLC | DISCOVERY LEAD; register on BidNet |
| 12/04 2:00 PM CT | OPP-115 | York City SD (PA) | Multicultural books K-8 sealed bid | Bookshop LLC | DISCOVERY LEAD; email for criteria |
| 12/04 5:00 PM CT | OPP-083 | ChildCareGroup (TX) | Pre-service ECE teacher training | Intellectual Child LLC | VERIFIED; weak fit |
| 12/07 10:00 AM CT | OPP-081 | Houston ISD | 27-10-28 SpEd materials and PD | Child LLC / Classroom | VERIFIED; gates passed |
| 12/08 1:30 PM CT | OPP-103 | Fulton County Schools (GA) | Title I private-school tutoring, Phase 2 | Intellectual Child LLC prime | PARTIALLY VERIFIED; Bonfire account; incumbents Braintrust, Study Smart |
| 12/10 | OPP-109 | HCDE / Choice Partners (TX) | Textbooks, library materials, instructional resources cooperative contract | Bookshop LLC prime | PARTIALLY VERIFIED; national piggyback |
| 12/10 1:00 PM CT | OPP-010 | Hamilton County Schools (TN) | 27-01 instructional vendor library | Intellectual Classroom | VERIFIED gates; BidNet |
| 12/11 10:59 AM CT | OPP-078 | East Hartford PS (CT) | K-5 core literacy program (1914-27) | sub to publisher | DISCOVERY LEAD |
| 12/11 4:00 PM CT | FC-003 | Michigan ISDs | 35a(2) coach grant closes | Intellectual Child LLC (downstream) | VERIFIED |
| 12/14 4:00 PM CT | OPP-105 | Detroit PSCD | Summer Student Enrichment K-8 | Intellectual Child LLC prime | PARTIALLY VERIFIED; DemandStar |
| 12/18 | OPP-079, OPP-080 | Houston ISD | Freelance RLA content contributor; Dyad (individuals) | Dr. Dames | VERIFIED |
| 12/18 1:00 PM CT | OPP-116 | Orange County PS (FL) | Before/after-school programs (~100 campuses) | sub to operator | PARTIALLY VERIFIED |
| 12/20 11:00 AM CT | OPP-082 | TEA | Rolling RFP #5 Tier 1 materials presolicitation | Classroom or sub | PARTIALLY VERIFIED |
| 12/21 11:00 AM CT | OPP-107 | Massachusetts DESE | 27TALRJ1 K-3 curriculum development (Scope A foundational skills) | sub to curriculum prime | PARTIALLY VERIFIED; COMMBUYS |
| 12/28 10:59 PM CT | OPP-001 | Ohio DEW | After School FY28 Cohort A (for-profits eligible; CBOs may apply; limited-scope contracted specialists allowed) | Intellectual Child LLC prime or sub | VERIFIED; FAQ posted 11/19 |
| 12/31 11:00 AM CT | OPP-011 | Massachusetts DESE | 25MACISMB1 early literacy tutoring master agreement | Intellectual Child LLC | VERIFIED |
| 1/15/2027 2:00 PM CT | OPP-110 | HCDE / Choice Partners | Curriculum, instructional programs, assessment materials cooperative contract | Intellectual Child LLC prime | PARTIALLY VERIFIED |
| 1/29/2027 2:00 PM CT | OPP-013 | Fort Worth ISD | 27-006 consultants and PD pool | Intellectual Child LLC prime | VERIFIED |
| rolling | OPP-029, OPP-086, OPP-119, OPP-024, OPP-023 | LIFE Academy (AL); Hempstead ISD (TX); Louisiana Steve Carter tutoring; Cy-Fair; Region 18 | rolling pools and provider lists | Intellectual Child LLC | VERIFIED / DISCOVERY LEAD |

## C. Material changes to previously reported items
- CPS: the Buying Plan updated November 4 lists a new $20M Professional Learning Services RFQ advertising October to December 2026. The new PL pool is this quarter, not late 2027 (OPP-102, FC-053 corrected). The plan has no line for tutoring, books, early childhood, summer or nonpublic Title I; the 2027 nonpublic successor may come as a renewal or late addition. Also listed: Community Schools Initiative RFQ $10M (January to March 2027).
- Baltimore: the HDT RFP-26089 was awarded November 4 to 21 vendors ($10.7M a year through November 2029). The run-2 forecast of a May 2027 re-compete is withdrawn; the route is subcontracting to the ELA awardees. The June 16 agenda has no nonpublic Title I contract; that cycle is each February.
- Detroit: the Tier III literacy intervention went to Reading and Language Arts Centers ($446K to June 2027). Detroit's contracts API shows about 90 instructional contracts expiring June 30, 2027, including the nonpublic Title I provider FACTS Education Solutions ($1.21M). The Multilingual PD RFP is under evaluation with 52 planholders.
- Milwaukee: RFP 1161 tutoring went to One on One Learning and Learn It Systems; ELO contracts run to June 2027; the 2026-27 nonpublic providers came from RFP 1157 (closed December 2025), which dropped Mainstream. A 2027-28 provider RFP would post on Milwaukee's Bonfire this quarter if re-bid; none is open. Next consultation January 19; affirmation due March 5.
- NYC: the planning spreadsheet lists a $250M Supplemental Instructional Services for Nonpublic Schools RFP (September 2027 to August 2030) that has slipped past its planned spring 2026 release, plus a $227M Trade Books RFB starting January 2027. R1129 Arts Education MTAC weights are 25/25/25/25.
- Texas PASS: an out-of-state company qualifies if registered in Texas with a Texas taxpayer number and one year serving Texas students; individuals qualify with reading-specialist or structured-literacy credentials.
- The DC structured-literacy training RFP belongs to KIPP DC, not Friendship. ESC Region 7's catalog bid closed today with award December 10, and Region 7's Library Books bid opens April 5, 2027.
- Fulton County's private-school tutoring rebid (143-27) is open now, not in summer 2027.
- Pittsburg USD's HDT RFP closed October 8 (board December 11); Wayne RESA's RFP closed August 2025; both run-1 dates were wrong.
- Polk County, Hillsborough, Metro Nashville, Guilford, NOLA and Region 11 awards are still not public.

## D. Access gaps and alternates used
Walls and unreachable hosts are listed in Section A and per row in the roster. Login-only facts: BidNet abstracts (issuer names for OPP-095, 096, 100), KIPP DC Quickbase (OPP-077, 099), Newark portal, Houston IonWave attachments, Bonfire opportunity documents, COMMBUYS attachments, VendorLink (Hillsborough, Orange, Polk), SIGMA (path changed), MOVERS (Missouri), SAM.gov API (needs a real key).

## E. Coverage misses logged today
Fourteen rows (MISS-033 to MISS-046). Root causes: issuer not on roster (7), portal blocked in earlier runs (4), list not scanned or page incomplete (3). Control changes: 30 roster rows added, cooperative IonWave lists put on weekly cadence, Govly public search made a daily discovery source.

## F. Forward signals added or corrected
Eighteen rows added (FC-075 to FC-092) and 29 corrected. Nearest: CPS PL Services RFQ now through January; CPS Board December 17; Baltimore board December 1; Michigan 35a(2) December 11; PDE list publication December 2026 then April 2027 (vendor form); Missouri Consulting and Coaching QVL projected November; NYC PEP December 16; Head Start NOFOs December 15; Fry Foundation December 1; Milwaukee consultation January 19; ESC Region 7 Library Books April 5 to May 20, 2027; Detroit FY28 re-ups May to August 2027.

## G. Awards and subcontract routes
Nine award rows added (AWD-031 to AWD-039). Catapult Learning now appears in Milwaukee, Youngstown, Polk, NOLA, Palm Beach, CPS pools and Baltimore math; Braintrust in Fulton, Detroit, Milwaukee (bid) and Michigan 35p; Reading and Language Arts Centers in Detroit; One on One Learning in Milwaukee and Orange County.

## H. Human-verification flags
1. OPP-077 KIPP DC: questions due tomorrow; sign in to Quickbase to download the RFP.
2. OPP-097 PACE Academy: 2:00 vs 4:00 PM ET close; call Dr. Vaughn.
3. OPP-103 Fulton: confirm close time (JSON suggests 2:30 PM ET) and pre-bid on Bonfire.
4. OPP-076 Ohio DEW: page says 12/07 7:00 AM ET, PDF says 12/04; email ApprovedAssessments.
5. OPP-057 Minneapolis nonpublic RFP: not posted as of tonight; check daily.
6. OPP-037 ELC Miami-Dade: due date for -04 unconfirmed; call contracts.
7. OPP-049 Hillsborough award: VendorLink login only.
8. FC-038 Idaho RFI dates conflict; open sde.idaho.gov in a browser.
9. OPP-009 Humble and OPP-100 Texas PD pool: unresolved identities.

## I. Legal-route notes
- Prime: Fulton 143-27, New Caney, Abilene, Cy-Fair, Region 18, Hempstead, Louisiana Steve Carter, Ohio After School (Intellectual Child LLC); Choice Partners 27/006SG, York City books, ESC Region 7 Library Books 2027 (Intellectual Bookshop LLC); Houston individual contractor items (Dr. Dames).
- Subcontract: Baltimore HDT awardees, Detroit FY27 vendors, Milwaukee tutoring and ELO awardees, MA DESE curriculum primes, Pittsburgh screener vendor, Region 9 awardees after December 10.
- Entity match rule applies before any submission (cover letter, W-9, SAM/UEI, insurance, execution page).

## Next-run controls
1. Daily: CPS Bonfire JSON (PL Services RFQ), Minneapolis procurement page, Milwaukee Bonfire JSON.
2. Weekly: Govly search, Starbridge catalog, cooperative IonWave lists, Detroit DemandStar API, ISBE REST.
3. Weekly backward audit due 2026-11-25; monthly metrics 2026-12-18.
4. Manual list refresh: add Quickbase (KIPP DC), Colbi SecureBids (Twin Rivers), Bid Locker (Seattle), SAM API key, COMMBUYS attachments, MCPS 4609.1 vendor PDF, Idaho SDE page.
