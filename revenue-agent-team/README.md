# Revenue Agent Team

A reusable, five-agent system that turns one idea into a revenue path:
**market signal → offer → content → conversion → review.**

Built for the Beyond Phonics / BRR Predictive Dashboard business. Anchored in the owner's
research, not generic marketing.

## The office, in plain English
```
revenue-agent-team/
  BUSINESS-BRIEF.md     the context — who we are, who we serve, how we make money
  RUNBOOK.md            the process — run this top to bottom every time
  prompts/              copy-paste prompts (beginner mode, sharpen the ask, run, second pass)
  outputs/              where finished work lands, numbered 01–05
.claude/agents/         the workers — one file per agent, Claude Code reads this folder
CLAUDE.md               project memory — standing rules Claude follows every session
```

## The team
| Agent                       | One-line job                                              |
|-----------------------------|-----------------------------------------------------------|
| market-signal-scout         | Finds real demand and the audience's exact language       |
| offer-architect             | Designs the offer ladder and the unique mechanism         |
| content-strategist          | Titles, hooks, and a timestamped structure that sells     |
| conversion-system-builder   | Lead magnet, word-for-word CTA, 5-email follow-up         |
| revenue-reviewer            | Grades the business logic, removes hallucinations, assembles the final brief |

## Fastest start
1. Edit the **[ASSUMPTION — edit me]** lines in `BUSINESS-BRIEF.md`.
2. Paste `prompts/04-run-the-team.md` into Claude Code with your idea.
3. Read `outputs/05-final-brief.md`. Add your notes. Paste `prompts/05-second-pass.md`.

See `RUNBOOK.md` for the full process.
