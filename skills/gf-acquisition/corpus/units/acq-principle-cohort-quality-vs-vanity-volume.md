---
id: acq-principle-cohort-quality-vs-vanity-volume
stage: acquisition
sub_stage: attribution-efficiency
business_model: plg-saas
tactic_family: attribution-efficiency
unit_type: principle
metric: [new_signups, activation_rate]
provenance: public
sources:
  - "Established PLG practice — judge acquisition by downstream cohort quality (activation / retention / revenue), not raw signup volume; the Acquisition↔Activation seam (see copilot/specialists/acquisition/CHARTER.md)."
---
**Principle — judge a channel by the quality of the users it brings, not the count of signups.**

Signup volume is a **vanity metric** on its own. A channel that delivers many signups who never
activate is worse than one that delivers fewer who stick — it inflates `new_signups` while filling the
funnel with users who cost money to serve and churn. So acquisition quality is measured **downstream**:
what share of each channel's cohort reaches the activation event (`activation_rate`), then retains and
pays. This is the acquisition side of the "is it an activation problem" check — if one channel's
signups activate far below the others, that channel is bringing the wrong users (an acquisition
targeting problem), not proof the onboarding is broken.

**How to apply.** Rank channels by **activated / retained** signups, not raw signups. When a client
cheers a signup spike, ask what those cohorts did next; a cheap channel with a terrible activation rate
is usually more expensive than it looks. Feed this back into channel and targeting choices — chase the
channels that bring users who get to value, and fix or cut the ones that bring tourists.

**When it applies.** Evaluating channel performance, a signup-volume spike with flat revenue, or
deciding where to concentrate (pairs with Bullseye's "customer fit" test).

**Caution (honesty).** This needs **downstream data** (activation/retention by acquisition cohort),
which many clients don't track cleanly yet — say what's needed rather than guessing. Attribution of a
cohort to a channel carries the usual limits (see [[acq-principle-attribution-limits]]). The onboarding
fix itself is Activation's, not Acquisition's — route it. Pairs with [[acq-framework-channel-model-fit]]
(cohort fit) and [[acq-framework-bullseye-channel-concentration]] (test on customer fit, not just cost).
