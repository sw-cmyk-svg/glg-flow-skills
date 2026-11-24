---
id: ref-framework-viral-loop-k-factor
stage: referral
sub_stage: viral-loops
business_model: plg-saas
tactic_family: viral-loops
unit_type: framework
metric: [new_signups]
provenance: public
sources:
  - "David Skok (Matrix Partners), 'Lessons Learned — Viral Marketing' (forentrepreneurs.com, 2009) — read at primary: K = invitations × conversion rate; growth ∝ K^(t/ct); K>1 for viral growth; hybrid/amplifier model."
---
**Framework — a viral loop has two numbers, and the less obvious one (cycle time) is the stronger lever.**

A referral/viral loop is described by two quantities. The **viral coefficient K** = the number of
invitations each user sends × the acceptance (conversion) rate of those invitations — how many new users
one user produces. The **viral cycle time (ct)** = how long one loop takes (see the product → send an
invite → the invitee signs up and sends their own). Growth over time *t* is proportional to **K^(t/ct)**:
because ct sits in the exponent, **halving the cycle time compounds harder than raising K**. Skok's
illustration: a loop with a 2-day cycle reaching ~20,000 users in 20 days reaches *millions* at a 1-day
cycle. **K > 1** is the threshold for self-sustaining growth (each user more than replaces themselves);
below 1 the loop decays to zero on its own.

**How to apply.** Instrument both numbers, not just K. To raise K, lift either invites-sent (more/better
share prompts, at the right moment) or acceptance (clearer invite, lower friction for the invitee). To cut
ct, shorten the gap between a user's value moment and their invite, and between an invite and the
invitee's own first loop — often the faster win. Model the loop before building it: a realistic K of 0.3
with a 1-day cycle can out-produce a K of 0.5 with a 30-day cycle. Virality is **built into the product**
(designers + engineers), not a campaign the marketing team runs.

**When it applies.** Designing or diagnosing any referral/viral loop; deciding whether to invest in the
loop at all; setting what to measure before launch.

**Caution (honesty).** k-factor and cycle time have **no canonical spec id** in `spec/metric-spec.yaml` —
pull the client's *exact* k-factor definition before reasoning over it (it is defined a dozen ways). K>1
is **rare and usually transient** — see [[ref-principle-most-loops-decay-k-below-1]]; most products use the
loop as an amplifier on other channels, not an engine. Pairs with [[ref-framework-virality-types]] (which
*kind* of loop) and the Acquisition seam: *measuring* this channel is Acquisition's
([[acq-principle-channel-saturation]]), *engineering* the loop is Referral's.
