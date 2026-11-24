---
id: prioritization-ice-pxl
collection: methods
title: Prioritization scoring — ICE and PXL
grade: C
sources:
  - ref: "Ellis & Brown (2017), 'Hacking Growth', Crown Business"
    year: 2017
  - ref: "Laja / CXL (ConversionXL), 'PXL: A Better Way to Prioritize Your A/B Tests', conversionxl.com"
    year: 2016
status: active
---

## Claim
Scoring frameworks like ICE (Impact, Confidence, Ease) and PXL impose
useful ordering discipline on a backlog of experiment ideas, but the
scores themselves are subjective estimates, not measurements. Treat the
resulting rankings as coarse buckets — top third, middle, bottom — not as
a precise ordering where item #7 is meaningfully ahead of item #8.

## Applicability — works when
- Used to triage a large, unsorted backlog into rough tiers before
  deeper analysis (MDE, feasibility), not to settle a close call between
  two similar ideas
- Multiple people score independently and scores are averaged or
  discussed, surfacing disagreement rather than laundering one person's
  opinion into a number

## Backfires when
- Treating a 0.5-point ICE gap as a real ranking; confidence theater
  where made-up numbers acquire false authority in stakeholder decks
- One person scores alone and the framework just formalizes their
  existing gut preference under the appearance of rigor
- Scores are set once and reused for months without revisiting them
  against new evidence — shipped experiments, fresh data — as it arrives

## Growth applications
- Triage the activation_rate experiment backlog into top/middle/bottom
  tiers with ICE before running MDE analysis on the top tier only
- Use PXL's "does this test a genuinely new hypothesis" question to keep
  weekly_active_users experiment slots from filling with redundant
  variant tweaks
- Re-score the paying_conversion backlog quarterly against fresh
  w4_retention results instead of letting initial scores fossilize

## Practice stance
We use ICE/PXL to sort a backlog into rough tiers, never to justify a
precise ranking, and we require at least two independent scorers before a
score reaches a stakeholder deck. We refuse to present a composite score
as if it were a measurement — it is a structured opinion, and we label it
as one.
