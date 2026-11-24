---
id: ref-principle-cycle-time-and-compounding
stage: referral
sub_stage: referral-measurement
business_model: plg-saas
tactic_family: referral-measurement
unit_type: principle
metric: [new_signups]
provenance: public
sources:
  - "David Skok, 'Lessons Learned — Viral Marketing' (forentrepreneurs.com, 2009, primary) — growth ∝ K^(t/ct); reducing viral cycle time compounds harder than raising K. The measurement corollary: instrument ct, not just K."
---
**Principle — measure viral cycle time, not just k-factor: because ct sits in the exponent, shortening the loop usually beats raising the coefficient.**

Teams instrument k and ignore **viral cycle time (ct)** — the elapsed time of one full loop (user gets value
→ sends invite → invitee signs up → invitee sends their own invite). But growth is proportional to
**K^(t/ct)**: ct is in the exponent, so cutting it compounds the loop faster than an equivalent effort to
lift K. A loop at k = 0.4 that completes in a day out-produces a stronger-looking k = 0.6 loop that takes a
month. The practical corollary for measurement and design: **find where days leak out of the loop** — the
gap between a user's value moment and the invite prompt, the gap between an invite and the invitee's
activation, delays in reward delivery that stall the next loop — and compress them.

**How to apply.** Break the loop into timed stages and measure each: time-to-first-invite after value,
invite-to-signup, signup-to-next-invite. Attack the longest gap first (often value-moment→invite, fixed by
contextual placement, and invitee onboarding speed). Report ct alongside k; a program improving k while ct
balloons may be getting slower, not faster. Model both before predicting growth.

**When it applies.** Diagnosing a sluggish loop, prioritising loop improvements, or modelling expected
growth from a program.

**Caution (honesty).** ct and k have **no spec id** — confirm definitions; ct is only meaningful once the
loop stages are instrumented, which many clients haven't done (say what's needed). The compounding is real
but bounded by decay and self-selection — a short cycle doesn't rescue a k that falls below replacement.
Pairs with [[ref-framework-viral-loop-k-factor]] (the K^(t/ct) math) and
[[ref-principle-contextual-share-surfaces]] (placement shortens the value-moment→invite gap).
