---
name: pitch-deck-builder
description: Use when building or revising the Demo Day pitch deck, writing the hook, allocating slides, scripting the 5-minute presentation, dividing speaking time across five members, or rehearsing. Triggers include pitch deck, slides, demo day, hook, speaker notes, presentation script, and rehearsal.
---

# Demo Day pitch deck (10–12 slides, 5 minutes, 5 speakers)

Read `/CLAUDE.md` (**Rule 5**), `/course/00-assessment-spec.md` and
`/course/week-06-capstone-tutorial.md`.

## Precondition
**A stable integrated draft must exist first** in `/results/drafts/`. The deck is built
**before** the report, but both extract from the *same* draft — this skill does not
originate content. If asked to build the deck before a draft exists, say so and stop.
(CLAUDE.md Rule 5.) Every hook number must trace to a VERIFIED figure, not a PROPOSED one.

## Generating the PPTX (optional tool)
For native, editable PowerPoint output, the team may use **ppt-master**
(github.com/hugohe3/ppt-master — Python 3.10+, `pip install -r requirements.txt`; installable
as a Claude Code skill or standalone). It produces real editable PPTX (shapes/charts/tables),
which matches the "submit in PPT format" requirement. Vet the third-party code and check its
licence before an unattended run uses it. Content still comes from the draft; ppt-master only
renders it.

## Structure
hook → problem → solution → market opportunity → business model → team → **the ask**

## The hook
Slide 1 is a quantified, bottom-line-up-front benefit. Convenor's pattern:
"Enable 70% savings on…", "Improve customer access by 2-fold…",
"Enhance market prediction accuracy by 50%…".
The number must exist in the financial model. A hook the CFO cannot defend is a liability.

## Hard rules
- 10–12 slides. Fewer is acceptable; more is not.
- **5 minutes total.** At a comfortable pace that is roughly 700–750 spoken words across the
  whole team. Script it and time it — do not assume.
- **Heavy on visuals, little text.** The audience should watch the speaker, not read.
- **All five members speak roughly equally** — about 60 seconds each. Assign explicitly.
- Storytelling over data. High-level savings, ROI and break-even timing only; detail lives
  in the report.
- Consistent narrative and language across all slides, even though different members build
  different slides.

## Procedure
1. Extract from the stable integrated draft — never write new claims here.
2. Assign each slide an owner and a speaker; they need not be the same person, but the
   speaker must be able to defend it.
3. Write a script with word counts per speaker. Sum it. If over 750, cut.
4. Build handover points between speakers so the transitions are deliberate, not awkward.
5. Do not open with product features. Features bore an audience that has not felt the pain.
6. Produce speaker notes covering the likely follow-up question for each slide.
7. Submission: **PPT format, by 12:00 noon Wednesday of Week 10.** The pitch itself is live
   and in person — video is not accepted.

## Refuse to produce
- A deck built before a stable integrated draft exists.
- A text-dense slide.
- A speaking split where one member has materially more time.
- A hook number that does not appear in `/deliverables/financials/`.
