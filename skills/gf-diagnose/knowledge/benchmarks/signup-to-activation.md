---
id: signup-to-activation
collection: benchmarks
title: Signup-to-activation within first week — PLG SaaS
grade: B
sources:
  - ref: "Rachitsky & Timen (2022), 'What is a good activation rate', Lenny's Newsletter — survey of 500+ products; SaaS-only median 30%, average 36% (the field's reference definition study)"
    year: 2022
  - ref: "Agile Growth Labs (Aug 2025), 'User Activation Rate Benchmarks 2025' — SaaS overall avg 37.5%, PLG-specific avg 34.6%, sales-led 41.6%"
    year: 2025
  - ref: "Userpilot (2024), 'SaaS Product Metrics Benchmark Report 2024' — 547 SaaS companies"
    year: 2024
status: active
---

## Claim
Self-serve B2B SaaS signup→activation within the first week sits roughly
20–40%, median close to 30%. The original reference study (Rachitsky &
Timen, Lenny's Newsletter, 2022, n=500+ products) put the SaaS-only median
at 30% and average at 36%; more recent 2024–2025 numbers (Userpilot's
547-company 2024 report, and Agile Growth Labs' 2025 synthesis, which
appears to draw on the same Userpilot data rather than an independent
sample) land in the same 34–38% neighborhood for PLG specifically. The
band held up under refresh — the number that moves most across sources isn't the
level, it's the definition: every report's activation event is a
different, company-specific "aha" action, so a 30% activation rate from
one company is not the same 30% as another's.

## Applicability — works when
- Comparing against a company that defines its activation event as a real
  value moment (not a setup step like "profile completed") and measures
  it within the same 7-day window
- The comparison is like-for-like on motion — PLG-specific benchmarks
  (34–38%) run lower than sales-led (41–42%) because SLG activation
  events are typically gated by onboarding calls, not self-serve behavior
- Used as a triage signal on a fresh diagnostic, not as a target baked
  into a roadmap

## Backfires when
- Used as a target rather than a diagnostic — teams redefine "activation"
  downward (e.g., "viewed the dashboard" instead of "completed first core
  action") until the number clears the benchmark, which destroys its
  value as a leak detector
- Motion is mismatched — comparing a sales-assisted trial's activation
  rate against this self-serve PLG band, or vice versa
- The activation event itself hasn't been validated as predictive of
  retention (see the growth-applications note below) — a well-hit
  benchmark on a poorly chosen event tells you nothing

## Growth applications
- Read `activation_rate` against this band as a severity call: <20% is a
  red-flag leak worth an immediate diagnostic session; 20–30% is a
  legitimate optimization candidate; >40% means look elsewhere in the
  funnel for the growth constraint
- Before trusting the number, confirm the activation event definition
  matches "a value moment reached within 7 days" per the PLG overlay —
  not a proxy setup step
- Pair with `time_to_activation`: a cohort hitting 30% activation but
  with a long median time-to-activation is a different problem (weak
  onboarding pacing) than one hitting 30% quickly (weak product-market
  fit for late activators)

## Practice stance
We treat this as a band to locate severity, not a score to hit. The
first thing we do with a client's activation number is interrogate the
event definition before we compare it to anything — a benchmark applied
to an undefined or gameable activation event is worse than no benchmark
at all. We refuse to let a client redefine activation mid-engagement
just to clear this line.
