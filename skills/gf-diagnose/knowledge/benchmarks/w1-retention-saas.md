---
id: w1-retention-saas
collection: benchmarks
title: Week-1 retention curve — PLG SaaS cohorts
grade: C
sources:
  - ref: "Amplitude (2025), '2025 Product Benchmark Report' / 'The 7% Retention Rule' — 2,600+ companies; day-7 single-day-return top quartile ~7%; enterprise segment: top decile 12.4%, enterprise median 2.1%"
    year: 2025
  - ref: "Userpilot (2024), 'SaaS Product Metrics Benchmark Report 2024' — 547 companies; month-1 retention PLG 48.4%, SLG 39.1% (no week-1-specific breakout published)"
    year: 2024
status: active
---

## Claim
This card's prior — a 40–60% week-1 retention band for PLG SaaS
cohorts — could not be corroborated by any ≥2024 large-sample report
isolating that exact window. The two most credible reports found bracket
wildly different numbers because they measure wildly different things:
Amplitude's 2025 Product Benchmark Report (2,600+ companies) measures
single-day-7 return and puts the top quartile at only ~7% (in its
enterprise segment: top decile 12.4%, enterprise median 2.1%);
Userpilot's 2024 report (547 companies)
measures month-1 active-any-day retention and finds PLG cohorts at 48.4%.
Neither matches the spec's `w1_retention` definition (active on any day
7–13). Read this card as a caution about definition variance, not a
verified level — state any specific target you're given with a grain of
salt until you've confirmed the exact window and activity bar it uses.

## Applicability — works when
- The retention definition is stated explicitly (single-day return vs.
  N-day active window vs. rolling-month active) before any number is
  compared across companies or sources
- The comparison is used to read curve *shape* — does it flatten by
  week 4, or does it keep bleeding — rather than to validate a specific
  week-1 percentage
- Same cohort basis (signup-week cohorts, not calendar-month cohorts) on
  both sides of the comparison

## Backfires when
- Used as a target rather than a diagnostic — a 40–60% figure quoted
  without its definition gets treated as gospel and teams optimize
  toward whichever loose definition clears it
- Motion mismatch — comparing a freemium product's low-intent-explorer
  cohort against a paid-trial cohort's retention, which is structurally
  higher because the signup already filtered for intent
- A single-week snapshot is read as a verdict — one good or bad week-1
  number without w4 as a reference tells you nothing about whether the
  curve is flattening or still bleeding

## Growth applications
- Do not gate a go/no-go decision on `w1_retention` against a specific
  published percentage; instead compare `w1_retention` to `w4_retention`
  within the same client's own cohorts — a curve that's still dropping
  steeply from w1 to w4 is the real signal, independent of the w1 level
- If a specific w1 number is demanded for a diagnostic, present it
  bracketed (Amplitude's single-day floor of ~2–12% vs. Userpilot's
  month-1 ceiling of ~40–48%) rather than as a point estimate, so the
  client understands it's not calibrated to their exact metric
- Use week-over-week curve shape, not the raw w1 level, to decide whether
  an activation-focused or a habit-formation-focused experiment backlog
  is the higher-leverage next move

## Practice stance
We flag this card's grade honestly: the sourcing here is weak, and we
say so to the client rather than presenting a confident band we can't
back. A retention percentage without its window and activity-bar
definition attached isn't a benchmark, it's a rumor with a percent sign
on it — and on this specific metric, we haven't found a report that
removes the rumor.
