---
id: ref-principle-cac-via-referral
stage: referral
sub_stage: incentive-economics
business_model: plg-saas
tactic_family: incentive-economics
unit_type: principle
metric: [new_signups]
provenance: public
sources:
  - "Established growth-economics practice — referral CAC = the fully-loaded reward cost (both sides) + program/engineering cost per qualified referred user; compare to paid CAC, but account for self-selection and cannibalisation. The LTV side is Monetization's."
---
**Principle — referral isn't free: its CAC is the loaded reward cost per qualified referred user — compare that to paid, honestly.**

"Referral has no CAC" is wrong. The cost per referred user is the **fully-loaded reward** (both sides of a
two-sided reward) plus the program and engineering cost, divided by the **qualified** referred users it
produced (those who activated/paid — not raw signups). That number is the thing to compare against paid-
channel CAC. Referral CAC is often lower and the users often better (see referred-user value), which is why
it's attractive — but two honesty adjustments matter: **self-selection** (some referred users would have
joined anyway, so part of the "referral" volume isn't incremental — only a holdout tells you the true
incremental CAC), and **cannibalisation** (rewarding referrals you'd have gotten free as word-of-mouth).
The reward **design/magnitude** is Referral's lever; what the business can *afford* (LTV, payback) is
Monetization's call.

**How to apply.** Compute referral CAC on qualified referred users with the full two-sided reward loaded in,
and set it beside paid CAC and payback. Size the reward against that qualified CAC, not against revenue or a
competitor's offer. For the "is it incremental / can we afford it" questions, run a holdout (measurement
units) and route the LTV/affordability side to Monetization.

**When it applies.** Deciding reward magnitude, comparing referral to paid channels, or justifying program
spend.

**Caution (honesty).** CAC, LTV, and payback have **no canonical spec id** — flag the client's definitions.
A referral CAC that ignores self-selection **understates** the true cost per *incremental* user. This unit
owns the reward-as-cost lever; LTV and affordability are Monetization's (route there). Pairs with
[[ref-principle-referred-users-more-valuable]] and mirrors [[acq-benchmark-cac-payback]] (paid-side
efficiency).
