---
id: mon-benchmark-free-to-paid-conversion
stage: monetization
sub_stage: free-to-paid
business_model: plg-saas
tactic_family: free-to-paid
unit_type: benchmark
metric: [paying_conversion]
provenance: public
sources:
  - "ChartMogul × ProductLed × Kyle Poyar — SaaS Conversion Report (survey Jan 2026, 200 B2B software products)."
  - "RevenueCat — State of Subscription Apps 2024 (30K+ apps, $6.7B+ tracked revenue) — MOBILE apps, cited as a comparator only."
---
**Benchmark prior — free-to-paid conversion by model (B2B SaaS figures, verified).**

Reference points for a signup cohort converting to paid, from the ChartMogul/ProductLed SaaS
Conversion Report (200 B2B software products, 2026):
- **Median free-to-paid across all products: ~8%** (within 6 months of signup) — though "very few
  products actually sit at exactly 8%".
- **Freemium → paid:** ~**2–6%** (their funnel example ≈ 5.6%).
- **Opt-in free trial** (no card) **→ paid:** ~**8–9%** (their funnel example ≈ 8.9%).
- **Opt-out free trial** (card required up front) **→ paid:** ~**30%**, more than **5×** a no-card
  trial. Only ~20% of trial products require a card; ~62% use a 14-day length.

**The important nuance.** Trials convert at a higher *rate* than freemium, but that edge **largely
washes out once you account for signup volume** — freemium pulls roughly **2× the signups** (≈90 vs 45
per 1,000 visitors). So model choice is about total paid customers, not the headline conversion rate.

**Mobile comparator (different market).** RevenueCat's State of Subscription Apps 2024 (30K+ mobile
apps): average **trial-to-paid 37.3%**, but **download-to-paid just 1.7%** within 30 days. Mobile
subscription apps are a *different* market from B2B SaaS — use only as a loose comparator, not a SaaS
benchmark.

**How to use.** Anchor the client's own free-to-paid rate against the band for *their* model (a 3%
freemium rate is normal; a 3% opt-in-trial rate is weak), and weigh conversion against signup volume,
not in isolation. The benchmark is a prior, not a target.

**Caveats.** Survey n=200 (B2B); conversion measured within 6 months; opt-out's high rate comes with
more involuntary churn and goodwill risk. Pairs with [[mon-tactic-model-choice]].
