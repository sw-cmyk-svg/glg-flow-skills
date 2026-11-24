---
id: act-principle-social-proof
stage: activation
sub_stage: signup
business_model: plg-saas
tactic_family: social-proof
unit_type: principle
metric: [signup_rate, activation_rate]
provenance: public
sources:
  - "UserGuiding — How Top AI Tools Onboard New Users (2026). https://userguiding.com/blog/how-top-ai-tools-onboard-new-users"
  - "Secondary stats cited therein: UGC ≈ +29% website conversion; 72% trust reviews/testimonials over branded content — confirm at original source before quoting."
---
**Principle — show that real people get value here, to lower the risk of trying.**

Seeing others succeed reduces a new user's perceived risk. In the UserGuiding teardown,
**Lovable** surfaces user-made projects *before* signup so a visitor sees what's possible, and
**6 of 10** AI tools feature user-generated content, reviews, or testimonials on their sites.
Cited secondary stats: UGC can lift website conversion **~29%**, and **72%** of consumers
trust reviews/testimonials over branded content.

**How to apply.** Put concrete, specific proof where hesitation happens — real example
projects, named testimonials, "most teams start with X" — at the signup decision and at the
first empty state. Specific beats generic ("Acme's team built this in 10 min" > "trusted by
thousands").

**When it applies.** Strongest at signup and empty-first-run, where risk/uncertainty is
highest. Note the teardown found social proof mostly **pre-signup on the website**, not inside
the product flow — the in-flow empty state is an underused slot.

**Caution.** The cited conversion figures are **second-hand** (UserGuiding quoting other
studies) and tied to *website* conversion, not the spec's `activation_rate` — confirm at
source before using as a benchmark.

**Caution (ethics).** Social proof must be **true**: real counts, real testimonials, real
usage. Fabricated user counts, fake "N people viewing now" urgency, or invented reviews are
dark patterns — document them only as things to avoid, never prescribe them. For bank/wallet and
other financial archetypes, take care not to use social proof to normalize risky financial
behaviour, and advise the client to confirm compliance with financial-promotion rules. Pairs with
[[act-tactic-value-before-signup]].
