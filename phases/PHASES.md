# Phases and gates

Kunlin (CTO) drafts through P1–P5. The team refines from P6. Each phase has a **gate** —
do not proceed until it passes. Gates exist because a bad problem statement carried into
P5 costs a rewrite of everything downstream.

Timing assumes roughly three weeks remain before the Week 10 deadlines. Compress P1–P2
hard if the topic is not yet locked.

---

## P0 — Repository and knowledge base ✅
Course notes, `CLAUDE.md`, `STYLE.md`, skills, templates in place.
**Gate:** the team can open the repo and understand it without Kunlin explaining it.

## P1 — Topic lock
Carry 2–3 candidates, pick one. Decide the **framing**: entrepreneur pitching external
investors, *or* intrapreneur pitching senior management inside a bank. Everything downstream
depends on this.

Fill the terminology lock in `/STYLE.md` — the name for the customer, the product and the
problem. Locking vocabulary now is what makes the one-voice requirement achievable later.

**Gate:** a one-sentence problem statement in the form *[who] cannot [do what] because
[why], costing [what]* — plus the framing decision, written down.
**Skill:** `ceo-problem-market`

## P2 — Evidence pack
Everything sourced goes into `/evidence/EVIDENCE-LOG.md` **as it is found**. Market size,
competitors, regulatory constraints, comparable business models. No prose yet.

**Gate:** every claim the argument depends on has a source, or an explicit
`[NUMBER NEEDED]` with a named place to find it. Zero unsupported assertions.
**Skills:** `ceo-problem-market`, `cmo-positioning-gtm`

## P3 — Solution architecture and prototype scope
The CTO's real work. Cloud/data/API design, build-vs-partner, and the model justification
following the W3 property-valuation shape. Decide what actually exists by Week 10 versus
what is roadmap — and be honest about the line.

**Gate:** every named technology passes the four-part test (what / why over alternative /
cost and requirements / how validated). Prototype scope is buildable in the time left.
**Skill:** `cto-solution-architecture`

## P4 — Business model and financial model
Unit cost → volume → revenue → 5-year P&L → break-even → ROI → the ask. Built bottom-up,
with a separate assumptions tab.

**Gate:** a working spreadsheet exists in `/deliverables/financials/`. Every input traces
to the assumptions tab. A downside case exists.
**Skills:** `cfo-business-model-financials`, `coo-delivery-risk-compliance`

## P5 — Report draft
Spine first, then sections in spine order. Report **before** deck (CLAUDE.md Rule 5).

**Gate:** complete draft, page-counted, at or under 25 pages including title page. Every
section present. `course-alignment-check` run, blockers resolved.
**Skills:** `report-assembler`, plus the five role skills

## P6 — Extract the deck, hand over to the team
Pull the deck from the report. Assign slides and speakers. Then produce the five handover
packs and speaker briefs — this is where Kunlin's 50% ends and the team's 50% begins.

**Gate:** deck at 10–12 slides, script under ~750 words, five roughly equal speaking blocks,
and five handover packs each with a speaker brief.
**Skills:** `pitch-deck-builder`, all role skills for handover

## P7 — Refine, rehearse, submit
Team refines their sections. Kunlin re-runs assembly and the gate after their edits — the
voice will have drifted, it always does.

Rehearse the pitch repeatedly as a team; the convenor was emphatic on this. Time it.

**Gate:** `course-alignment-check` returns **READY**. Then:
- Deck in **PPT** by 12:00 noon Wednesday Week 10
- Pitch delivered live and in person, Week 10 class
- Report as **PDF** by 21:00 Sunday Week 10
- Peer evaluation completed, based on facts

---

## Standing rule
After **any** team member edits **any** section, re-run `report-assembler` voice pass and
`course-alignment-check`. Refinement by five people is exactly how a single-voice document
becomes five stitched-together ones.
