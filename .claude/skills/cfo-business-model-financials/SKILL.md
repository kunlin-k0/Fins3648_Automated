---
name: cfo-business-model-financials
description: Use when building the business model, revenue streams, unit economics, cost structure, P&L projections, break-even analysis, ROI, funding requirement or the ask. Triggers include financial model, unit cost, pricing, five-year forecast, break-even, ROI, and how much are we raising. Owner - CFO.
---

# Business model and financials (CFO)

Read `/CLAUDE.md` (**Rule 2** especially), `/course/00-assessment-spec.md` and
`/course/week-06-capstone-tutorial.md`. The convenor expects a real spreadsheet, not prose
about money.

## Required outputs (all in `/deliverables/financials/`)
1. **Revenue model** — every stream named, with the pricing mechanism and who pays.
2. **Unit cost of the technology solution** — explicitly required by the convenor.
3. **5-year P&L** — revenue minus cost, by year. Three years is usually too short to reach
   break-even; five is the expectation.
4. **Break-even point and ROI**.
5. **Scale economics** — how unit cost falls with volume, and why.
6. **The ask** — amount, use of funds, what it buys, what milestone it reaches.

## Procedure
1. Build **bottom-up**: unit cost first, then volume, then revenue. Top-down revenue targets
   with reverse-engineered costs are transparent to a marker.
2. Every input is a labelled assumption with a basis. The spreadsheet needs an explicit
   **assumptions tab** — inputs separated from calculations, no hardcoded numbers inside
   formulas.
3. Expect the realistic shape: **early losses, then a scalable profit curve**. A model that
   is profitable in year one is a red flag, not a strength.
4. Cloud consumption is OPEX that scales with usage `[W2: CAPEX-to-OPEX]` — model it as
   variable cost, not fixed. This is where most student models go wrong.
5. Run at least a downside case. State what breaks the model.
6. If monetising fee income rather than lending spread, anchor on the W5 profit-pool point.
7. If the model is BNPL/BaaS/PaaS, name it and use that model's standard economics `[W4]`.

## Refuse to produce
- Any figure not traceable to the assumptions tab.
- A hockey-stick with no mechanism explaining the inflection.
- A "conservative estimate" that is neither conservative nor estimated.
- Numbers in the deck that disagree with the spreadsheet.

## Handover
Write `/handover/CFO.md` and a speaker brief. The brief must state, in one line each: the
three numbers most likely to be challenged, and the defence of each.
