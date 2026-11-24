---
id: act-benchmark-product-tour-engagement
stage: activation
sub_stage: onboarding
business_model: plg-saas
tactic_family: guidance
unit_type: benchmark
metric: [activation_rate, time_to_activation]
provenance: public
sources:
  - "Chameleon — User Onboarding Benchmark Report 2025 (550M+ interactions) + Product Tour Benchmarks highlights (15M interactions). https://www.chameleon.io/benchmark-report ; https://www.chameleon.io/blog/product-tour-benchmarks-highlights"
---
**Benchmark — how product tours / checklists actually perform (Chameleon platform data).**

- **Tour completion ≈ 61%** on average (just under two-thirds finish a tour they start).
- **Progress indicators** raise completion **~12%** and cut dismissal **~20%**.
- **Self-triggered / self-serve tours** vastly outperform blanket auto-triggered ones:
  **+123%** completion (highlights); launcher-driven **67% vs 31%** (2025 report);
  self-triggered ≈ **2×** the engagement.
- **Keep it short:** tours **beyond 5 steps lose more than half** of users.
- **Checklists:** users complete **~5 items per session** when surfaced via a launcher.

**How to apply (Design/Validate).** Default to **short (<5 step), user-triggered** guidance with
a **visible progress indicator**; don't force a long auto-tour on first load. Use these as
priors, then measure the client's own funnel.

**When it applies.** Any in-product guidance (tours, checklists, tooltips) in the onboarding
step.

**Caution.** This is **Chameleon's own platform data**, so it reflects companies already using
onboarding tooling (selection bias) and defines completion in their terms — directional priors,
not a universal `activation_rate`. Several figures sit in charts, not text. Reinforces (second
source) [[act-benchmark-tour-completion-by-steps]] on the step-count effect.
