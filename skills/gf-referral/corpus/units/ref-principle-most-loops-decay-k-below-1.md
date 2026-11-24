---
id: ref-principle-most-loops-decay-k-below-1
stage: referral
sub_stage: viral-loops
business_model: plg-saas
tactic_family: viral-loops
unit_type: principle
metric: [new_signups]
provenance: public
sources:
  - "David Skok, 'Lessons Learned — Viral Marketing' (forentrepreneurs.com, 2009, primary) — 'only a very small number of companies actually achieve true viral growth'; the hybrid model covers the shortfall with other channels."
  - "Andrew Chen, 'The Law of Shitty Clickthroughs' — invite/share response rates decay as a channel saturates a user's network (concept applied to invites)."
---
**Principle — assume k < 1: a referral loop is almost always an amplifier on other channels, not a growth engine on its own.**

Self-sustaining virality (k > 1 held over time) is rare and usually temporary. The honest planning
assumption is **k < 1** — the loop adds a multiplier to acquisition you already have rather than replacing
it. With k = 0.5, every 100 users acquired elsewhere bring ~100 more across the full decay of the loop (a
~2× amplification), which is valuable and worth engineering — but it is not a flywheel that runs without
fuel. Loops also **decay**: invite acceptance falls as the loop saturates a user's network (the same
"shitty clickthroughs" effect that hits paid channels), and early-adopter enthusiasm doesn't generalize to
the mainstream. A k that looks like 0.8 in month one can settle far lower.

**How to apply.** Model the loop as an amplifier: estimate the realistic steady-state k, apply it as a
multiplier on paid/organic/content acquisition, and fund those channels accordingly — don't bet the plan
on the loop carrying growth. Re-measure k over time and by cohort; treat a high early k as provisional
until it holds past the early adopters. If the honest number is very low, the loop may not be worth the
build — say so.

**When it applies.** Growth modelling, go/no-go on a referral build, or a reality check when a founder
expects a program to "make us go viral."

**Caution (honesty).** A measured k is **confounded by self-selection** — your most engaged users adopt the
loop first and would have referred anyway, inflating early readings (see the measurement units in wave 3).
k has **no spec id** — confirm the client's definition. Pairs with [[ref-framework-viral-loop-k-factor]]
(the math) and mirrors [[acq-principle-channel-saturation]] (channels, including invite channels, decay).
