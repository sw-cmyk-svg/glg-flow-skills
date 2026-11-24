---
id: act-framework-onboarding-shape
stage: activation
sub_stage: signup
business_model: plg-saas
tactic_family: guidance
unit_type: framework
metric: [signup_rate, activation_rate, time_to_activation]
provenance: public
sources:
  - "AI UX Playground — AI onboarding compared: Notion AI, Lovable, Manus (Jul 2026). https://aiuxplayground.com/teardowns/compare/ai-onboarding-first-value"
---
**Framework — choose the onboarding *shape* to the product, not by fashion.**

A three-way teardown (Notion AI / Lovable / Manus) maps onboarding shape to product type:

- **Embedded (Notion AI).** No wizard; AI activates in-document at the cursor. **Choose when
  the feature extends a tool the user already has open** — surface categorized one-click prompt
  starters at the point of work. See [[act-design-embedded-prompt-starters]].
- **Short wizard (Lovable).** A 4-step full-screen wizard (theme, name, role, company size),
  one question per screen. **Choose when you genuinely need segmentation data to personalize a
  blank builder before the first prompt** — and keep it short. See
  [[act-tactic-segment-at-signup]].
- **Role cards + taught meter (Manus).** A 9-card outcome-framed role grid, then Pro pricing
  with a 7-day trial mid-funnel. **Choose when you sell autonomous, metered work** — frame the
  job, and teach the meter before users hit a limit.

**How to apply (Design step).** Pick the shape from the product's relationship to the user's
existing workflow and business model; don't default to a wizard. Stated cross-pattern rules:
**keep steps skippable** and **show real capability, not slides**.

**When it applies.** Any first-run design decision in the propose pipeline's Design step.

**Caution.** This is **design guidance, not benchmarks** — the page reports no activation
figures (step counts only: Notion 0, Lovable 4, Manus 9). Mid-funnel pricing (Manus) must stay
skippable; for bank/wallet and other financial archetypes, advise compliance with financial-promotion rules rather than pressure.
Pairs with [[act-principle-goal-dilution]] (don't let the shape multiply goals).
