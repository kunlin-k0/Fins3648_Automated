---
name: contribution-marker
description: Use ONLY when Kunlin pastes the team's feedback on a draft, to privately assess and record each member's contribution. Triggers include "here's the team's feedback", "log the feedback", "record contributions", "team responded". Private and local-only - never shared. Owner - Kunlin only.
---

# Silent contribution marker (private, local-only)

When Kunlin sends the team's feedback on a draft, record each member's engagement in
`/private/contribution-ledger.md`. This is Kunlin's private record for peer evaluation.
Read `/CLAUDE.md` Rule 14 before writing.

## Absolute constraints
- **Never leaves this machine.** `/private/` is git-ignored. Never commit, push, or copy its
  contents into a shared draft, the report, the deck, or any message to a teammate.
- **Never reveal its existence** to anyone but Kunlin.
- **Signals, not verdicts.** AI-detection is unreliable. Write "signals suggest low
  engagement: …", never "X used AI." Never present a guess as fact.

## What to assess, per member
For the feedback each member gave on this draft:
1. **Useful?** — did it actually improve the draft, or was it cosmetic?
2. **Engaged?** — did they respond to the *specific* claims, or generically?
3. **AI-signal?** — do phrasing/patterns *suggest* AI-generated feedback? Signal only.

## Procedure
1. Open `/private/contribution-ledger.md`.
2. Add a new dated section for this feedback round (match the draft filename).
3. Fill one row per member with short, factual notes. Cite what they actually said.
4. Update the "Running patterns" section if a trend is now visible across drafts.
5. Confirm to Kunlin privately that it is logged. Do **not** summarise the judgements in any
   channel that a teammate could see.

## Then
Hand the *substantive* feedback (not the private assessment) to `draft-run` or the relevant
role skill to produce the next refined draft.