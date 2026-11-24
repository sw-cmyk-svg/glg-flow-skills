---
id: test-full-weeks
collection: methods
title: Run tests in whole weeks
grade: B
sources:
  - ref: "Kohavi, Tang & Xu (2020), 'Trustworthy Online Controlled Experiments', Cambridge University Press — experiment duration and weekly-cycle guidance"
    year: 2020
status: active
---

## Claim
Run experiments in whole-week multiples (7, 14, 21 days), never partial
weeks. Day-of-week mix shifts both traffic composition (channel, device,
new-vs-returning ratio) and user behavior, so a test that starts or stops
mid-week compares non-equivalent populations and biases the result.

## Applicability — works when
- The metric or its traffic source has known day-of-week seasonality
  (B2B weekday peaks, B2C weekend spikes, campaign-driven Monday surges)
- The test's minimum runtime can be planned in whole weeks before launch,
  tied to the power calculation (see mde-sample-size)

## Backfires when
- Stopping mid-week after a "significant" weekend reads novelty +
  weekend-user mix as truth
- Extending past the power-calculated stopping point just to round up to
  a whole-week boundary adds cost without adding information
- The organization's own marketing or release calendar shifts mid-test,
  so even whole weeks stop being comparable to each other

## Growth applications
- Schedule paying_conversion tests in full 7-day multiples so weekday
  and weekend traffic mix is represented equally in every arm
- Align w1_retention cohort start dates to calendar weeks so each cohort
  enters with the same day-of-week composition
- Read weekly_active_users only at week boundaries — never compare a
  mid-week snapshot against a prior full week

## Practice stance
We set an experiment's minimum runtime in whole weeks before it launches,
derived from the MDE calculation, and we refuse to call a result before
that boundary regardless of interim significance. If a stakeholder wants
an earlier read, the fix is a properly designed sequential test next
time, not an early stop on this one.
