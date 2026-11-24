---
id: mon-benchmark-involuntary-churn
stage: monetization
sub_stage: revenue-retention
business_model: plg-saas
tactic_family: revenue-retention
unit_type: benchmark
metric: [weekly_revenue, paying_conversion]
provenance: public
sources:
  - "Stripe data (involuntary churn share, by segment and order value), reported by Churnkey — 'Involuntary churn benchmarks'. Recovery figures: Churnkey / Stripe Smart Retries."
---
**Benchmark prior — about a fifth of SaaS churn is involuntary (failed payments), and much is recoverable.**

A large, often-ignored slice of churn is **involuntary** — cards that expire, decline, or hit limits,
not customers choosing to leave. Stripe data (via Churnkey): involuntary churn is **~22% of total SaaS
churn** (higher for low-price / B2C: ~24% B2C vs ~16% B2B; ~35% for sub-$10 order values). It's
recoverable: payment **retries recover ~51–55%** of failed payments, dunning emails add a few points
each, and a full recovery stack (retries + dunning + a failed-payment wall) can recover **~70%** of
involuntary churn.

**How to use.** Before chasing voluntary churn with product changes, check how much of the client's
churn is **failed payments** — if it's ~20%+, fixing dunning/retries is often the fastest revenue win
and purely operational. Split involuntary from voluntary churn in any churn read.

**Definition caveat.** Figures vary by billing model, price point, and whether churn is measured by
logo or by revenue. The ~22% is a traceable Stripe-based average, not a universal constant.

**When it applies.** Any revenue-churn diagnosis. Pairs with [[mon-tactic-dunning-recovery]].
