---
id: act-benchmark-activation-rates-by-percentile
stage: activation
sub_stage: onboarding
business_model: plg-saas
tactic_family: friction-reduction
unit_type: benchmark
metric: [activation_rate]
provenance: public
sources:
  - "Amplitude — 2026 Product Benchmark Report (2,500+ companies). https://amplitude.com/resources/2026-product-benchmark"
verified: 2026-11-17
---
**Benchmark — day-N activation rates (Amplitude 2026 percentiles).**

| | Day 1 | Day 14 |
|---|---|---|
| Typical (50th) | 4.3% | 1.3% |
| Top (90th) | 20.7% | 8.9% |

For half of all products, ~99% of new users are no longer active two weeks after their
first action. Day-7 activation slipped in every industry year-over-year, and the "activate
5% by day 7 → top-quartile retention" threshold fell from 7% (prior year) to 5%.

**How to apply.** Use as a rough sanity band for how steeply early-return activation
decays — "top" is roughly 5× "typical." A young product's absolute numbers will look low in
this measure; that is normal, not a crisis.

**Definition caveat.** Same as [[act-benchmark-activation-predicts-retention]] — Amplitude's
activation is day-N *return*, not the spec's event-based `activation_rate`. Use for shape,
not as the client's target number.
