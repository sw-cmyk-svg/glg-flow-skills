---
id: acq-principle-ltv-cac-heuristic
stage: acquisition
sub_stage: paid-acquisition
business_model: plg-saas
tactic_family: paid-acquisition
unit_type: principle
metric: [new_signups]
provenance: public
sources:
  - "David Skok, 'SaaS Metrics 2.0' (For Entrepreneurs blog, ~2010–2013) — origin of the LTV:CAC > 3 guideline, drawn from mature public SaaS companies."
  - "High Alpha, 2024 SaaS Benchmarks Report, p.33 'Net Revenue Retention Is a Key Growth Driver' — high-NRR (>106%) companies grow ~2.5x faster than low-NRR (<98%); p.38 CAC payback by stage (verified at primary)."
  - "Kyle Poyar / SaaS Benchmarks commentary — CAC payback and net revenue retention emphasized as predictors of profitable growth (supporting)."
---
**Principle — LTV:CAC ~3:1 is a rough first screen, not a target; prefer CAC payback and NRR.**

The "LTV:CAC should be at least 3:1" rule came from Skok's analysis of **mature public** SaaS companies
— ones with stable churn, multi-year lifetimes, and paybacks already under a year. Applied to an early
or cash-constrained company it misleads, because LTV is a long-horizon estimate that's highly sensitive
to churn assumptions and usually isn't discounted, so it flatters long-lived cohorts. Current practice
treats 3:1 as a **floor / sanity check, not a goal**, and leans on **CAC payback period and net revenue
retention** as the stronger, shorter-history predictors of profitable growth — and the data backs NRR
directly: high-NRR (>106%) companies grow about **2.5× faster** than low-NRR (<98%) ones (High Alpha
2024). A 4:1 ratio that takes five years to pay back is worse for a startup than a 3:1 that pays back in
ten months.

**How to apply.** Use LTV:CAC as a quick directional check, not the headline metric. For a client's
acquisition efficiency, lead with **CAC payback** (does the channel pay back fast enough to fund the
next cohort?) and read **NRR** alongside it. If you do quote LTV:CAC, state the churn/lifetime
assumptions behind the LTV, because the ratio moves far more on churn than on CAC.

**When it applies.** Any "is our acquisition efficient / is paid worth it" judgement, especially
early-stage where lifetime data is thin.

**Caution (honesty).** LTV:CAC has **no canonical spec id** — and neither does CAC; flag definitions.
Don't present an LTV-based ratio as proven unit economics for a young product; the lifetime is a
projection. Pairs with [[acq-benchmark-cac-payback]] (the metric to lead with) and
[[acq-principle-channel-saturation]].
