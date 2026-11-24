# Monetization corpus — index

**Version:** 0.0.3 (waves 1–3 — 2026-11-18) · business_model: `plg-saas`
**Status:** drafting (I draft, founder vets). **18 units — all six families ≥3 (robust bar met).**
Same curation rules: authored distilled note + citation, I-draft-you-vet, verification-as-drafting,
persuasion-ethics principle.

**Curation principle — persuasion & ethics (inherited).** Persuasion / behavioural pricing tactics are
allowed, but every persuasion-adjacent unit MUST carry an explicit `Caution (ethics):` line.
Monetization's ethics edge is **pricing fairness and transparency**: deceptive pricing, hidden fees,
drip pricing, hard-to-cancel subscriptions, and manufactured urgency are dark patterns — documented as
anti-patterns, never prescribed — and several are unlawful in many jurisdictions. Regulated archetypes
(bank/wallet, betting) get a compliance caution, not a ban.

| id | unit_type | tactic_family | sub_stage | verified |
|---|---|---|---|---|
| [mon-principle-charm-pricing](units/mon-principle-charm-pricing.md) | principle | price-setting | price-setting | ⚠ small effect; ✅ book (Shlain 2023) |
| [mon-principle-price-relativity-anchoring](units/mon-principle-price-relativity-anchoring.md) | principle | price-setting | price-setting | ⚠ ethics (decoy); ✅ book (S&F 2022) |
| [mon-principle-temporal-reframing](units/mon-principle-temporal-reframing.md) | principle | price-setting | price-setting | ⚠ honesty (show total); ✅ book (Gourville 1998) |
| [mon-principle-present-bias-deferral](units/mon-principle-present-bias-deferral.md) | principle | free-to-paid | free-to-paid | ⚠⚠ ethics (overspend/lending); ✅ book (Bain, Delaney&Lades 2017) |
| [mon-principle-value-metric](units/mon-principle-value-metric.md) | principle | pricing-model | pricing-model | ✅ Poyar/OpenView (1,800-co assessment) |
| [mon-principle-usage-vs-seat](units/mon-principle-usage-vs-seat.md) | principle | pricing-model | pricing-model | ✅ Poyar/OpenView; ⚠ bill-shock honesty |
| [mon-tactic-model-choice](units/mon-tactic-model-choice.md) | tactic | pricing-model | pricing-model | ✅ Reforge/Poyar + ChartMogul 2026 |
| [mon-principle-good-better-best](units/mon-principle-good-better-best.md) | principle | packaging-tiering | packaging-tiering | ✅ PLG practice + price relativity |
| [mon-tactic-feature-gating](units/mon-tactic-feature-gating.md) | tactic | packaging-tiering | packaging-tiering | ⚠ ethics (never-gate basics); ✅ PLG practice |
| [mon-principle-decoy-tier](units/mon-principle-decoy-tier.md) | principle | packaging-tiering | packaging-tiering | ⚠⚠ ethics (decoy line); ✅ Huber/Payne/Puto 1982 |
| [mon-tactic-paywall-placement-timing](units/mon-tactic-paywall-placement-timing.md) | tactic | free-to-paid | free-to-paid | ⚠ Activation seam; ✅ PLG practice |
| [mon-benchmark-free-to-paid-conversion](units/mon-benchmark-free-to-paid-conversion.md) | benchmark | free-to-paid | free-to-paid | ✅ ChartMogul/ProductLed/Poyar 2026 (200 B2B); RevenueCat mobile comparator |
| [mon-principle-expansion-nrr](units/mon-principle-expansion-nrr.md) | principle | expansion | expansion | ✅ Poyar/OpenView; ⚠ NRR masks churn |
| [mon-benchmark-nrr-saas](units/mon-benchmark-nrr-saas.md) | benchmark | expansion | expansion | ✅ Poyar/Growth Unhinged 2024 (4,000+ co) |
| [mon-tactic-upsell-at-value-moments](units/mon-tactic-upsell-at-value-moments.md) | tactic | expansion | expansion | ✅ PLG practice; ⚠ ethics (real limits) |
| [mon-benchmark-involuntary-churn](units/mon-benchmark-involuntary-churn.md) | benchmark | revenue-retention | revenue-retention | ✅ Stripe via Churnkey (~22%) |
| [mon-tactic-dunning-recovery](units/mon-tactic-dunning-recovery.md) | tactic | revenue-retention | revenue-retention | ✅ Churnkey/Stripe retries; ⚠ easy-cancel |
| [mon-tactic-downgrade-winback](units/mon-tactic-downgrade-winback.md) | tactic | revenue-retention | revenue-retention | ⚠⚠ ethics (cancel dark patterns); ✅ practice |

**Tactic-family coverage (robust — all ≥3):** pricing-model ✓✓✓, packaging-tiering ✓✓✓,
price-setting ✓✓✓, free-to-paid ✓✓✓, expansion ✓✓✓, revenue-retention ✓✓✓.
**Benchmark priors anchored (all verified first-party):** NRR ~110% median (Poyar/Growth Unhinged
2024); involuntary churn ~22% of SaaS churn (Stripe via Churnkey); free-to-paid conversion — median
~8%, freemium ~2–6%, opt-in trial ~8–9%, opt-out trial ~30% (ChartMogul × ProductLed × Poyar 2026, 200
B2B products), with the signup-volume nuance that freemium's lower rate is offset by ~2× signups; mobile
comparator from RevenueCat 2024. **Verification notes (per founder's standing ask):** old OpenView
blog-post URLs are dead (redirect to homepage) — value-metric/usage figures sourced via Reforge's
summary of Poyar + Growth Unhinged + OpenView's State of Usage-Based Pricing instead. The ProfitWell
freemium primary is retired (now a Paddle series); free-to-paid is grounded in ChartMogul/Poyar 2026
instead. Nothing fabricated to fill a gap.
**Persuasion-adjacent (mandatory `Caution (ethics):`):** charm-pricing, price-relativity, temporal-
reframing, present-bias, decoy-tier (heaviest), feature-gating, downgrade-winback (cancel patterns).
Monetization's dark-pattern surface (drip pricing, hidden fees, hard-to-cancel, surprise renewals) is
documented as anti-patterns only, several unlawful in many jurisdictions.

**Six tactic families (target ≥3 each):**
1. **pricing-model** — subscription / usage-based / seat / hybrid; freemium vs trial vs reverse trial;
   the **value metric** (charge on the thing that scales with customer value).
2. **packaging-tiering** — good-better-best, feature gating, what sits in each tier.
3. **price-setting** — price points, willingness-to-pay / price sensitivity, anchoring, charm pricing.
4. **free-to-paid** — freemium / trial conversion, paywall placement & timing, free vs paid line.
5. **expansion** — upsell, cross-sell, usage-based growth, seat expansion, the path to NRR > 100%.
6. **revenue-retention** — subscription / revenue churn, downgrade prevention, involuntary churn
   (dunning), win-back of paying customers.

**Drafting order (plan):**
1. **Benchmarks (anchor first):** freemium→paid, trial→paid, NRR, involuntary-churn share
   (ProfitWell / OpenView). → the Analyze/benchmark priors for the revenue band.
2. **pricing-model (the spine):** the value metric (charge on what scales with value); freemium vs
   free trial vs reverse trial; usage-based vs seat-based.
3. **price-setting:** willingness-to-pay (Van Westendorp), charm pricing (book ch.5), price relativity
   / anchoring (book ch.8) — each with the ethics caution.
4. **packaging-tiering:** good-better-best, decoy/anchor tier (ethics), feature gating.
5. **free-to-paid:** paywall placement & timing, value-metric-aligned gating, present-bias / annual
   framing (book ch.13).
6. **expansion** + **revenue-retention:** upsell/cross-sell, usage expansion & NRR; dunning /
   involuntary churn, downgrade prevention, paying-user win-back.

**Reuses:** the book epub (ch.5 charm pricing, ch.8 price relativity, ch.13 present bias), Balfour
strategy spine, and the Activation/Retention PDFs. New mining: ProfitWell/Paddle, OpenView/Kyle Poyar,
Reforge, Lenny's. See `SOURCES.md`.
