---
id: mde-sample-size
collection: methods
title: Minimum detectable effect & sample size
grade: A
sources:
  - ref: "Kohavi, Tang & Xu (2020), 'Trustworthy Online Controlled Experiments', Cambridge University Press — ch. 17"
    year: 2020
status: active
---

## Claim
Before running a test, compute the minimum detectable effect (MDE) from
available weekly traffic. Rule of thumb at 80% power, α=0.05, 50/50
split: n per variant ≈ 16 × σ² / δ² — for conversion metrics,
n ≈ 16 × p(1−p) / (p·MDE_rel)². If the honest MDE is larger than any
plausible effect, the test cannot succeed and should not run.

## Applicability — works when
- Binary or near-binary conversion metrics with stable baselines
- Traffic estimate uses the actual eligible population, not total visits

## Backfires when
- Applied to high-variance revenue-per-user metrics without variance
  reduction (CUPED or winsorizing) — sample sizes explode silently
- Baseline taken from a seasonal peak; the running test never matches it

## Growth applications
- Gate every proposed experiment on signup_rate / activation_rate with a
  computed MDE before it enters the backlog
- Scale-ups with <1,000 weekly eligible users: route to when-not-to-test

## Practice stance
Every experiment proposal must state its MDE and weeks-to-power. A
proposal without them is not a proposal; it is a wish. When weeks-to-power
exceeds 6, we recommend a reversible ship-and-watch instead (see
when-not-to-test).
