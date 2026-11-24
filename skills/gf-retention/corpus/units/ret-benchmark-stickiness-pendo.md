---
id: ret-benchmark-stickiness-pendo
stage: retention
sub_stage: habit
business_model: plg-saas
tactic_family: habit-formation
unit_type: benchmark
metric: [weekly_active_users]
provenance: public
sources:
  - "Pendo × Mind the Product — Global Product Benchmarks (6,800+ apps, 2,500 companies), Stickiness section."
---
**Benchmark — stickiness (WAU/MAU, DAU/MAU) across 6,800+ products (Pendo × MTP).**

Stickiness = the share of a month's users who come back **weekly** (WAU/MAU) or **daily** (DAU/MAU).
It's a **leading indicator of retention and habit**.

- **Average: WAU/MAU 53%, DAU/MAU 16%.** **Best-in-class: 77% / 38%** (the top 10% are ~**1.5×**
  stickier). By percentile — low 41% / 10%, average 53% / 16%, high 67% / 26%, best-in-class 77% / 38%.
- **Pick the denominator to the product's natural frequency:** watch **weekly** stickiness for
  infrequent-task products (e.g. expense tools), **daily** for products meant for daily use
  (productivity, messaging). Measuring daily stickiness on a weekly product makes a healthy product
  look broken.
- **Stickiness tracks feature adoption:** the stickiest industries (Manufacturing, Consumer Goods
  ~55% WAU/MAU) also have the highest feature adoption and retention — the more value users get from
  features, the more they return. Government/Education are least sticky.

**How to apply (Analyze/Recommend).** Use ~53% WAU/MAU as the reference, with the right cadence for
the product. Low stickiness **plus** low feature adoption points to an **engagement-depth** problem
(users aren't finding enough value to come back), not just a reminder problem. Pendo's own levers:
encourage engagement (triggers), replicate the behaviours of the most engaged users, and guide
at-risk users to value.

**Caution.** Stickiness is a **ratio** (WAU/MAU), not the spec's raw `weekly_active_users` count;
"active" = any event in the period (Pendo's definition). A reminder/notification lever here carries
the ethics caution — frequency and consent matter; don't manufacture engagement with notification
spam ([[ret-tactic-reengagement-lifecycle]]). Pairs with [[ret-benchmark-retention-curve-pendo]].
