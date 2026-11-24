---
id: diagnose-cliff-walk-the-flow
collection: judgment
title: A silent drop-off is a context-break tell, not a friction diagnosis
grade: C
sources:
  - ref: "Galangal Lab practice experience — sportsbetting platform onboarding funnel, ~50% silent post-registration drop-off traced to a context-destroying cashier redirect"
    year: 2026
status: active
---

## Claim
When a funnel step shows a silent drop-off with zero downstream action — not
friction, not a slow trickle, but total disengagement — treat it as a tell
for a context break (the user was dumped somewhere disorienting), not
automatically as downstream friction (KYC, deposit form, pricing). The
funnel dashboard shows WHERE users leave; it never shows WHY. Before
theorizing, walk the flow yourself as a new user and do a competitor UX
teardown to see what normal looks like.

## Applicability — works when
- A funnel step shows a sharp, near-total drop with no partial completions
  or retries downstream — the signature of users being lost, not merely
  deterred
- You can walk the flow yourself as a fresh user (no seeded account, no
  internal shortcuts) to see exactly what a new user sees
- A competitor teardown is feasible and the client's category has visible
  competitors to benchmark navigational norms against

## Backfires when
- The real cause IS downstream friction (a broken KYC step, a confusing
  deposit form) — walking the flow and ruling this out is still required
  before concluding it's a context break; don't skip straight to "it must be
  a redirect"
- Over-indexing on competitor norms when the client's product context
  genuinely differs (regulatory constraints, a deliberately different flow)
  — "competitors don't do this" is corroborating evidence, not proof

## Growth applications
- A cliff between new_signups and time_to_activation with no partial funnel
  movement — walk the post-signup flow yourself before writing a friction
  hypothesis
- Segment activation_rate by immediate next action after signup; a spike of
  "zero subsequent action" users is the context-break signature to
  investigate firsthand
- Validate the fix with an experiment (redirect change, onboarding tour) and
  confirm the read via activation_rate lift before calling it solved

## Practice stance
We don't diagnose a behavioral cliff from the funnel alone. Every silent,
total drop-off gets a firsthand walkthrough and a competitor teardown before
we write a hypothesis, and every fix gets validated by an experiment against
activation_rate — "walked the flow and it felt off" is not sufficient
without a measured before/after.
