---
id: visitor-to-signup
collection: benchmarks
title: Marketing-site visitor-to-signup — PLG SaaS
grade: B
sources:
  - ref: "Unbounce, 'Conversion Benchmark Report' (current edition, periodically updated) — SaaS category, median landing-page conversion 3.8%"
    year: 2024
  - ref: "Daydream (Apr 2026), 'Landing Page Conversion Rate Benchmarks for SaaS' — aggregated $5M–$50M ARR client cohort; self-serve product pages 4–10% median (best-in-class 12–18%), demo-request pages 1.5–4%, content pages 0.5–2%"
    year: 2026
status: active
---

## Claim
Marketing-site visitor→signup for self-serve PLG SaaS sits roughly 2–5%
overall, anchored by Unbounce's Conversion Benchmark Report SaaS-category
median of 3.8% (current edition). But the number is sharply
landing-page-type dependent: Daydream's 2026 client-cohort data
splits it into self-serve product pages at 4–10% (best-in-class 12–18%),
demo-request pages at 1.5–4%, and top-of-funnel content pages at
0.5–2%. Treat "2–5%" as the blended default and the split as the real
diagnostic tool.

## Applicability — works when
- Comparing signup rate from a self-serve product/pricing page, not a
  demo-request or content page — mixing these into one blended number
  erases the diagnostic value
- Traffic source and intent are comparable (paid vs. organic, cold vs.
  warm) — email traffic reportedly converts multiples better than other
  sources and will skew a blended rate upward
- The window and cohort basis match — visitor counted per unique_visitors
  definition (distinct people per ISO week), not sessions

## Backfires when
- Used as a target rather than a diagnostic — teams narrow traffic
  sources or add friction-reducing dark patterns just to move the ratio,
  degrading lead quality without growing revenue
- Motion mismatch — comparing a demo-request-gated enterprise motion
  (1.5–4% is normal there) against a self-serve PLG band (2–10%) as if
  they're the same funnel
- Page type isn't segmented before comparing — a company blending
  content-page and product-page traffic into one number will always look
  worse than a company that reports product-page traffic alone

## Growth applications
- Read `signup_rate` against the 2–5% blended band for a fast severity
  call, then re-segment by page type before concluding there's a real
  leak — a 3% blended rate could hide a healthy 8% product-page rate
  dragged down by a weak content funnel
- If `signup_rate` sits under 2% even on product/pricing pages, treat it
  as a message-market-fit problem on the page itself, not a funnel-volume
  problem
- Use the self-serve vs. demo-page split to sanity-check which motion a
  client's site is actually optimized for before recommending
  experiments

## Practice stance
We never quote a single visitor-to-signup number back to a client without
first asking which page type produced it. A blended site-wide rate is a
rumor about ten different pages; the band only becomes useful once it's
split by page intent. We hold the line at 2–5% as the sanity-check floor,
not the goal.
