---
id: mon-tactic-dunning-recovery
stage: monetization
sub_stage: revenue-retention
business_model: plg-saas
tactic_family: revenue-retention
unit_type: tactic
metric: [weekly_revenue, paying_conversion]
provenance: public
sources:
  - "Churnkey / Stripe — failed-payment retry and dunning recovery data (Stripe Smart Retries ~51%; staged dunning emails)."
---
**Tactic — recover failed payments with smart retries plus a short, staged dunning sequence.**

Most involuntary churn ([[mon-benchmark-involuntary-churn]]) is recoverable with plumbing, not product
work. Two levers: **retry logic** (retry the card at smarter times — Stripe Smart Retries recover
~51%, tuned retries a few points more) and a **dunning sequence** (a short series of emails/SMS asking
the customer to update their card). Each dunning message adds a point or two of recovery; open rates
fall sharply after the first, so the first message matters most.

**How to apply.** Turn on intelligent retries, send a first dunning message promptly and clearly
(card failed, one-click update), then 2–4 well-spaced follow-ups — not an endless nag. Add a
failed-payment prompt in-app for active users. Keep the tone helpful ("your card didn't go through"),
not punitive. Measure recovered revenue; a full stack can recover ~70% of involuntary churn.

**When it applies.** Any subscription product with card-on-file billing and non-trivial failed-payment
churn.

**Caution (ethics).** Don't degrade or lock the account before a fair recovery window and clear notice,
and make updating or cancelling **easy** — using a failed payment to trap a user who wants to leave is a
dark pattern. Respect card-network and anti-spam rules on retries and messaging. Pairs with
[[mon-tactic-downgrade-winback]].
