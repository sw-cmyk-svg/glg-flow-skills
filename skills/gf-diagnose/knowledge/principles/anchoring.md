---
id: anchoring
collection: principles
title: Anchoring
grade: A
sources:
  - ref: "Tversky & Kahneman (1974), 'Judgment under Uncertainty: Heuristics and Biases', Science 185"
    year: 1974
  - ref: "Furnham & Boo (2011), 'A literature review of the anchoring effect', The Journal of Socio-Economics"
    year: 2011
status: active
---

## Claim
The first number a person encounters — even an arbitrary or irrelevant
one — pulls subsequent numeric judgments toward it. This holds across
probability estimates, negotiations, and pricing, and is one of the
most replicated effects in judgment research; the 2011 review found it
robust across dozens of domains and elicitation methods.

## Applicability — works when
- The judgment is genuinely uncertain (the person has no firm reference
  price or estimate of their own)
- The anchor is presented before the target judgment, not after
- The comparison is numeric — price, quantity, duration, percentage

## Backfires when
- Anchors set below the market or the user's expectation drag
  willingness-to-pay down, not up — anchoring cuts both ways, and a
  poorly chosen "was $X" or low starting tier trains users to expect less
- The anchor is transparently arbitrary or self-serving, which invites
  discounting of the entire number (sophisticated buyers adjust it away)
- Repeated exposure to the same anchor across a session desensitizes it

## Growth applications
- Show the highest-value plan first so mid-tier pricing reads as
  reasonable by comparison (paying_conversion)
- Anchor a usage-based cost estimate with a representative high number
  before showing the actual quote (arpu)
- Anchor time-to-value copy with the fastest recorded onboarding time,
  not the average, to compress perceived effort (time_to_activation)

## Practice stance
We treat anchoring as a first-look lever, not a permanent fixture — it
degrades with repeat exposure, so we test it on first-visit and new-cohort
surfaces, not on pages returning users see weekly. We refuse anchors we
can't defend as roughly true; a low anchor that undercuts our own
willingness-to-pay is a bigger risk than no anchor at all.
