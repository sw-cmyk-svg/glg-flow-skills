---
id: ref-principle-self-selection-confound
stage: referral
sub_stage: referral-measurement
business_model: plg-saas
tactic_family: referral-measurement
unit_type: principle
metric: [new_signups]
provenance: public
sources:
  - "Established causal-inference practice applied to referral — referred signups are confounded by self-selection: your most engaged users adopt the loop first and would have referred/recommended anyway, so attributed referral volume overstates incremental new users. The core measurement honesty of the stage."
---
**Principle — referral numbers flatter themselves: your best users adopt the loop first and would have brought friends anyway, so attributed referrals overstate the incremental users.**

The central measurement trap in referral is **self-selection**. The users who join a referral program and
send invites are disproportionately your *most engaged, happiest* users — exactly the people whose friends
would have heard about the product through ordinary word-of-mouth regardless. So a chunk of the signups the
program *attributes to itself* are not **incremental**; they'd have happened anyway, now wearing a referral
code and sometimes collecting a reward you didn't need to pay. The same applies to k-factor: an early k
measured on enthusiastic early adopters reads high and then falls as the loop reaches ordinary users. Any
pre/post "we launched referral and signups rose" is confounded by this plus seasonality and the other
channels running at the same time — it is **not proof** the program caused the lift.

**How to apply.** Treat attributed referral volume as an **upper bound** on the program's real contribution,
not its true value. Discount for the share that would have converted anyway, and don't reward-pay for
cannibalised organic word-of-mouth where avoidable. For any real "is it working / what's the incremental
CAC" decision, use a holdout rather than the attribution dashboard (next unit). Re-measure k over time and
by cohort, expecting the early number to overstate.

**When it applies.** Reading referral performance, defending or cutting program spend, validating a claimed
k-factor or a post-launch lift.

**Caution (honesty).** Mandatory causal-vs-correlational discipline for this stage: a referral lift is
**correlational, self-selection-confounded**; never present it as proven. k has **no spec id** — confirm the
definition. Pairs with [[ref-principle-incrementality-over-attribution]] (the fix) and
[[ref-principle-most-loops-decay-k-below-1]] (early k overstates).
