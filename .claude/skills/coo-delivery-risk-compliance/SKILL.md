---
name: coo-delivery-risk-compliance
description: Use when writing the implementation plan, operating model, delivery roadmap, resourcing, risk register, mitigation steps, regulatory and compliance analysis, or governance. Triggers include implementation, roadmap, risks, mitigation, compliance, APRA, ASIC, CDR, licensing, operational resilience, and governance. Owner - COO.
---

# Delivery, risk and compliance (COO)

Read `/CLAUDE.md`, `/course/week-07-regulation-governance.md` and
`/course/week-02-building-blocks.md`. The report explicitly requires
"challenges, risks and mitigation steps" — this section is not optional.

## Required outputs
1. **Implementation plan** — phased, with what exists at the end of each phase.
2. **Resourcing** — roles and headcount, feeding the CFO's cost model. Reconcile the two.
3. **Risk register** — risk, likelihood, impact, mitigation, owner.
4. **Regulatory analysis** — which obligations apply, which regulator, what the pathway is.
5. **Operating model** — how the thing actually runs day to day once live.

## Procedure
1. Classify risks using the **Judo three-class model**: **preventable / external /
   strategic** `[case: Judo]`. Preventable risks are managed by monitoring KPIs and people;
   external by forecasting and impact reduction; strategic by lowering probability while
   putting countermeasures in place.
2. If the architecture relies on third parties, third-party/concentration risk is a named
   top-five risk. APRA treats cloud platforms at the extreme end of the risk curve, yet
   approved Judo because risks were identified and mitigated **in advance** — mirror that
   posture `[case: Judo]`.
3. Map compliance to **both the data lifecycle and the model lifecycle** `[W7]`. For AI
   specifically: privacy by design, training vs operational data, prompt data,
   output accuracy.
4. Treat regulation as **strategy, not cost** `[W7]` — where a compliance capability is a
   differentiator, say so. This is a marks-earning move most teams miss.
5. Propose a **sandbox / supervisory engagement** pathway where a regulatory barrier exists
   `[W7]`. Regulators actively offer this; "we would seek approval" is not a mitigation,
   a named pathway is.
6. Incident response must be described as **rehearsed**, with the rehearsal cadence `[W7]`.
7. Governance must produce **evidence**: what was done, how results were measured, how the
   response was made `[W7]`.

## Refuse to produce
- A risk register where every mitigation is "monitor closely".
- "We will comply with all relevant regulations."
- An implementation plan with no dependency between phases.
- A timeline that ignores licensing or approval lead times.

## Handover
Write `/handover/COO.md` and a speaker brief. Include the single hardest question an
investor could ask about feasibility, and the answer.
