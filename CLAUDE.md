# Project memory — BRR Dashboard / Revenue Agent Team

## Who I am working with
An education transformation leader and literacy researcher. Treat them as a beginner with
Claude Code: explain files, agents, and commands in plain English as you go, briefly.

## Standing rules
- Pedagogy is anchored in the **Beyond Phonics** framework. Use newer research only when it
  clearly enhances that baseline, and say so.
- No invented statistics, sources, or student results. Label estimates as estimates.
- No guaranteed-outcome language. Never suggest collecting student PII in marketing assets.
- Voice: warm, expert, practical. Educator-to-educator.

## The Revenue Agent Team
- Context: `revenue-agent-team/BUSINESS-BRIEF.md`. Process: `revenue-agent-team/RUNBOOK.md`.
- Agents live in `.claude/agents/`. Run them **sequentially** in this order:
  market-signal-scout → offer-architect → content-strategist → conversion-system-builder →
  revenue-reviewer. Each reads the previous agent's output file.
- Outputs land in `revenue-agent-team/outputs/` as `01-` through `05-`.
- The agents never edit dashboard source code.

## The dashboard
`brr-predictive-dashboard-full.zip` holds a React prototype (BRR Predictive Dashboard). It
scores reading risk across five language domains and six meaning categories and recommends
Beyond Phonics actions. Do not unzip into the repo root without being asked.
