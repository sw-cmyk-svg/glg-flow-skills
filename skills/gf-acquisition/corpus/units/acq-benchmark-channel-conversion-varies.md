---
id: acq-benchmark-channel-conversion-varies
stage: acquisition
sub_stage: attribution-efficiency
business_model: plg-saas
tactic_family: attribution-efficiency
unit_type: benchmark
metric: [signup_rate, new_signups]
provenance: public
sources:
  - "Unbounce Conversion Benchmark Report 2024, SaaS industry page — conversion rate by traffic channel (median), read directly from the public report page (unbounce.com/conversion-benchmark-report/saas-conversion-rate). Verified at primary."
---
**Benchmark prior — in SaaS, channels convert wildly differently: email ~17% down to display ~0.3%. Judge a channel by its own conversion, not blended volume.**

Median landing-page conversion by traffic channel, SaaS (Unbounce 2024):

| Channel | Median CVR | | Channel | Median CVR |
|---|---|---|---|---|
| Email | **16.9%** | | Paid social (overall) | 2.9% |
| Instagram (paid) | 9.2% | | Facebook (paid) | 3.5% |
| Google paid search | 5.1% | | Bing paid search | 1.9% |
| Paid search (overall) | 4.1% | | Display | **0.3%** |

Email converts **~50× better than display** and ~4× better than paid search. The lesson for
acquisition: a blended `signup_rate` hides enormous channel variance, so a "low" overall conversion is
often a **traffic-mix** story (too much low-intent display/awareness traffic) rather than a broken page.
Warm, high-intent channels (email, your own audience) convert far above cold paid reach — which is also
why owned channels and message match matter.

**How to apply.** Before "fixing the page," split `signup_rate` by channel and compare each to its own
benchmark band. A channel converting near these medians is normal; one far below suggests message
mismatch or wrong-fit traffic *for that channel*. Don't compare a display campaign to an email number.

**When it applies.** Diagnosing conversion, allocating budget across channels, or explaining why blended
conversion moved (usually a mix shift, not a page change).

**Caution (honesty).** Conversion rate ≠ **value per conversion** — display's 0.3% and email's 16.9%
aren't directly comparable in ROI (channels sit at different funnel stages and reach different
intent). These are SaaS medians from Unbounce's dataset (campaign/paid landing pages, Unbounce
customers); other archetypes differ. Pairs with [[acq-principle-attribution-limits]] and
[[acq-benchmark-landing-page-conversion]] (the overall industry figure).
