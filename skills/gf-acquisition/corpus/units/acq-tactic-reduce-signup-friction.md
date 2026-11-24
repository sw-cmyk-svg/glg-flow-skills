---
id: acq-tactic-reduce-signup-friction
stage: acquisition
sub_stage: acquisition-conversion
business_model: plg-saas
tactic_family: acquisition-conversion
unit_type: tactic
metric: [signup_rate, new_signups]
provenance: public
sources:
  - "Established signup / form-conversion CRO practice (reduce fields, single clear CTA, defer non-essential data, show value before asking)."
---
**Tactic — remove friction between landing and account: ask for less, promise value, one clear action.**

The visitor→signup step leaks when the form asks for too much too soon, offers more than one competing
action, or demands commitment before the visitor sees why it's worth it. The levers: cut the signup
form to the fields you truly need at this step (defer the rest to onboarding), make the primary
call-to-action single and unambiguous, remove distractions that compete with it, and let the visitor
glimpse the value before the ask (a demo, a preview, or "start free") where the product allows. Each
removed step of effort or doubt recovers signups you already paid to attract.

**How to apply.** Audit the path from landing to created account: count the fields, the clicks, and the
decisions. Drop every field that isn't needed to create the account, collapse multi-step forms where
you can, and make the one next action obvious. Offer social/SSO or "start free" when it fits the model.
Measure the change on `signup_rate` — but see the seam caution.

**When it applies.** A surface with traffic and interest (good message match) but drop-off at the
signup form itself.

**Caution (honesty + seam).** There's an **Activation seam**: reducing *signup* friction can raise
`signup_rate` while *lowering* downstream activation if you let in users who never needed the product —
judge the change on signup **quality** (do they activate?), not signup count alone (see
[[acq-framework-channel-model-fit]] on cohort fit; route onboarding friction to the Activation
specialist). And "reduce friction" never means hiding costs, pre-ticking consent, or making cancellation
hard — those are dark patterns, not friction reduction. Pairs with [[acq-tactic-message-match]].
