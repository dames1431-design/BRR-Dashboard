# BRR Procurement Watch: Control Specification

Owner: Dr. Kathy W. Dames, EdD (The Intellectual Child LLC; The Intellectual Bookshop LLC d/b/a The Intellectual Classroom)
System of record: this folder. Nothing here is deleted; items move through lifecycle status only.
Spec adopted: 2026-11-18. Source: "RFP scopr" working document.

The watch is judged by a visible coverage system, not by how thorough a report looks. Trust comes from showing where the search looked, when each source was checked, and where discovery failed.

---

## 0. The one sentence that governs every daily report

> "No new opportunities" may be stated only when BOTH the direct-source lane and the fresh-discovery lane were completed for the current run, and the report names which priority sources were actually checked and which could not be accessed.

"No new opportunities" therefore means "none were found across the named sources checked today," never "the public procurement universe was exhaustively searched."

---

## 1. Three-layer assurance standard

| Layer | Cadence | What it does | Output |
|---|---|---|---|
| 1. Direct-source checks | Daily | Every priority issuer/portal on `source_roster.csv` is opened and marked CHECKED / INACCESSIBLE / NOT FOUND | Source roster status column; Discovery Control header |
| 2. Fresh national discovery | Daily | Independent keyword-family sweep outside the roster (aggregators, state bulletins, cooperatives, nonpublic, library, early-childhood, juvenile-justice, charter, tribal, rural) | New issuers to add to roster; new opportunities |
| 3. Backward coverage audit | Weekly (30-day audit monthly) | Deliberately search releases from the prior 7 days (30 days monthly) and reconcile against what the daily watch reported. Every unmatched item is a documented coverage miss | `closed_miss_ledger.csv`; roster expansion |

Backfill is also run daily: every run searches the prior 7 days, not only forward, to catch late-indexed releases.

---

## 2. Daily report header: DISCOVERY CONTROL

Every report opens with this block, filled with real numbers and a denominator:

```
DISCOVERY CONTROL  (run date, Central Time)
Priority direct sources checked:            NN / NN   (denominator = roster rows flagged priority)
Sources inaccessible today:                 NN   (named in Section D)
New releases found by direct checks:        NN
New releases found by fresh discovery:      NN
Coverage misses discovered:                 NN   (3+ days late)
High-severity misses:                       NN   (found after an early mandatory gate)
Serious misses:                             NN   (found after final deadline)
Earliest newly found release:               YYYY-MM-DD
Oldest newly found release:                 YYYY-MM-DD
Six-month forecast sources checked:         NN
Known upcoming releases currently tracked:  NN
Direct-source lane complete:                YES / NO
Fresh-discovery lane complete:              YES / NO
```

Report "43 of 47 checked," never "priority markets checked."

---

## 3. Source accountability

- Every run names the exact official sources checked. "Texas checked" is too broad; the report says ESBD, TEA Bonfire, Houston ISD IonWave, ESC Region 4, and so on, each with a status.
- Evidence hierarchy: official issuer page first, official procurement portal second, official legal notice third, aggregator only as a discovery lead.
- Access-failure logging: when Bonfire, IonWave, BidNet, NexSys, EUNA, PASSPort or any portal blocks access, log the gap and search an alternate official source. Never conclude "no opportunity" from a blocked portal.
- Portal-login dependency flag: mark opportunities requiring authenticated access and list which facts remain unverified behind the login.
- Source freshness check: if a procurement page has not changed for weeks, verify through a second official source (board agenda, legal notice).
- Monthly source audit: confirm every priority portal still uses the same platform and URL. Districts switch vendors.
- Source expansion after every miss: any issuer or portal tied to a coverage miss is added permanently to the direct-check roster.
- File-level verification: when the packet is a PDF, spreadsheet or attachment, open the file; do not rely on the summary page.
- Portal-search variation: search by solicitation number, exact title, abbreviated title, buyer name, commodity code, NAICS and keyword family.
- Board-packet attachments: search exhibits, memos and consent-agenda backup PDFs, not only agenda titles.

---

## 4. Discovery-lane rules

- Keyword-family search (see `libraries/keyword_families.md`), never "literacy" alone.
- Commodity-code tracking: NIGP, NAICS, UNSPSC, state commodity codes and district category codes for literacy, books, tutoring, consulting, training, assessment, software and instructional materials (see `libraries/commodity_codes.md`).
- Broad-scope capture: never discard an RFP because math, technology, special education or multilingual services sit beside literacy. Extract the BRR parcel.
- False-positive control: do not inflate the watch with generic education solicitations lacking a plausible literacy, language, PD, assessment, tutoring, materials or implementation parcel.
- No-market-blindness: rural, suburban, regional service agencies, tribal, juvenile-justice, charter, nonpublic and library opportunities are searched alongside large urban districts.
- Supplier-diversity lane: MBE/WBE, DBE, HUB, SBE and local subcontracting goals are searched even when BRR is not the prime.
- Prime-bidder watch: when bidder or attendee lists become public, identify likely primes and map BRR's subcontract parcel before award.
- Sole-source and emergency-purchase watch; cooperative piggyback clauses; interlocal agreements.
- Lanes that must be searched explicitly: Title funding (I, II, III, IV, IDEA, ESSER closeout, McKinney-Vento, Migrant, 21st CCLC, school improvement); research grants (IES, NSF, foundations, RPPs); university partners; foundation-funded district work; library systems; early childhood (Head Start, state pre-K); juvenile justice and alternative schools; charter networks and authorizers; nonpublic equitable services; school-level discretionary purchasing under small-purchase thresholds; cooperative purchasing (ESCs, BOCES, IUs, Choice Partners, OMNIA, TIPS, Sourcewell, BuyBoard).

---

## 5. Forward-signal lane (six-month runway)

Searched every run; produces `forecast_ledger.csv` entries before any notice exists.

- Historical-cycle model: for every recurring procurement, store prior release month, award month, term, renewal options and the likely successor window.
- Contract-expiration trigger: contracts ending within 18 months create forecast entries.
- Renewal-risk watch: as an option year approaches, flag whether the district must renew, rebid, amend or board-approve.
- Board-agenda trigger: "approve RFP," "authorize solicitation," "curriculum adoption," "professional services," "tutoring," "literacy," "instructional materials," "grant-funded services."
- Award-board reconciliation: compare portals with board agendas and minutes; boards often act before the portal changes.
- Budget-line trigger: adopted budgets and amendments for literacy, tutoring, intervention, curriculum, assessment, summer learning and PD.
- Grant-to-procurement trigger and awarded-grant recipient watch: every major literacy or OST grant award creates a recipient-level downstream watch.
- Vendor-pool reopening trigger: supplemental rounds, annual refreshes, new cutoffs.
- State-legislation trigger and rulemaking trigger.
- Approved-materials-list watch: additions, removals, review cycles, appeal windows.
- Pilot-to-adoption conversion watch.
- Superintendent-plan and school-improvement-plan scanning (CSI, TSI, ATSI, MTSS).
- Union-contract implementation, staffing-vacancy, program-expansion, performance-data, audit-finding and litigation/consent-decree triggers.
- Buyer-calendar tracking: board meeting dates, budget adoption dates, procurement planning calendars, fiscal-year milestones (`libraries/buyer_calendar.md`).
- Buyer-name tracking: procurement officers, curriculum directors, Title I leads, literacy directors (`libraries/buyer_contacts.csv`). Personnel changes signal rebids.
- Pre-award networking signals: vendor fairs, bidder conferences, supplier-diversity events, industry days, pre-solicitation webinars.
- Reference-district intelligence and geographic heat map: track where literacy funding and activity is rising.

---

## 6. Opportunity record rules

Every tracked item carries:

| Field | Rule |
|---|---|
| Lifecycle status | forecast -> announced -> released -> submitted/closed -> award pending -> awarded/canceled -> successor watch. No silent deletion. |
| Procurement stage | forecast, RFI, presolicitation, released, vendor pool, grant, funded demand, award, subcontract route, closed-successor watch |
| Confidence | VERIFIED / PARTIALLY VERIFIED / DISCOVERY LEAD |
| Probability | HIGH / MEDIUM / LOW from source strength and procurement history |
| Priority score | Four separate 1-5 scores: Fit, Revenue, Ease of entry, Time-to-action. Never collapsed into one number, so a hard but valuable item stays visible |
| Revenue quality | one-time project / recurring contract / vendor-pool eligibility / grant-funded demand / speculative forecast |
| Legal route | Dr. Kathy individually / The Intellectual Child LLC / The Intellectual Bookshop LLC d/b/a The Intellectual Classroom / partner or subcontract, per the actual solicitation |
| Time zone | issuer-local deadline AND Central Time, always both |
| Evidence-age stamp | date the source was last verified |
| Release date | actual publication date; findings sorted by release date newest first, due date secondary |
| Discovery lag | days from release to discovery; drives miss severity |
| Portal-login flag | which facts are unverified behind login |
| Conflict-resolution | when two official sources disagree, show both, name the conflict, do not pick one without stronger evidence |
| Human-verification trigger | any item within 7 days of a mandatory gate with conflicting public information gets a prominent MANUAL VERIFICATION flag |
| Calendar consistency | release, questions, conference, proposal, award and start dates compared; impossible schedules flagged immediately |
| No-deadline-source dismissal | an item with no due date stays active until closure, award, cancellation or a verified superseding notice |
| No duplicate noise | a previously reported item reappears only for a material change: runway-band transition, amendment, new gate, award, reopening, correction |
| Amendment diff | every addendum summarized: dates, scope, eligibility, pricing, insurance, mandatory meetings, samples, references, subcontract rules |

---

## 7. Miss taxonomy and learning loop

| Severity | Definition |
|---|---|
| DISCOVERY COVERAGE MISS | found 3+ days after release |
| HIGH-SEVERITY MISS | found after an early mandatory gate (pre-bid conference, intent-to-bid, question deadline) |
| SERIOUS DISCOVERY MISS | found after the final deadline |

Every miss row in `closed_miss_ledger.csv` must carry:
1. Root cause: portal access / missing keyword / issuer omission from roster / indexing delay / wrong cadence / analyst error.
2. One concrete control change (not just a label), for example a roster row added, a keyword added, a cadence changed.
3. Successor route: awardee subcontract, rebid forecast, renewal date, cooperative route, school-level purchase, or next annual cycle. A closed miss with no follow-on path is incomplete.
4. Cancellation/reissue watch when an RFP is canceled or withdrawn.

Market-loss learning: when BRR declines or loses, capture the reason so qualification and timing improve.

---

## 8. Intelligence libraries (append-only)

- `libraries/win_themes.md`: recurring buyer priorities (evidence base, implementation fidelity, multilingual learners, accessibility, data use, family engagement, teacher capacity).
- `libraries/pricing_intelligence.csv`: public rates, per-student pricing, hourly and session rates, materials costs, renewal increases, award values by service type. Sources: bid tabs, pricing abstracts, award recommendations, prior contracts.
- `libraries/evaluation_criteria.csv`: weighted scoring criteria for every major RFP.
- `libraries/disqualification_patterns.md`: recurring compliance failures (signatures, insurance, references, samples, portal errors, missing forms).
- `libraries/partner_intelligence.csv`: likely partners by capability (math, assessment, software, multilingual, special education, tutoring staffing, research, national implementation).
- `libraries/incumbents.csv`: current vendor, value, start/end, extensions, performance issues, rebid status.
- `libraries/keyword_families.md` and `libraries/commodity_codes.md`.
- `libraries/buyer_calendar.md` and `libraries/buyer_contacts.csv`.

---

## 9. After-award tracking

Once an award is made (to BRR or anyone else): kickoff, training, materials delivery, pilot, benchmark windows, midyear review and renewal decision points go into `award_subcontract_ledger.csv`. Award-to-subcontract trigger: identify the winner and assess BRR subcontract, implementation, materials, training or licensing routes immediately.

---

## 10. The watch measures itself

Monthly metrics report (`reports/YYYY-MM_metrics.md`):
- Discovery rate (new releases found per run)
- Average discovery lag (days)
- Number of coverage misses; number of serious misses
- Percentage of priority sources successfully checked
- Percentage of newly released opportunities found within 24 hours
- Actionable-lead rate; conversion to bids and partnerships
- Search-term decay review: which keywords actually found opportunities; new buyer language added

Quarterly watch audit: source coverage, hit rate, missed-release rate, actionable-lead rate, conversion.

---

## 11. Required files

| File | Purpose |
|---|---|
| `source_roster.csv` | Every priority source with platform, URL, lane, cadence, last-checked, status |
| `ledgers/opportunity_ledger.csv` | Every announced or released item through its full lifecycle |
| `ledgers/forecast_ledger.csv` | Six-month runway items before a notice exists |
| `ledgers/closed_miss_ledger.csv` | Every coverage miss with root cause, control change, successor route |
| `ledgers/award_subcontract_ledger.csv` | Awards, winners, subcontract routes, implementation calendars |
| `ledgers/amendment_log.csv` | Addendum diffs |
| `reports/YYYY-MM-DD_daily_watch.md` | Daily report with Discovery Control header |
| `reports/YYYY-MM-DD_weekly_audit.md` | Weekly backward audit |
| `reports/YYYY-MM_metrics.md` | Monthly self-measurement |
