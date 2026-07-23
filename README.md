# Fins3648_Automated

Agent-assisted workspace for the FINS3648 capstone project. Built by Kunlin (CTO).

## What this is
A Claude Code project that keeps the capstone anchored to course material and to the actual
marking criteria. The rules in `CLAUDE.md` are enforced on every piece of generated content —
particularly: nothing goes in the report unless it is grounded in a course concept, a real
citation, or a labelled assumption.

## Setup
1. Put this folder in `~/Documents/Github/Fins3648_Automated`.
2. Open it with Claude Code (`claude` from inside the folder).
3. `git init && git add -A && git commit -m "P0: scaffold"`.

Skills load automatically from `.claude/skills/`. No configuration needed.

## Layout
```
CLAUDE.md            Hard rules. Read this first — it is enforced, not advisory.
STYLE.md             Single-voice style guide. Loaded before any writing.
course/              Condensed W1–W7 notes + assessment spec + case index.
phases/PHASES.md     P0–P7 workflow with gates.
evidence/            Sourced-claims register. Fill as you go.
deliverables/        report/ deck/ financials/ — outputs land here.
handover/            Templates for the five handover packs and speaker briefs.
.claude/skills/      Eight skills (below).
```

## The skills
Five by role, three by deliverable:

| Skill | Owner | Produces |
|---|---|---|
| `ceo-problem-market` | CEO | Problem statement, sizing, why-now, competitive map |
| `cmo-positioning-gtm` | CMO | Segment, positioning, GTM, pitch storyline |
| `cto-solution-architecture` | CTO | Architecture, model justification, prototype scope |
| `cfo-business-model-financials` | CFO | Revenue model, unit economics, 5-yr P&L, the ask |
| `coo-delivery-risk-compliance` | COO | Implementation, risk register, regulatory pathway |
| `report-assembler` | — | 25-page assembly, page budget, voice harmonisation |
| `pitch-deck-builder` | — | 10–12 slides, 5 min, five equal speaking blocks |
| `course-alignment-check` | — | **The gate.** Run before anything is called finished |

The role skills are named by function, not persona, so they trigger reliably on the task
rather than on a job title. `course-alignment-check` is the one that protects the marks —
run it often, and do not argue with it.

## Workflow
Kunlin drafts P1–P5, extracts the deck at P6, then hands each member a pack containing their
section, the decisions made on their behalf, what is deliberately unfinished, and a **speaker
brief** so they can defend the content live. The team refines from P6; Kunlin re-runs
assembly and the gate after their edits.

50/50 split: draft and evidence base from Kunlin, refinement and delivery from the team.

## Three things that will cost marks if ignored
1. **Report before deck.** Building the deck first produces a deck that contradicts the report.
2. **Justify every technology.** "We use AI" was explicitly called out as unacceptable.
3. **One voice.** Five people editing will fragment it. Re-run the voice pass every time.

## Deadlines
Deck (PPT) 12:00 noon Wed Week 10 · Live pitch Week 10 class · Report (PDF) 21:00 Sun Week 10.
Full detail in `course/00-assessment-spec.md`.
