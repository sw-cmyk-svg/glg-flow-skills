---
id: verify-instrumentation-first
collection: judgment
title: Verify instrumentation before trusting a metric
grade: B
sources:
  - ref: "Galangal Lab practice experience — crypto-wallet client vanity acquisition metrics masking low downstream quality"
    year: 2026
  - ref: "Galangal Lab practice experience — sportsbetting + casino client, casino engagement undercounted by bad instrumentation, reversing the product's core strategic narrative"
    year: 2026
  - ref: "Galangal Lab practice experience — standard first-10-minute reconnaissance sequence run on every new client's analytics"
    year: 2026
status: active
---

## Claim
When two metrics that should move together diverge — or a number conveniently
confirms what everyone already believes — distrust the instrumentation before
the finding. Validate the measurement framework itself (event taxonomy,
funnel monotonicity, order-of-magnitude plausibility, cross-consistency
between related events) before running any real analysis on top of it, and
cross-check a suspicious number against an independent signal that isn't
subject to the same instrumentation bug.

## Applicability — works when
- Two metrics that should move together (e.g. revenue and reported
  engagement) diverge, or a metric conveniently confirms the client's
  existing strategic belief — a surprising-but-convenient number deserves
  more scrutiny, not less (Twyman's law)
- This is the first session with a client's analytics — before trusting any
  dashboard, walk the event taxonomy, then sanity-check funnel monotonicity
  (no step exceeds the step before it), order-of-magnitude plausibility of
  event counts, and cross-consistency between related events
- An independent, differently-instrumented signal exists to cross-check
  against (e.g. pre-registration behavior corroborating a post-registration
  number)

## Backfires when
- Over-distrust stalls analysis chasing a phantom instrumentation bug when
  the divergence is real and simply uncomfortable — not every reconciliation
  gap is a bug, some are the finding
- Treating every partial reconciliation gap as fatal, when small
  discrepancies are normal in any real analytics stack and don't warrant
  re-litigating the whole measurement framework

## Growth applications
- activation_rate and weekly_revenue should move directionally together; a
  sharp divergence is a cue to check instrumentation before reporting a win
  or a loss
- signup_rate and new_signups should reconcile; a mismatch points to a
  taxonomy or double-counting bug, not a growth signal
- paying_conversion reported at odds with observed engagement volume is a
  cue to verify the event definition, not to conclude pricing is broken

## Practice stance
Before any diagnostic work begins, we run the sanity pass — event taxonomy,
funnel monotonicity, order-of-magnitude checks, cross-consistency — and we
treat a convenient number with more suspicion than an inconvenient one. We
earn the right to distrust an instrument by finding the specific
reconciliation break (a redirect, an undercounted event, a taxonomy
mismatch); if a bounded check finds none, we accept the number and move on.
