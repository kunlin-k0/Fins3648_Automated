---
name: cto-solution-architecture
description: Use when designing the solution architecture, selecting models or technologies, defining data pipelines and APIs, specifying cloud deployment, scoping the prototype, or writing the technology building blocks section. Triggers include architecture, tech stack, model selection, data pipeline, API design, prototype scope, and MLOps. Owner - CTO (Kunlin).
---

# Solution architecture and technology building blocks (CTO)

Read `/CLAUDE.md` (especially **Rule 3**), `/STYLE.md`, `/course/week-02-building-blocks.md`
and `/course/week-03-ai-genai-foundations.md` before writing.

## Required outputs
1. **Architecture diagram** — mapped to the W2 triad: **CLOUD / DATA / APIs**.
2. **Build-vs-partner table** — what is core and built, what is subscribed. Justify each.
3. **Model justification** — see procedure below. This is the highest-risk section in the
   whole report.
4. **Data architecture** — sources, pipeline, storage, privacy, governance `[W2]`.
5. **Prototype scope** — what will actually exist by Week 10, and what is roadmap.
6. **Deployment** — hybrid/multi-cloud posture, scaling path, cost driver.

## Model justification procedure (mandatory — CLAUDE.md Rule 3)
Follow the shape of the W3 property fair-value case:
1. State the prediction or generation task precisely.
2. State the data available: type, volume, structure, provenance, refresh rate.
3. Name **at least two candidate approaches**, including a deliberately simple baseline
   (rules or regression). A baseline you can beat is stronger evidence than a complex model
   you assert.
4. State selection criteria — accuracy, latency, explainability, cost, data requirement,
   regulatory acceptability — and which criterion dominates and why.
5. State how the output is **validated and explained**, and what the failure mode looks like.
6. State the guardrails `[W3]`: RAG, prompt engineering/chaining, value alignment,
   human-in-the-loop — and which apply here.
7. Align technical metrics to **financial KPIs** `[W3: MLOps]`. An accuracy number with no
   P&L consequence is not an argument.

## Architecture principles to apply explicitly
- Modular microservices over monolith; event-driven where real-time matters `[W2]`.
- **API-first**; API-as-gatekeeper for partner connections `[W2]`.
- **Compliance and security by design**, with auditability and explainability `[W2]`.
- **CAPEX-to-OPEX** via cloud `[W2]` — the core cost argument.
- Build core strength, partner for standard functions (payments, KYC) `[W2]`.
- If proposing full EaaS, carry the Judo third-party risk analysis with it — the strategy
  and its risks are inseparable `[case: Judo]`.

## Refuse to produce
- Any technology named without justification, cost and validation.
- "AI-powered" as a description of a component.
- An architecture with no stated failure mode.
- A prototype scope that could not be built in the remaining weeks.

## Handover
Kunlin owns this section directly. Still write `/handover/CTO.md` recording decisions and
rejected alternatives — the rejected options are what make the section defensible in Q&A.
