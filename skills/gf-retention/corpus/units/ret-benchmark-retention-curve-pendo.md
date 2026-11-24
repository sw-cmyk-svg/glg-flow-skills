---
id: ret-benchmark-retention-curve-pendo
stage: retention
sub_stage: retention-curve
business_model: plg-saas
tactic_family: engagement-depth
unit_type: benchmark
metric: [w1_retention, w4_retention, weekly_active_users]
provenance: public
sources:
  - "Pendo × Mind the Product — Global Product Benchmarks (6,800+ apps, 2,500 companies, Pendo One data, May 2023–Mar 2024), User retention section."
---
**Benchmark — the user-retention curve across 6,800+ products (Pendo × MTP).**

- **1-month retention: avg 38.8%; 3-month: avg ~30%.** "Add 100 active users, ~30 still return
  after three months (70 leave)."
- **By percentile (Month 1 / 2 / 3):** best-in-class 66.6 / 60.8 / **56.6%**; high 53.1 / 47.9 /
  44.3%; **average 38.3 / 33.0 / 30.1%**; low 23.6 / 19.4 / 16.8%. Best-in-class retain **1.7–1.9×**
  the average.
- **The curve flattens** from month 1 to 3 (the drop is steepest in month 1, then levels off). A
  curve that **flattens** is the sign of real value / product-market fit; one that keeps decaying is
  a leaky product (ties to [[ret-framework-retention-is-the-engine]]).
- **By industry:** Manufacturing (42.6% M1) and Consumer Goods (40.7%) highest; Financial and
  Government hardest to bring back. **By size:** small companies retain better early (40.2% M1), but
  large companies win by month 3.

**How to apply (Analyze/Benchmark).** Use ~38% as the 1-month reference and ~30% at 3 months, but the
**shape matters more than the level**: does the client's curve *flatten* (healthy — a returning
core) or keep *decaying* (no stickiness)? Always anchor to the client's own cohort.

**Caution.** Pendo "user retention" = **new visitors returning within month windows** (30 / 60 /
90-day return), which is **not** the spec's `w1_retention` / `w4_retention` (week-1 / week-4) — don't
compare the numbers naively. Userpilot's 1-month retention (46.9%) differs again (different
definition + sample), so treat cross-source figures as directional. Pairs with the
activation→retention link (`act-benchmark-activation-predicts-retention` in the activation corpus).
