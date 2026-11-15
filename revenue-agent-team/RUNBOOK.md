# Runbook — how to run the Revenue Agent Team

> Plain English: this is the process sheet. Follow it top to bottom every time you have a new
> idea, offer, video, or audience. The order matters: **market signal → offer → content →
> conversion → review.** Skip the order and you get random content. Follow it and you get a system.

## 0. Before you run (2 minutes)
- Open `BUSINESS-BRIEF.md`. Fix anything marked **[ASSUMPTION — edit me]**.
- Decide the ONE idea you are running this time (e.g. "a 14-minute screen recording showing the
  BRR dashboard to literacy coaches").

## 1. Sharpen the ask (optional, recommended)
Paste `prompts/02-strategist-analysis.md` into Claude Code with your idea. Read the gaps it finds.
Then paste `prompts/03-merge-upgrade.md` so it rewrites your idea without losing your voice.

## 2. Run the team
Paste `prompts/04-run-the-team.md` into Claude Code, filling in the idea. Claude will run the
five agents **one at a time, in order**, because each agent reads the previous agent's file:

| Step | Agent                       | Reads                      | Writes                        |
|------|-----------------------------|----------------------------|-------------------------------|
| 1    | market-signal-scout         | brief                      | outputs/01-market-signal.md   |
| 2    | offer-architect             | brief + 01                 | outputs/02-offer.md           |
| 3    | content-strategist          | brief + 01 + 02            | outputs/03-content.md         |
| 4    | conversion-system-builder   | brief + 02 + 03            | outputs/04-conversion.md      |
| 5    | revenue-reviewer            | brief + 01–04              | outputs/05-final-brief.md     |

Running them in parallel would break the chain, so do not.

## 3. Add your taste (the step most people skip)
Open `outputs/05-final-brief.md`. Mark anything that is wrong, generic, or not how you would say
it. Then paste `prompts/05-second-pass.md`. The reviewer re-grades with your notes.

## 4. Archive the run
Move the five output files into `outputs/archive/YYYY-MM-DD-<idea>/` so the next run starts
clean but nothing is lost. (Or ask Claude to do it.)

## Agent permissions (who may do what)
- **Research the web:** market-signal-scout only.
- **Write files:** all five, but each writes only its own numbered output.
- **Run commands / edit code:** none. This team never touches the dashboard source.
- **Remember the project:** `CLAUDE.md` at the repo root holds the standing rules.

## Reusing the system for something new
Change only two things: the idea in `prompts/04-run-the-team.md` and, if the audience changed,
the audience section in `BUSINESS-BRIEF.md`. Everything else stays.
