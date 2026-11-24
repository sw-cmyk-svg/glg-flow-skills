---
id: act-benchmark-time-to-value-saas
stage: activation
sub_stage: aha
business_model: plg-saas
tactic_family: friction-reduction
unit_type: benchmark
metric: [time_to_activation, activation_rate]
provenance: public
sources:
  - "Pendo × Mind the Product — Global Product Benchmarks (6,800+ apps, 2,500 companies, Pendo One data, May 2023–Mar 2024)."
---
**Benchmark — time to value (TTV) across 6,800+ products (Pendo × MTP).**

TTV by percentile (days to the product's top "aha" / Core Event; **lower is better**):
- **Low (25th): 2.6** · **Average (50th): 1.5** · **High (75th): 0.7** · **Best-in-class (90th):
  0.2** (≈ **4.8 hours**). Best-in-class products get users to value **~7.5× faster** than
  average.
- **By company size (avg):** Small 1.2 · Medium 1.6 · Large 1.5 days; the top 10% of large
  companies are **12× faster** than the average large org.
- **By industry:** all-industry avg **1.6 days**; Media & Government fastest at **1.1 days**.

**Cross-source corroboration.** Pendo's **1.5-day average** lines up with Userpilot's independent
**~1 day 12 hours** ([[act-benchmark-activation-rate-saas-2025]]) — two large datasets agreeing
strengthens ~1.5 days as the PLG-SaaS TTV prior.

**How to apply (Analyze/Benchmark).** Treat **~1.5 days** as the median reference and **sub-24h**
as strong; measure to the client's own top Core Event, not a generic signal. The report's levers
for shortening TTV: in-app guidance toward Core Events, replicating the behaviors of fast
activators, and lowering onboarding friction.

**Caution.** Pendo measures TTV as **average days** from first login to accomplishing the top
**Core Event** (each product's own ≤10 key features), vs the spec's `time_to_activation` (**median
hours** to the activation event) — don't compare the numbers naively. Cross-industry data, so
adjust by vertical.
