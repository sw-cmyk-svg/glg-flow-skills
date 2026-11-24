---
id: acq-benchmark-cac-payback
stage: acquisition
sub_stage: paid-acquisition
business_model: plg-saas
tactic_family: paid-acquisition
unit_type: benchmark
metric: [new_signups]
provenance: public
sources:
  - "High Alpha, 2024 SaaS Benchmarks Report (in partnership with OpenView, Paddle, Tremont), p.38 'CAC Payback Increases as Companies Mature' — CAC payback period in months, median by ARR band (verified at primary)."
  - "Benchmarkit, 2025 B2B SaaS Performance Metrics Benchmarks (May 2025), 'Customer Acquisition Efficiency' — New Customer CAC Ratio (verified at primary; a ratio, not a payback period)."
---
**Benchmark prior — CAC payback is stage-dependent and rises as a company matures: ~2 months early, ~14, up to ~20 at scale.**

Median **CAC payback period in months** by ARR band (High Alpha 2024): **<$1M ≈ 2mo**, **$1–5M ≈
8mo**, **$5–20M ≈ 14mo**, **$20–50M ≈ 14mo**, **>$50M ≈ 20mo** (upper-quartile runs 8 / 14 / 22 / 22 /
27). The headline is the *shape*, not a single number: payback **increases as companies scale and their
cheaper early channels saturate**, so there is no one "SaaS median" — a sub-$5M company paying back in
~8 months and a >$50M company at ~20 months are both normal for their stage. The common "**under 12
months = healthy**" rule only describes early-to-mid companies; larger ones routinely run longer.

A complementary efficiency read (Benchmarkit 2025, CY-24 data): the median **New Customer CAC Ratio is
~$2.00** — $2 of sales-and-marketing to add $1 of new-customer ARR, up ~14% year over year — with the
blended ratio (new + expansion) around $1.40. CAC *ratio* and CAC *payback* are different lenses on the
same efficiency; quote whichever the client actually tracks.

**How to apply.** Judge a client's CAC payback against its **ARR stage**, not a blanket "<12mo," and
expect it to lengthen as they grow and scale paid channels. Use payback as the primary test of whether
*paid* acquisition is sustainable (can the business fund the gap to payback?). Rising payback with scale
is the expected signal of channel saturation, not a failure.

**When it applies.** Assessing paid-acquisition sustainability, comparing channels on efficiency, or
setting a stage-appropriate CAC target.

**Caution (honesty).** CAC and payback have **no canonical spec id** in `spec/metric-spec.yaml` — flag
the client's own definition (which costs are in CAC? gross-margin-adjusted?). **Early-stage payback is
often understated**: the report flags that young companies frequently omit founder sales salaries and
CS/support costs from CAC, flattering the number (hence the ~2-month <$1M figure). This is PLG/B2B-SaaS
survey data — other archetypes differ. Pairs with [[acq-principle-ltv-cac-heuristic]] and
[[acq-principle-channel-saturation]] (the same maturation/saturation effect).
