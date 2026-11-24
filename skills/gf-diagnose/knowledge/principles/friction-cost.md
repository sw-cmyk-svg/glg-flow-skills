---
id: friction-cost
collection: principles
title: Friction cost
grade: A
sources:
  - ref: "Thaler & Sunstein (2021), 'Nudge: The Final Edition'"
    year: 2021
  - ref: "Sunstein (2020), 'Sludge Audits' / sludge literature, Behavioural Public Policy"
    year: 2020
status: active
---

## Claim
Small increases in the effort required to complete an action cause
disproportionate drop-off relative to the effort itself — an extra form
field, an extra click, an extra wait costs far more conversion than its
objective difficulty implies. This is consistent across decades of field
A/B testing and formalized in the "sludge" literature as the inverse of
a nudge: friction deliberately or accidentally added to a desired path.

## Applicability — works when
- The action is one the user already intends to complete (signup,
  checkout, upgrade) — friction here is pure leakage, not a filter
- The friction is removable without changing what the user is agreeing
  to or receiving
- The funnel step is high-volume, so even a small per-step lift compounds

## Backfires when
- Removing all friction from irreversible or high-regret actions
  (account deletion, one-click large purchases, destructive changes)
  raises refunds, regret, chargebacks, and support load — some friction
  is protective, not wasteful
- Friction is removed from a step that was doing legitimate qualification
  (e.g., a form field that filtered out bad-fit leads); conversion goes
  up but downstream quality goes down
- The "friction" removed was actually trust-building (e.g., skipping a
  confirmation step that reassured cautious buyers)

## Growth applications
- Cut form fields on signup to the minimum required for account creation
  (signup_rate, new_signups)
- Remove confirmation modals from reversible, low-stakes in-product
  actions (activation_rate)
- Reduce steps between "trial ends" and "payment method entered" for
  users who already indicated intent to convert (trial_to_paid)

## Practice stance
We audit friction step by step and ask what each step is buying us
before cutting it — friction removal is our highest-confidence lever
(grade A) but only on paths where the user's intent is already formed.
We refuse to strip friction from irreversible actions purely to chase a
conversion metric; we measure downstream regret and support volume
alongside the funnel metric whenever we touch a destructive or
high-commitment flow.
