---
id: mon-tactic-feature-gating
stage: monetization
sub_stage: packaging-tiering
business_model: plg-saas
tactic_family: packaging-tiering
unit_type: tactic
metric: [paying_conversion, arpu]
provenance: public
sources:
  - "General PLG packaging practice (Reforge / OpenView lineage); value-metric alignment from mon-principle-value-metric."
---
**Tactic — gate the upgrade on the value metric, not on random features.**

What you put behind each paywall decides whether upgrading feels fair. The durable approach gates on
the **value metric and the capabilities that scale with value** — more usage, more seats, more of the
thing power users need — so a customer upgrades exactly when they're getting more value. Gating on
arbitrary or essential-but-cheap features (export, basic security, the core job) feels like a hostage
situation and breeds resentment and churn.

**How to apply.** Sort features into: **free** (drives adoption and the aha), **paid** (scales with
value or serves power users / teams), and **never-gate** (basic security, data export, core safety —
gating these is hostile and sometimes non-compliant). Put the natural upgrade trigger where a growing
customer will hit it (a usage limit, a seat limit, a team feature), and make the value of crossing it
obvious at that moment.

**When it applies.** Designing tiers; deciding the free/paid line; fixing a plan where upgrades feel
punitive.

**Caution (ethics).** Don't gate things users reasonably consider basic rights — **data export,
account security, the ability to leave** — behind a paywall; that's a lock-in dark pattern. Keep the
free tier genuinely useful, not crippled bait. Pairs with [[mon-principle-good-better-best]] and
[[mon-tactic-paywall-placement-timing]].
