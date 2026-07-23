---
name: report-assembler
description: Use when assembling, merging, editing, formatting or page-counting the 25-page capstone report, harmonising voice across sections, building the section spine, or preparing the Word/PDF submission. Triggers include assemble the report, merge sections, page count, table of contents, consistent voice, and final draft.
---

# Report assembly (25 pages, one voice)

Read `/CLAUDE.md`, `/STYLE.md` and `/course/00-assessment-spec.md`. This skill owns the
page budget and the voice. It has authority to cut.

## The spine (fixed order — W6 narrative flow)
1. Title page *(counts toward 25)*
2. Executive summary
3. **Introduction** — big picture → the specific problem
4. Problem and market opportunity — size, why unsolved, why now *(CEO)*
5. **Proposed solution** — what it is, evidence and thought logic *(CTO + CMO)*
6. Technology building blocks — cloud / data / APIs, model justification *(CTO)*
7. Business model and financials — revenue, unit economics, 5-year P&L, ROI *(CFO)*
8. Go-to-market and positioning *(CMO)*
9. Implementation, challenges, risks and mitigation *(COO)*
10. Team — why this team *(CEO)*
11. The ask *(CFO)*
12. **Conclusion** — restate problem and solution
13. References *(does not count)*
14. Appendices *(do not count)*

## Procedure
1. **Count pages, do not estimate.** 25 includes the title page and closing page and
   excludes appendices and references.
2. When over budget, cut in this order: (i) repetition across sections, (ii) background
   the marker already knows, (iii) detail that belongs in an appendix, (iv) figures that
   duplicate text. Never shrink fonts or margins.
3. **Voice pass** — read the whole document end to end for: Australian English, third
   person, consistent terminology (check `/STYLE.md` terminology lock), consistent heading
   case, consistent citation format. Rewrite any section that reads differently.
4. **Consistency pass** — every number in the report must match
   `/deliverables/financials/`. Every figure numbered and referenced in text.
5. **Ownership pass** — confirm each of the five members owns roughly 5 pages, and record
   who owns what. Peer evaluation depends on this being real.
6. Push all prototype screenshots, diagrams, code and user journeys to appendices.
7. Final format: Word document, exported to **PDF** for submission.

## Refuse to produce
- A "final" report that has not been page-counted.
- Sections in different voices with a note saying the team will harmonise later.
- A submission that has not passed `course-alignment-check`.
