---
name: draft-run
description: Use to run the whole capstone at once and produce ONE integrated draft. Triggers include "run everything", "do a draft run", "generate the draft", "run all phases", "new draft", "draft the project". Owner - orchestrator. Produces a single AI-friendly reasoning document in /results/drafts/, never a PPT and never the final report.
---

# Draft run — one integrated draft, all roles at once

This is the orchestrator. It does the whole project in a single run and composes it into
**one** self-contained draft, so Kunlin never has to run phases by hand or work out which
phase belongs to whom. Read `/CLAUDE.md` in full before starting.

## Hard stops (check first)
1. **Topic set** in `/config/team.md`? If not → STOP and ask Kunlin for the topic (Rule 11).
2. **Framing chosen** (entrepreneur / intrapreneur)? If not → flag; do not assume silently.
3. This run may **only draft**. It must not mark any evidence VERIFIED (Rule 13). If running
   autonomously/overnight, everything unconfirmed is tagged `[UNVERIFIED — Kunlin to confirm]`.

## Load
`/CLAUDE.md`, `/STYLE.md`, `/config/team.md`, `/phases/PHASES.md`, and the `/course/` files
relevant to the topic. Never write from general knowledge alone (Rule 1).

## Procedure
Work through the internal phases in `/phases/PHASES.md` (P1–P5), invoking the role skills:
- `ceo-problem-market`, `cmo-positioning-gtm`, `cto-solution-architecture`,
  `cfo-business-model-financials`, `coo-delivery-risk-compliance`.
Log every sourced fact to `/evidence/EVIDENCE-LOG.md` as **PROPOSED** as you go.

Then **compose one draft** (P6) from `/results/drafts/TEMPLATE-draft.md`:
- Copy it to `/results/drafts/draft_YYYY-MM-DD[-n].md` (next free suffix for today).
- Fill the context block, the plain-English spine, each role's reasoning, the inline
  claims+evidence table, the **per-person peer map**, and the "how Kunlin can check this"
  worklist.
- Keep it **AI-friendly and self-contained** (Rule 10): a teammate with only this file, and
  any AI model, must be guided correctly. Include the double-check warning.

Finally, run `course-alignment-check` against the draft and paste the result into section 7.

## Output contract
- Exactly one new file in `/results/drafts/`. Plain English. Not a PPT, not the report.
- All evidence PROPOSED (or `[UNVERIFIED]`). Nothing approved.
- Announce to Kunlin: the draft path, the open verification worklist, and the top
  weaknesses you'd challenge yourself.

## What this skill does NOT do
- It does not build the deck or the report (those come later, from the *stable* draft:
  `pitch-deck-builder` first, then `report-assembler`).
- It does not touch `/private/`.
- It does not decide the topic.