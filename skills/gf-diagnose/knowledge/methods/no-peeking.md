---
id: no-peeking
collection: methods
title: No peeking — stopping rules and repeated significance testing
grade: A
sources:
  - ref: "Johari, Koomen, Pekelis & Walsh (2017), 'Peeking at A/B Tests: Why It Matters, and What to Do About It', KDD"
    year: 2017
status: active
---

## Claim
Repeatedly checking significance and stopping the first time p<0.05
appears severely inflates the false-positive rate — it can exceed 25%
against a nominal 5% threshold. Use a fixed sample size decided before
launch, or a proper always-valid / sequential testing method built for
continuous monitoring; casual daily peeking with a fixed-horizon test is
neither.

## Applicability — works when
- A sample size and stopping date are fixed and documented before the
  test launches, or a true sequential method (e.g., mSPRT, group
  sequential design) is used from the start
- Dashboards are used for health monitoring only, with decisions deferred
  to the pre-registered stopping rule

## Backfires when
- Sequential/always-valid methods buy flexibility at a power cost — they
  are not free; naive Bonferroni correction on daily peeks overcorrects
  into uselessness and buries real effects
- Anyone with dashboard access can informally peek and unilaterally call
  a result — a governance failure that no statistical method fixes
- Multiple corrections get stacked (a sequential method plus ad hoc
  Bonferroni on top) and the test becomes unable to detect anything

## Growth applications
- Pre-register a fixed sample size and stopping date for signup_rate
  tests, tied to the MDE calculation, and lock the decision until it's
  reached (see mde-sample-size)
- Use an always-valid sequential method for activation_rate tests when
  faster reads matter more than the extra sample the power cost requires
- Monitor new_signups daily as a guardrail only — the go/no-go call is
  made once, at the pre-registered horizon, not on any earlier day

## Practice stance
We commit to a fixed-horizon or a true sequential design in writing
before a test launches, and we refuse to let an early "it looked
significant" override the pre-registered stopping rule. Wanting to call a
test early is a signal to design a sequential test next time — not a
reason to break the current one's rules.
