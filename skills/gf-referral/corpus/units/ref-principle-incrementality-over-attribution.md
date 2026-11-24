---
id: ref-principle-incrementality-over-attribution
stage: referral
sub_stage: referral-measurement
business_model: plg-saas
tactic_family: referral-measurement
unit_type: principle
metric: [new_signups]
provenance: public
sources:
  - "Established causal-measurement practice — a holdout / randomised experiment measures the INCREMENTAL effect of a referral program; an attribution dashboard (who had a referral code) is directional and self-selection-biased. Mirrors the Acquisition attribution-limits unit."
---
**Principle — to know what a referral program is really worth, run a holdout; the referral-attribution dashboard tells you who used a code, not what the program caused.**

A referral dashboard counts signups that carried a referral code or came through an invite link. That is
**attribution**, not **incrementality** — it includes all the self-selected users who'd have joined anyway,
so it overstates the program's true effect and can't price the reward correctly. The honest test is an
**experiment**: withhold the program (or a reward tier, or a prompt) from a randomised **holdout** — a slice
of users, or whole geos/segments where a user-level holdout isn't clean — and compare incremental new
signups and their downstream value against the treated group. The difference is what the program actually
caused, and dividing the reward cost by *incremental* qualified referred users gives the real referral CAC.

**How to apply.** For any material referral-spend decision, design a holdout before scaling: randomise who
sees the program/reward, run long enough to clear the viral cycle time and seasonality, and read incremental
signups + referred-cohort quality, not raw attributed volume. Where a user-level holdout would leak (shared
links), use a geo or cohort holdout. Route the experiment design to Validate/`propose-experiments`; this
unit sets *why* incrementality is the right bar.

**When it applies.** Deciding whether to scale, cut, or re-size a referral program; setting the true
referral CAC; rebutting an inflated attributed-referrals claim.

**Caution (honesty).** A holdout costs some referral volume during the test — worth it for a real spend
decision, overkill for a tiny program (say which). Even a holdout has limits (novelty effects, contamination
via shared links) — state them. Mirrors [[acq-principle-attribution-limits]] (incrementality > models on
the acquisition side). Pairs with [[ref-principle-self-selection-confound]] (the problem this solves) and
[[ref-principle-cac-via-referral]] (incremental CAC).
