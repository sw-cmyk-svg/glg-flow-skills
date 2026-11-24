---
id: free-to-paid
collection: benchmarks
title: Free-to-paid conversion — freemium vs. trial, PLG SaaS
grade: B
sources:
  - ref: "ChartMogul (Jan 2026), 'The SaaS Conversion Report' — survey of 200 B2B software products, $1–10M ARR typical; freemium distribution 25% <2.5%, 29% 2.5–7.5%, 25% 10–15%; freemium 'good' 3–5%, 'great' 8–12%; card-required trial 'good' 25–35%, 'great' 50–60%"
    year: 2026
  - ref: "First Page Sage (updated Sep 2025), 'SaaS Free Trial Conversion Rate Benchmarks' — 86 companies tracked Q1 2022–Q3 2025; opt-in (no card) trial-to-paid 17–18%, opt-out (card required) trial-to-paid 49–51%"
    year: 2025
status: active
---

## Claim
Freemium→paid for self-serve B2B SaaS holds close to the prior 2–5%
band as the "good" tier (ChartMogul's Jan 2026 survey of 200 B2B
products), with a real upside tail to 8–15% for tightly-targeted,
high-intent products. Trial→paid moved meaningfully higher than the
prior band once split by trial type: opt-in (no card required) trials
convert at 17–18% median (First Page Sage, 86-company tracked panel
through Q3 2025) — not the 8–15% this card's prior assumed — while
opt-out (card required upfront) trials convert roughly 3x higher, at
49–51%. The opt-in/opt-out split matters more than any single point
estimate; conflating them produces a meaningless blended average.

## Applicability — works when
- Freemium and trial motions are compared separately — they are
  different funnels with different intent filtering, not two flavors of
  the same number
- Trial comparisons are split opt-in (no card) vs. opt-out (card
  required) — collapsing them erases the single biggest driver of
  variance in this metric
- The cohort window matches (paying_conversion's 30-day-from-signup
  basis, or trial_to_paid's trial-length-plus-7-days basis)

## Backfires when
- Used as a target rather than a diagnostic — teams add a card-required
  step purely to chase the opt-out number without accounting for the
  volume loss upstream (opt-out trials convert fewer visitors into
  trials in the first place; it's a lever with a real trade-off, not a
  free win)
- Motion mismatch — comparing a freemium product's conversion rate
  against an opt-out trial's, or a self-serve motion's rate against a
  sales-assisted freemium (which converts higher because a human is
  involved in the upgrade path)
- The distribution is ignored in favor of the median — ChartMogul's data
  shows freemium conversion is bimodal (a quarter of products under
  2.5%, a quarter at 10–15%), so "median 8%" describes almost no actual
  product

## Growth applications
- Read `paying_conversion` (freemium cohorts) against the 3–5% "good" /
  8–12% "great" bands as a severity call; under 2.5% is a genuine
  red-flag worth diagnosing before running acquisition experiments
  upstream
- Read `trial_to_paid` split by whether the client's trial is opt-in or
  opt-out before applying any benchmark — applying the opt-out band
  (49–51%) to an opt-in trial will read a healthy 20% conversion as a
  failure
- If a client's trial currently has no card-capture step, use the
  opt-in/opt-out gap (roughly 3x) to size the experiment backlog item
  "add contextual card capture," while flagging the expected volume
  trade-off as part of the same experiment's success criteria

## Practice stance
We refuse to quote a single free-to-paid number without first asking
which motion (freemium or trial) and which trial type (opt-in or
opt-out) produced it — collapsing these into one blended figure is the
single most common way this metric gets misread. The band moves the
client's expectations; the split is what actually tells them what to
build next.
