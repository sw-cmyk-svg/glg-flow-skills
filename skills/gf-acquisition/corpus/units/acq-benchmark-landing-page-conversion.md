---
id: acq-benchmark-landing-page-conversion
stage: acquisition
sub_stage: acquisition-conversion
business_model: plg-saas
tactic_family: acquisition-conversion
unit_type: benchmark
metric: [signup_rate, unique_visitors]
provenance: public
sources:
  - "Unbounce Conversion Benchmark Report 2024 (~57M conversions, ~41,000 landing pages, +464M visitors, past year). Overall + all nine per-industry medians and SaaS channel splits read directly from the report's public pages (unbounce.com/conversion-benchmark-report and its per-industry pages) — verified at primary, no gate."
---
**Benchmark prior — landing-page conversion is 6.6% median across industries; SaaS is the lowest at 3.8%.**

Median landing-page conversion by industry (Unbounce 2024, all verified on public pages):

| Industry | Median | | Industry | Median |
|---|---|---|---|---|
| SaaS | **3.8%** (lowest) | | Healthcare & wellness | 8.2% |
| Ecommerce | 4.2% | | Finance & insurance | 8.3% |
| Travel & hospitality | 4.8% | | Education | 8.4% |
| Professional services | 6.1% | | Entertainment | **12.3%** (highest) |
| Legal | 6.3% | | **All industries** | **6.6%** |

"Conversion" is the page's primary action (often a signup/lead), which maps to `signup_rate`. The
headline for a PLG-SaaS client: SaaS converts **42% below** the all-industry median — **3.8%** is normal,
not broken (within SaaS, hardware ~4.1% is best, data/infrastructure ~3.3% worst). The benchmark to beat
is your **own industry's** median, never the 6.6% overall.

**Channel swings conversion more than the page does** (SaaS, same report): email **16.9%** ≫ Google paid
search 5.1% > paid search overall 4.1% > paid social 2.9% > display **0.3%**. So a "low" `signup_rate`
can be a traffic-mix problem, not a page problem — segment by channel before fixing the page.

**How to apply.** Compare a client's visitor→signup rate to its **own industry** band. For PLG-SaaS,
~3.8% is the typical figure; moving from (say) 2% to 4% is a real win. Size the opportunity with the
number, then improve it with message match and friction reduction — don't treat a below-6.6% SaaS page
as underperforming by default. If conversion is low, split it by channel first.

**When it applies.** Sizing a landing-page/signup-conversion opportunity, or sanity-checking whether a
`signup_rate` is actually low for the archetype. The full industry table also gives a starting prior for
non-SaaS archetypes (flag borrowed priors per the charter).

**Caution (honesty).** A reference point, not a target or verdict — "conversion" definitions vary (lead
vs trial vs purchase) and the dataset skews to Unbounce customers and campaign/paid landing pages. All
figures here are **verified on the report's public pages** (overall, per-industry, and SaaS channels);
the deeper cut (sub-industries, top-quartile ranges) sits behind the report's email form. Pairs with
[[acq-tactic-message-match]] and [[acq-tactic-reduce-signup-friction]].
