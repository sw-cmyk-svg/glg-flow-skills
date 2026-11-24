---
id: post-hoc-segments
collection: methods
title: Post-hoc segmentation and the multiple-comparisons trap
grade: A
sources:
  - ref: "Kohavi, Tang & Xu (2020), 'Trustworthy Online Controlled Experiments', Cambridge University Press — ch. 3 on Twyman's law and segment fishing"
    year: 2020
status: active
---

## Claim
Unplanned subgroup analysis multiplies the number of comparisons made
against the same result. Standard multiple-comparisons statistics show
that with 20 segments examined at α=0.05, you expect roughly one false
"winner" by chance alone. "It worked for mobile users in Spain" — found
by slicing the data after the fact — is usually noise, not signal
(Twyman's law: any figure that looks interesting is probably wrong).

## Applicability — works when
- Segments were defined and pre-registered before the test started
  (device, plan tier, acquisition channel chosen in advance)
- The number of segments examined is disclosed and a multiplicity
  correction is applied before any segment result is reported

## Backfires when
- Even pre-registered segments need multiplicity correction; and
  dismissing all segmentation loses real heterogeneity — the sin is
  unplanned discovery presented as confirmation
- A pattern noticed after seeing results ("let's check mobile, it looked
  good") gets sliced out and reported as a finding
- Small per-segment sample sizes make a real effect indistinguishable
  from noise, but the segment gets reported with false precision anyway

## Growth applications
- Pre-register a small set of segments (new vs. returning) for
  signup_rate tests and apply a multiplicity correction before reporting
  any segment-level result
- Treat "activation_rate improved for enterprise trial users" as a
  hypothesis for a follow-up test, not a conclusion, when it emerged
  post-hoc
- Report w4_retention by plan tier only when tier was a planned,
  corrected-for segment — not by every dimension the dashboard happens to
  expose

## Practice stance
We pre-register segments before a test launches and correct for the
number we examine; any segment discovered after looking at results
becomes a hypothesis for the next test, never a headline finding. We
refuse "it worked for X" claims that weren't planned and corrected for,
and we refuse to throw away real, well-powered segment heterogeneity just
because pre-registration discipline is hard.
