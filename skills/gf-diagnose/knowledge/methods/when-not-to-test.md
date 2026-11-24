---
id: when-not-to-test
collection: methods
title: When not to test — reversible bets under low traffic
grade: B
sources:
  - ref: "Kohavi, Tang & Xu (2020), 'Trustworthy Online Controlled Experiments', Cambridge University Press — power math applied to low-traffic products"
    year: 2020
status: active
---

## Claim
Below roughly 1,000 weekly eligible users per variant, most conversion
tests are underpowered for any realistic effect size (see
mde-sample-size). Below that threshold, ship reversible bets instead —
changes behind a flag or easy rollback, with a pre-registered guardrail
metric and rollback criteria — rather than running a test that cannot
conclude.

## Applicability — works when
- Weekly eligible traffic for the funnel step is under ~1,000 per
  variant and the honest MDE exceeds any plausible effect size
- The change is reversible (feature flag, config toggle, easy rollback)
  and has a clear guardrail metric to watch after launch

## Backfires when
- Cargo-culting "test everything" stalls low-traffic products for
  quarters, waiting on tests that could never conclude; equally, "we
  can't test" must not become "ship anything without measurement" —
  guardrails and a pre/post read still apply
- The reversible-bet label is used to skip experimentation on changes
  that are cheap and fast enough to test properly

## Growth applications
- Ship reversible pricing-page changes with paying_conversion as a
  guardrail metric and a pre-registered rollback trigger, instead of a
  test the traffic can't power
- Route low-traffic activation_rate ideas to qualitative research
  (usability sessions, session replay) instead of a doomed A/B test
- Pre-register a rollback threshold on weekly_revenue before shipping a
  reversible change without a formal control group

## Practice stance
Below the power threshold, we ship with a pre-registered guardrail metric
and rollback criteria instead of running a test we already know can't
conclude — that is a decision, not an absence of rigor. We refuse to let
low traffic become an excuse to skip measurement altogether; every
reversible bet still gets a before/after read.
