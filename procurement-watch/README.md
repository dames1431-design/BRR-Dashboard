# BRR Procurement Watch

An auditable procurement-intelligence system for Beyond Reading Readiness (BRR) opportunities: RFPs, RFQs, RFIs, vendor pools, grants, funded demand, awards and subcontract routes across US K-12, early-childhood, library, juvenile-justice, charter and nonpublic-school buyers.

Start with `CONTROLS.md`. It is the governing specification. The folder layout:

- `source_roster.csv`: every priority source with status from the last run.
- `ledgers/`: opportunity, forecast, closed-miss, award/subcontract and amendment ledgers. Append-only; lifecycle status changes, rows never vanish.
- `libraries/`: keyword families, commodity codes, win themes, pricing, evaluation criteria, disqualification patterns, partners, incumbents, buyer calendar, buyer contacts.
- `reports/`: daily watch reports (with the Discovery Control header), weekly backward audits, monthly metrics.

Research baseline for any instructional content referenced in proposals: Beyond Phonics: Making Comprehension Visible, unless newer peer-reviewed research strengthens that baseline.
