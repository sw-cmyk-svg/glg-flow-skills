---
id: match-measurement-horizon-to-mechanism
collection: judgment
title: Match the measurement horizon to the mechanism, not the reporting cycle
grade: C
sources:
  - ref: "Galangal Lab practice experience — recurring pattern of teams killing UX/onboarding changes for short-term revenue flatness while celebrating novelty-driven feature spikes"
    year: 2026
status: active
---

## Claim
Measure a change over a horizon matched to its mechanism. UX, onboarding,
and retention effects compound slowly and need a longer observation window;
feature-launch spikes must be discounted for novelty before being called a
win. Short-window revenue is the wrong judge for a long-mechanism change,
and without a control group a lift can't be attributed to a release at all
— seasonality, concurrent changes, and marketing are live confounds.

## Applicability — works when
- Evaluating a UX, onboarding, or retention-oriented change against revenue
  or conversion in the weeks immediately after launch
- A feature launch shows an immediate metric spike — check for a novelty
  effect (does the lift persist past the first cohort's first exposure?)
  before declaring a win
- No controlled experiment ran alongside a release — treat any coincident
  lift as a hypothesis, not an attributed result, given untracked confounds

## Backfires when
- "It's a long-term play" is used to indefinitely shield a change that
  genuinely isn't working — the longer window needs its own endpoint and
  its own bar, not an open-ended pass
- An over-long observation window lets a real regression run uncorrected
  while everyone waits for the "compounding" effect to show up

## Growth applications
- Judge onboarding/UX changes against w4_retention or w1_retention trend
  over multiple cohorts, not week-one weekly_revenue
- Discount an immediate arpu or weekly_revenue spike after a feature launch
  for novelty before reporting it as a durable lift — recheck after the
  initial cohort's novelty fades
- Where no control group ran, label a coincident lift as an unattributed
  correlation, not a causal result, regardless of which metric moved

## Practice stance
We set the measurement window before the change ships, sized to its
mechanism, not to whatever the next reporting cycle happens to be — and we
hold ourselves to it on both ends: we don't kill a long-mechanism change
early, and we don't let "give it time" become permanent cover for something
that isn't working.
