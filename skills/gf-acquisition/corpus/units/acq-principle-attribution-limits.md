---
id: acq-principle-attribution-limits
stage: acquisition
sub_stage: attribution-efficiency
business_model: plg-saas
tactic_family: attribution-efficiency
unit_type: principle
metric: [new_signups]
provenance: public
sources:
  - "Established marketing-measurement practice — attribution models (last-click / multi-touch) are directional, not causal; incrementality (holdout / geo tests) is the stronger test. Privacy changes (Apple ATT 2021, third-party-cookie deprecation) degraded deterministic tracking."
---
**Principle — attribution is directional, not truth: prefer incrementality (what spend actually caused) over any attribution model.**

Every attribution model is a **story about credit**, not a measurement of cause. **Last-click**
over-credits the final touch (usually branded search or the channel someone was already going to use)
and under-credits awareness channels that created the demand. **Multi-touch** spreads credit by a rule
you chose, which is still an assumption. None of them answer the real question — *did this spend produce
signups that wouldn't have happened anyway?* That question is answered by **incrementality**: a holdout
or geo test where you turn a channel down/off for a random slice and measure the difference. On top of
this, **privacy changes** (Apple's App Tracking Transparency, the decline of third-party cookies) have
made deterministic tracking leakier, so precise per-user attribution is less trustworthy than it looks.

**How to apply.** Treat attribution dashboards as a directional guide, not a verdict — especially
before cutting an "underperforming" awareness channel that last-click can't see. When a channel
decision carries real budget, propose an **incrementality test** (holdout or geo) rather than trusting
the model. State plainly which channels the client's setup is likely under- or over-crediting.

**When it applies.** Any "which channel is working / where should we spend" question, or a plan to cut a
channel based on attributed CAC.

**Caution (honesty).** Incrementality is the stronger test but it isn't free — it needs enough volume
and the discipline to withhold exposure. Don't present attributed CAC as proven causation. CAC/channel
metrics have no canonical spec id — flag definitions. Pairs with
[[acq-benchmark-channel-conversion-varies]] and [[acq-principle-cohort-quality-vs-vanity-volume]].
