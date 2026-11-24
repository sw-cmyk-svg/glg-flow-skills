---
id: ref-principle-referral-fraud-controls
stage: referral
sub_stage: incentive-economics
business_model: plg-saas
tactic_family: incentive-economics
unit_type: principle
metric: [new_signups]
provenance: public
sources:
  - "Established referral-program practice — any rewarded program is gamed (self-referral, fake accounts, reward farming); controls (reward on qualified action, caps, verification, clawback) are designed in, not bolted on. The reward trigger is the primary control."
---
**Principle — any reward will be gamed; design the fraud controls into the program, don't bolt them on after.**

A referral reward is a bounty, and bounties attract gaming: **self-referral** (inviting your own second
account), **fake accounts** created only to claim rewards, and **reward farming** at scale. The single
biggest control is the **reward trigger** — paying on a *qualified* downstream action (the referred user
activates or makes a first payment) rather than on signup makes most fraud uneconomic, because a fake
account would have to behave like a real paying user to earn anything. Layer on **caps** (per-user reward
limits), **verification** (unique payment method / device / email where proportionate and privacy-
respecting), **velocity checks** (a flag on improbable referral bursts), and a **clawback** window if a
referred user turns out fraudulent or refunds.

**How to apply.** Start from the qualified-action trigger (it does most of the work), then add caps and
velocity monitoring sized to the reward's value — heavier controls for cash, lighter for low-value in-
product rewards. Decide the clawback rule up front and put it in the program terms. Monitor referred-cohort
quality: a sudden drop in referred-user activation/retention is often fraud, not a mechanic problem.

**When it applies.** Designing a rewarded program (especially cash); investigating a program with high
invite volume but collapsing referred-cohort quality or runaway reward cost.

**Caution (ethics & privacy):** fraud controls must stay **proportionate and privacy-respecting** — device/
identity checks handle personal data (HR2 / data-protection); don't over-collect, and don't punish honest
users with hostile friction. Never design the *fraud itself* (fake-account schemes) — document only. Pairs
with [[ref-principle-reward-timing-value-moment]] (the trigger is the main control) and
[[ref-principle-reward-type-matches-product]] (in-product rewards are less fraud-prone than cash).
