---
id: acq-principle-channel-saturation
stage: acquisition
sub_stage: channel-strategy
business_model: plg-saas
tactic_family: channel-strategy
unit_type: principle
metric: [signup_rate, new_signups]
provenance: public
sources:
  - "Andrew Chen, 'The Law of Shitty Clickthroughs' (andrewchen.com, 2009; with later follow-up)."
---
**Principle — every channel decays: a channel's response rate falls over time as it saturates.**

Chen's "law of shitty clickthroughs": the response rate of a marketing channel declines every year
after it appears, trending toward zero. The anchor example — the **first banner ad, on HotWired in
1994, ran at a ~78% clickthrough rate**; banner CTRs have since fallen asymptotically toward nothing.
Three forces drive it: **novelty fades** (people stop responding to a format they've seen), **first
movers don't stay ahead** (competitors copy in, auction prices rise), and **scale brings worse-fit
customers** (the best prospects convert first; later volume is less qualified). The practical reading:
a channel's early ROI is its *best* ROI, not its steady state.

**How to apply.** Don't model a channel's launch performance as permanent — expect the cost per signup
to rise and conversion to fall as you scale it, and bank the early advantage while it lasts. Being
early to a channel (a new ad platform, a new content surface, a new partnership type) is itself an
edge. Keep discovering the next channel before the current one saturates, rather than squeezing a
decaying one harder.

**When it applies.** Forecasting a channel's future cost, explaining a channel that "stopped working,"
or deciding whether to double down or diversify. Pairs with
[[acq-framework-bullseye-channel-concentration]] (concentrate, but keep the next candidate ready).

**Caution (honesty).** Decay is directional, not a precise curve — the rate varies by channel and by
how fast competitors pile in; don't quote a decline number you haven't measured. CAC / cost-per-signup
has no canonical spec id — flag the client's definition. A channel can also be *revived* (new creative,
new audience), so saturation is a reason to iterate or rotate, not always to abandon.
