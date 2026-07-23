---
name: course-alignment-check
description: Use to audit any capstone deliverable before it is called finished - checking that claims are sourced or assumption-tagged, technology choices are justified, page and slide and time budgets are met, course concepts are correctly grounded, and voice is consistent. Triggers include check this, review before submission, audit, is this ready, and quality gate.
---

# Course alignment gate

This is the last skill run before anything is called done (CLAUDE.md Rule 9). It does not
write content. It finds problems and reports them. Be adversarial — mark this the way a
sceptical convenor would.

## Audit sequence

### 1. Evidence audit
Go sentence by sentence through substantive claims. Every one must carry `[W<n>: concept]`,
a real citation, or `[ASSUMPTION: … — basis: …]`.
- **FAIL** any untagged claim.
- **FAIL** any `[W<n>: X]` where X does not actually appear in `/course/week-0<n>-*.md`.
  Miscited course concepts are worse than no citation.
- **FAIL** any number with no source and no assumption basis.
- Report `[NUMBER NEEDED]` and `[TBD]` markers as blockers, not notes.

### 2. Technology audit (CLAUDE.md Rule 3)
For every technology or model named, confirm all four exist: what it does, why over a named
alternative, cost and requirements, how output is validated.
- **FAIL** on "AI-powered", "leverages machine learning", "intelligent automation" used as
  descriptions rather than claims.
- **FAIL** if no simple baseline was considered.

### 3. Budget audit
- Report: count pages. 25 max including title page, excluding appendices and references.
- Deck: count slides. 10–12.
- Script: count words. ~750 max across five speakers.
- Speaking: check the split is roughly even.
- Report ownership: roughly 5 pages per member, recorded.

### 4. Voice audit
Read end to end. Flag: US spelling, first person, mixed citation formats, inconsistent
terminology against the `/STYLE.md` lock, tonal shifts at section boundaries, banned
consultant filler.

### 5. Consistency audit
Every number in the report and deck matches `/deliverables/financials/`. The deck's hook
number is defensible. The COO's headcount matches the CFO's cost model. The implementation
timeline matches the ask.

### 6. Rubric audit
Against `/course/00-assessment-spec.md`: are all required report sections present? Is the
introduction genuinely big-picture-to-specific? Does the solution section cover solution,
evidence and logic, business model, technology building blocks, **and** challenges/risks/
mitigation? Is implementation realistic rather than futuristic?

### 7. Case audit
Is every course case used for what it is actually good for (`/course/cases.md`)? Is Kabbage
cited on both sides? Is Judo's EaaS argument carrying its risk analysis with it?

## Output format
A findings table: severity (BLOCKER / MAJOR / MINOR), location, what is wrong, what fixes it.
End with a single verdict line: **READY** or **NOT READY**, and if not ready, the count of
blockers. Do not soften. A gate that passes everything is not a gate.
