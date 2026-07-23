# Phases — the internal checklist for one draft run

These are **no longer manual gates Kunlin clicks through.** They are the internal order the
orchestrator works through in a single run to produce **one integrated draft** in
`/results/drafts/`. Kunlin does not run these phase-by-phase; he sets a topic, triggers a
run, and challenges the draft that comes out (CLAUDE.md Rule 12).

The old "which phase belongs to whom" composition problem is gone: the run does all roles at
once and composes them into one document.

---

## Pre-flight (hard stops)
- **Topic set** in `/config/team.md`? If not — STOP (Rule 11).
- **Framing chosen** (entrepreneur / intrapreneur)? If not — flag it and assume nothing.
- Load `/CLAUDE.md`, `/STYLE.md`, `/config/team.md`, and the relevant `/course/` files.

## P1 — Problem, market, why-now  *(CEO lens)*
One-sentence problem: *[who] cannot [do what] because [why], costing [what]*. Sizing,
competitive map, why-now. Skill: `ceo-problem-market`.

## P2 — Evidence pack  *(CEO + CMO lens)*
Everything sourced goes to `/evidence/EVIDENCE-LOG.md` as `PROPOSED`. No unsupported claim;
gaps become `[NUMBER NEEDED]`. Skills: `ceo-problem-market`, `cmo-positioning-gtm`.

## P3 — Solution architecture & prototype scope  *(CTO lens — Kunlin's core)*
Cloud/data/API design, build-vs-partner, model justification (W3 property-valuation shape),
honest prototype-vs-roadmap line. Every technology passes the four-part test (Rule 3).
Skill: `cto-solution-architecture`.

## P4 — Business model & financials  *(CFO + COO lens)*
Unit cost → volume → revenue → 5-year P&L → break-even → ROI → the ask, bottom-up with an
assumptions tab. Working file in `/deliverables/financials/`. Skills:
`cfo-business-model-financials`, `coo-delivery-risk-compliance`.

## P5 — Positioning, GTM, implementation, risk  *(CMO + COO lens)*
Segment, positioning, GTM storyline; implementation roadmap, risk register, regulatory
pathway (APRA/ASIC/CDR as relevant). Skills: `cmo-positioning-gtm`,
`coo-delivery-risk-compliance`.

## P6 — Compose the integrated draft  *(the actual output of a run)*
Fold P1–P5 into **one AI-friendly draft** (Rule 5, 7, 10) in `/results/drafts/`:
- Context block (topic, framing, roster, how to use this file, double-check warning).
- The reasoning and claims for all five roles.
- Inline evidence with PROPOSED/VERIFIED state.
- A **per-person peer map**: for each member — the whole picture, their section, decisions
  made for them, what's open, their evidence, and how to defend it live.
- A "how Kunlin can check this" section listing every link/claim to verify.

Then run `course-alignment-check` against the draft and record blockers **inside** the draft.
Use the draft template in `/results/drafts/TEMPLATE-draft.md`.

## After the run — human loop (not automated)
1. **Kunlin verifies** each PROPOSED source → VERIFIED (Rule 13). Nothing approved while
   sleeping.
2. **Kunlin + team challenge** the draft (they drop the one file into any AI + send feedback).
3. Feedback comes back → you refine into the next `draft_YYYY-MM-DD-n.md`, and log the
   silent contribution marker (Rule 14) in `/private/`.
4. Repeat until stable → **build the deck first** (`pitch-deck-builder`), then **assemble the
   report** (`report-assembler`) from the same draft.

## Final gate (before submission)
`course-alignment-check` returns **READY**, then:
- Deck in **PPT** by 12:00 noon Wed, Week 10
- Pitch delivered live, Week 10 class
- Report as **PDF** by 21:00 Sun, Week 10
- Peer evaluation completed (informed by the private ledger, based on facts)

---

## Standing rule
After **any** refinement, re-run the voice pass (`report-assembler`) and
`course-alignment-check`. Five people editing is exactly how one voice becomes five.