---
id: act-benchmark-tour-completion-by-steps
stage: activation
sub_stage: onboarding
business_model: plg-saas
tactic_family: friction-reduction
unit_type: benchmark
metric: [activation_rate]
provenance: public
sources:
  - "Produktly — SaaS Onboarding Benchmarks 2026 (464 companies, Jan–Jun 2026; SMB-skewed). https://produktly.com/research/saas-onboarding-benchmarks-2026"
verified: 2026-11-17
---
**Benchmark — product-tour completion falls sharply as step count rises.**

Across Produktly's 2026 data, median product-tour completion (distinct users reaching the
final step ÷ users who started) is **~29% per company** (p25 15%, p75 55%). Completion is
strongly correlated with **length**:

| Tour length | Median completion |
|---|---|
| 1–2 steps | **73%** |
| 3–5 steps | 38% |
| 6–8 steps | 25% |
| 9+ steps | **8%** |

Start type matters too: **user-initiated** tours complete at ~69% median vs ~23% for
**auto-started** ones.

**How to apply.** Keep onboarding tours short (≤5 steps) and prefer user-initiated over
forced auto-start. Longer, auto-triggered tours predict steep drop-off.

**Metric note — this is *not* `activation_rate`.** Tour completion is an onboarding-flow
leading indicator, not the activation event. Treat it as a proxy for onboarding friction,
not a substitute for the client's activation metric.

**Caution.** Produktly's base skews small/mid SaaS (enterprise underrepresented); the
step-count relationship is a correlation, not proof that cutting steps raises completion.
