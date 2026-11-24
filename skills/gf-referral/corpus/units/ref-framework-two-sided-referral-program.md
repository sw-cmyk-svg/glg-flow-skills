---
id: ref-framework-two-sided-referral-program
stage: referral
sub_stage: referral-program-design
business_model: plg-saas
tactic_family: referral-program-design
unit_type: framework
metric: [new_signups]
provenance: public
sources:
  - "Dropbox two-sided space-reward program (Drew Houston, 2010 Startup Lessons Learned talk; recounted in Sean Ellis & Morgan Brown, Hacking Growth, 2017) — CONCEPT; the '3900% in 15 months' / '~35% of signups' figures are historical (2008–2010) and reach us via varying secondary accounts."
  - "PayPal two-sided cash bonus, c.2000 ($20 step-down to $10 then $5) (Peter Thiel, Zero to One; practitioner teardowns) — CONCEPT; figures historical and secondary."
---
**Framework — the strongest referral program is two-sided (both the referrer and the invitee get something) and gives a reward the product itself makes cheap.**

A **one-sided** reward (only the referrer benefits) can read as the user selling their friends for personal
gain. A **two-sided** reward (give-and-get) gives the referrer a *generous reason to share* — "here's
something for you too" — which is both more effective and more honest. The second design choice is the
**reward itself**: the best programs reward in a currency the product can mint cheaply and that pulls the
invitee *into the product*. Dropbox's canonical case gave **storage space to both sides** — nearly free for
Dropbox to grant, and it deepened usage rather than just paying people out. PayPal, a money product, could
credibly give **cash** because money *was* the product. The mechanism, not the numbers, is the lesson:
two-sided + reward-matched-to-the-product + a low-friction share.

**How to apply.** Default to a two-sided structure. Choose a reward the product can grant at low marginal
cost and that increases engagement (extra seats, usage credits, feature access, storage) over raw cash
where possible — cash attracts reward-seekers who don't stick (see the reward-type unit). Keep the ask
simple and put it where the value is felt. Size the reward against the *qualified* CAC you'd otherwise pay,
not against revenue.

**When it applies.** Designing a referral program from scratch, or fixing a one-sided program that feels
transactional or attracts poor-fit signups.

**Caution (honesty).** The Dropbox/PayPal figures are **historical (2000, 2008–2010), secondary-sourced,
and vary across accounts** — use them to illustrate the *mechanism*, never quote them to a client as a
target (the recency rule). Reward design is persuasion-adjacent: avoid incentives so large they drive fraud
or mercenary invites (see [[ref-principle-reward-timing-value-moment]] and the fraud-controls unit in wave
2). `new_signups` is shared with Acquisition (referred slice). Pairs with
[[ref-principle-reward-type-matches-product]].
