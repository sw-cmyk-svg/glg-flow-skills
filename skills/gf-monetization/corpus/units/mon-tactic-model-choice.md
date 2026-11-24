---
id: mon-tactic-model-choice
stage: monetization
sub_stage: pricing-model
business_model: plg-saas
tactic_family: pricing-model
unit_type: tactic
metric: [paying_conversion, weekly_revenue]
provenance: public
sources:
  - "General PLG monetization practice (Reforge / OpenView lineage); conversion figures from the ChartMogul × ProductLed × Poyar SaaS Conversion Report (2026) — see mon-benchmark-free-to-paid-conversion."
---
**Tactic — choose the acquisition-to-paid model that fits the product: freemium, free trial, or reverse trial.**

Three common ways to get a user to paid, each with a trade-off (figures:
[[mon-benchmark-free-to-paid-conversion]]):
- **Freemium** (a free tier forever): great for top-of-funnel reach, but it's an **acquisition model,
  not a revenue model** — free-to-paid conversion is **low (~2–6%)**. It makes up for it with volume
  (roughly 2× the signups of a trial). Works when the free tier is cheap to serve and the product has a
  natural upgrade trigger.
- **Free trial** (full product, time-limited): higher *rate* than freemium, but the edge largely
  washes out once you account for signups. **Opt-in** trials (no card) convert around **~8–9%**;
  **opt-out** trials (card up front) much higher (~**30%**, >5× opt-in) but with more involuntary churn
  and goodwill risk.
- **Reverse trial** (start with full/premium access, then drop to free or paid): blends freemium reach
  with trial conversion — the user feels the premium value before deciding.

**How to apply.** Match the model to the product: freemium when reach and virality matter and the free
tier is cheap; free trial when the product's value lands fast within a trial window; reverse trial when
you want both. Align the free/paid line to the value metric, not to arbitrary features.

**When it applies.** Designing or changing the acquisition-to-paid motion.

**Caution (ethics).** Opt-out (card-required) trials must make the **charge date and cancellation
clear and easy** — surprise first-charges and hard cancels are dark patterns and increasingly unlawful
(auto-renewal / click-to-cancel rules). Pairs with [[mon-tactic-paywall-placement-timing]] and
[[mon-principle-present-bias-deferral]].
