# Fins3648_Automated

Agent-assisted workspace for the FINS3648 capstone. Kunlin (CTO) leads; the whole team
refines from one shared draft.

## What this is
A Claude Code project that keeps the capstone anchored to course material and the marking
criteria. The rules in `CLAUDE.md` are enforced on every piece of generated content — nothing
enters a deliverable unless it is grounded in a course concept, a real citation, or a
labelled assumption, and no number is invented.

## The workflow (one draft, whole team, refine)
```
Set topic in /config/team.md
        │
        ▼
draft-run  →  ONE integrated draft in /results/drafts/draft_YYYY-MM-DD.md
              (all five roles, plain English, AI-friendly, all evidence PROPOSED)
        │
        ▼
Kunlin verifies sources (PROPOSED → VERIFIED). Nothing is approved while sleeping.
        │
        ▼
Kunlin + team challenge it  →  they drop the ONE file into any AI + send feedback
        │                        (silent contribution marker logged privately)
        ▼
Refine  →  next dated draft   (repeat until stable)
        │
        ▼
Deck FIRST (pitch-deck-builder)  →  Report SECOND (report-assembler)
        │                            both derive from the SAME draft → no contradiction
        ▼
course-alignment-check = READY  →  submit
```

The single integrated draft *is* the handover. No separate packs, no "what did you do?" —
every teammate reads one self-contained, AI-friendly file and sees the whole project.

## Layout
```
CLAUDE.md            Hard rules (1–14). Enforced, not advisory. Read first.
STYLE.md             Single-voice style guide. Loaded before any writing.
config/team.md       Topic, framing, roster. A run reads this. Topic gate lives here.
course/              Condensed W1–W7 notes + assessment spec + case index.
phases/PHASES.md     Internal checklist for one run (not manual gates).
evidence/            Evidence log with PROPOSED → VERIFIED two-gate states.
results/drafts/      Where each integrated draft lands. TEMPLATE-draft.md + README.
deliverables/        report/ deck/ financials/ — final outputs land here.
private/             GIT-IGNORED, local-only. Silent contribution ledger. Never shared.
handover/            Folded into the draft; see handover/README.md.
.claude/skills/      Role skills + draft-run + contribution-marker.
```

## The skills
| Skill | Role | Produces |
|---|---|---|
| `draft-run` | orchestrator | The one integrated draft (runs everything at once) |
| `ceo-problem-market` | CEO | Problem, sizing, why-now, competitive map |
| `cmo-positioning-gtm` | CMO | Segment, positioning, GTM, storyline |
| `cto-solution-architecture` | CTO | Architecture, model justification, prototype scope |
| `cfo-business-model-financials` | CFO | Revenue model, unit economics, 5-yr P&L, the ask |
| `coo-delivery-risk-compliance` | COO | Implementation, risk register, regulatory pathway |
| `pitch-deck-builder` | — | Deck FIRST: 10–12 slides, 5 min, five equal speakers |
| `report-assembler` | — | Report SECOND: 25-page assembly, page budget, one voice |
| `course-alignment-check` | — | **The gate.** Run before anything is called finished |
| `contribution-marker` | Kunlin only | Private, local-only record of teammate engagement |

## Hard rules that cost marks if ignored
1. **Master draft first**, then deck, then report — all from one spine (no contradictions).
2. **Never invent numbers.** Fabricated stats in a submission is an integrity breach.
3. **Justify every technology.** "We use AI" was explicitly called unacceptable.
4. **No drafting without a topic** set in `config/team.md`.
5. **Overnight runs only draft**, never approve; evidence is verified by a human.

## Deadlines
Deck (PPT) 12:00 noon Wed Week 10 · Live pitch Week 10 class · Report (PDF) 21:00 Sun Week 10.
Full detail in `course/00-assessment-spec.md`.

## Setup
This folder is a git repo. Private ledger is git-ignored. `git log` shows the restructure.