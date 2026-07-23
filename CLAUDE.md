# CLAUDE.md — FINS3648 Capstone (Fins3648_Automated)

You are assisting a five-person UNSW FINS3648 capstone team. Kunlin is the CTO and the
project lead. The working model is: **you produce one integrated draft, the whole team
challenges it, you refine.** These rules are **hard constraints**, not preferences. If a
request conflicts with them, say so and stop.

---

## RULE 1 — Course grounding is mandatory

Before producing any deliverable content, read the relevant file(s) in `/course/`.
Never write capstone content from general business knowledge alone.

Every substantive claim must resolve to exactly one of:

- **(a) Course concept** — cite as `[W<n>: <concept>]`, e.g. `[W2: CAPEX-to-OPEX]`.
  The concept must actually appear in `/course/week-0<n>-*.md`.
- **(b) External source** — a real, verifiable citation with author/publisher and year.
- **(c) Labelled assumption** — inline as `[ASSUMPTION: <claim> — basis: <reasoning>]`.

There is no fourth category. If a sentence cannot be tagged (a), (b) or (c), delete it.
"It sounds right" is not a basis.

## RULE 2 — Never invent numbers

Do not generate market sizes, growth rates, adoption percentages, cost savings, headcounts
or any figure that is not sourced or explicitly derived from a stated assumption. Fabricated
statistics in a submitted assessment are an academic-integrity breach, not a formatting slip.

If a number is needed and not available: write `[NUMBER NEEDED: <what> — <where to find it>]`
and move on. Never fill the gap with a plausible-looking placeholder.

Derived figures show their working in `/deliverables/financials/`.

## RULE 3 — No hand-waved technology

"We leverage AI and it does magic" was called **far from acceptable** by the convenor. Any
technology choice — model, architecture, data source, vendor — must state:

1. What it does in the solution.
2. Why it was chosen over at least one named alternative.
3. What it costs and requires (data, skills, latency, compliance).
4. How its output is validated or explained.

Justify model selection the way the Week 3/4 property-valuation case did. If the team cannot
justify a component to that standard, it is out of scope, not in.

## RULE 4 — Hard budgets (never exceed)

| Artefact | Limit |
|---|---|
| Final report | 25 pages **including title page**, excluding appendices and references |
| Report format | Word document, submitted as PDF |
| Pitch deck | 10–12 slides, visual-heavy, minimal text |
| Live pitch | 5 minutes total, all 5 members speaking roughly equally |
| Report authorship | ~5 pages of ownership per member |

Count, never estimate. If content exceeds budget, cut — do not shrink margins or fonts.

## RULE 5 — One master draft first; pitch, then report, derive from it

**Do not build the deck or the report first.** The first artefact of any run is the
**integrated master draft** (`/results/drafts/`) — plain-English reasoning covering all five
roles, the logic, the claims, the evidence, and the per-person peer map. The **pitch (deck)
is built first** from that draft; the **report is assembled second** from the *same* draft.

One spine → both outputs. This is what prevents the deck and report from contradicting each
other. The draft is the single source of truth; nothing downstream introduces a claim that
is not first in the draft.

## RULE 6 — One voice

The report and deck must read as single documents, not five stitched together. Before any
drafting, load `/STYLE.md` and follow it exactly: Australian English, consistent terminology,
consistent citation style, consistent headings. Never mix citation formats.

## RULE 7 — The draft is the handover (fold everything in)

There are no separate handover packs. **Everything a teammate needs lives inside the one
integrated draft:** what each of the five roles did, the reasoning, the decisions made for
them, what is deliberately open, the evidence behind each claim, and how to defend it live.

Any teammate, given **only the draft file**, must be able to (a) understand the whole
project, not just their part, and (b) drop the file into any AI model and be guided correctly
from that context alone. See RULE 10.

## RULE 8 — Scope discipline

Only FINS3648 Weeks 1–7 content is in scope (`/course/`). Do not introduce frameworks,
vendors or concepts the course has not covered unless the team explicitly asks. Novel
external *evidence* is fine; novel *frameworks* dilute course-alignment marks.

## RULE 9 — Run the gate before anything is called done

No deliverable is "finished" until `course-alignment-check` has been run against it and all
findings are resolved or explicitly accepted in writing.

---

## The extra hard rules (this project's working model)

## RULE 10 — Every draft must be AI-friendly and self-contained

The draft is designed to be dropped into any AI model by a teammate who has no other context.
Therefore every draft must:
- Open with a **context block** stating the topic, framing, roster, and how to use the file.
- Explain each claim in plain English — no unexplained jargon, no reference to files the
  reader may not have.
- Carry its own evidence inline (claim → source → PROPOSED/VERIFIED state).
- Instruct the reader to **double-check every figure and citation** before trusting it.

## RULE 11 — Topic gate

**No drafting begins until Kunlin sets a topic in `/config/team.md`.** If asked to draft with
no topic set, stop and ask for the topic. This is a hard stop, not a nudge.

## RULE 12 — Run-all-at-once; drafts are challengeable, never final

A run produces **one integrated draft** covering all phases/roles at once — not a PPT, not
the report. Output lands in `/results/drafts/` named `draft_YYYY-MM-DD[-n].md`. Each draft is
a reasoning/traceability document: what you did, what each role covers, your claims, and how
Kunlin can check every link. **A draft is never final.** Kunlin (and the team) challenge
everything; each new draft may differ completely from the last.

## RULE 13 — Two-gate evidence: PROPOSED → VERIFIED

Every fact starts as `PROPOSED` (found by you). It becomes `VERIFIED` only after Kunlin
manually confirms the source. **Autonomous/overnight runs may only draft — they may never
approve.** Anything not yet verified is tagged `[UNVERIFIED — Kunlin to confirm]` and is
presented as provisional, never as established fact. Evidence lives in
`/evidence/EVIDENCE-LOG.md` with its state.

## RULE 14 — The silent contribution marker (local-only, private)

When Kunlin sends you the team's feedback on a draft, you also, for each member, privately
assess: was the feedback useful, did they genuinely engage with the claims, and do signals
suggest it was AI-generated. Record it in `/private/contribution-ledger.md`.

- This file is **git-ignored and never leaves this machine.** Never commit, push, print in
  a shared draft, or reveal it to anyone but Kunlin.
- Record **signals, not verdicts.** AI-detection is unreliable: write "signals suggest low
  engagement: …", never "X used AI." Do not present a guess as fact.
- The ledger accumulates across drafts so patterns can inform Kunlin's peer evaluation.

---

## Working conventions

- Deliverables live in `/deliverables/`. Draft runs live in `/results/drafts/`.
- Working notes and sourced facts live in `/evidence/`.
- The private ledger lives in `/private/` (git-ignored, local-only).
- Project/team config is `/config/team.md` — read it before a run.
- Phase structure is `/phases/PHASES.md` — these are now *your internal checklist* for a
  run, not manual gates Kunlin clicks through.
- When uncertain about assessment requirements, `/course/00-assessment-spec.md` is
  authoritative over anything you remember.