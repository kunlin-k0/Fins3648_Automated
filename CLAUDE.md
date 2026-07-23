# CLAUDE.md — FINS3648 Capstone (Fins3648_Automated)

You are assisting a five-person UNSW FINS3648 capstone team. Kunlin is the CTO and
produces the first draft; the other four refine it. These rules are **hard constraints**,
not preferences. If a request conflicts with them, say so and stop.

---

## RULE 1 — Course grounding is mandatory

Before producing any deliverable content, read the relevant file(s) in `/course/`.
Never write capstone content from general business knowledge alone.

Every substantive claim in any deliverable must resolve to exactly one of:

- **(a) Course concept** — cite as `[W<n>: <concept>]`, e.g. `[W2: CAPEX-to-OPEX]`.
  The concept must actually appear in `/course/week-0<n>-*.md`.
- **(b) External source** — a real, verifiable citation with author/publisher and year.
- **(c) Labelled assumption** — written inline as `[ASSUMPTION: <claim> — basis: <reasoning>]`.

There is no fourth category. If a sentence cannot be tagged (a), (b) or (c), delete it.
"It sounds right" is not a basis.

## RULE 2 — Never invent numbers

Do not generate market sizes, growth rates, adoption percentages, cost savings,
headcounts, or any other figure that is not either sourced or explicitly derived from
a stated assumption. Fabricated statistics in a submitted assessment are an academic
integrity breach, not a formatting slip.

If a number is needed and not available: write `[NUMBER NEEDED: <what> — <where to find it>]`
and move on. Do not fill the gap with a plausible-looking placeholder that could survive
into the final draft.

Derived figures must show their working in `/deliverables/financials/`.

## RULE 3 — No hand-waved technology

The course convenor stated explicitly that proposals saying "we leverage AI and it does
magic" are **far from acceptable**. Any technology choice — model, architecture, data
source, vendor — must state:

1. What it does in the solution.
2. Why it was chosen over at least one named alternative.
3. What it costs and what it requires (data, skills, latency, compliance).
4. How its output is validated or explained.

Justify model selection the way the Week 3/4 property-valuation case did it. If the team
cannot justify a component to that standard, the component is out of scope, not in.

## RULE 4 — Hard budgets (never exceed)

| Artefact | Limit |
|---|---|
| Final report | 25 pages **including title page**, excluding appendices and references |
| Report format | Word document, submitted as PDF |
| Pitch deck | 10–12 slides, visual-heavy, minimal text |
| Live pitch | 5 minutes total, all 5 members speaking roughly equally |
| Report authorship | ~5 pages of ownership per member |

Report and deck must be counted, not estimated. If content exceeds budget, cut — do not
shrink margins or fonts.

## RULE 5 — Report first, deck second

Build the full proposal, then extract the pitch from it. Never draft the deck first.
The convenor's guidance: draft the report, then pull key components out to form the pitch,
otherwise the deck and report will contradict each other.

## RULE 6 — One voice

The report must read as a single document, not five stitched together. Before any
drafting, load `/STYLE.md` and follow it exactly: Australian English, consistent
terminology, consistent citation style throughout, consistent heading structure.
Never mix citation formats.

## RULE 7 — Ownership is real

Each of the five sections has a named owner. When drafting on someone's behalf, also
produce their **speaker brief** (`/handover/TEMPLATE-speaker-brief.md`) so they can
defend the content live in the pitch and in Q&A. Never hand over prose without the
reasoning behind it.

## RULE 8 — Scope discipline

Only FINS3648 Weeks 1–7 content is in scope (`/course/`). Do not introduce frameworks,
vendors or concepts the course has not covered unless the team explicitly asks. Novel
external evidence is fine; novel *frameworks* dilute the course-alignment marks.

## RULE 9 — Run the gate before anything is called done

No deliverable is "finished" until `course-alignment-check` has been run against it and
all findings are resolved or explicitly accepted in writing.

---

## Working conventions

- Deliverables live in `/deliverables/`. Working notes live in `/evidence/`.
- Every sourced fact goes in `/evidence/EVIDENCE-LOG.md` **when found**, not later.
- Phase gates are in `/phases/PHASES.md`. Do not skip a phase gate.
- When uncertain about assessment requirements, `/course/00-assessment-spec.md` is
  authoritative over anything you remember.
