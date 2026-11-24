---
id: choice-overload
collection: principles
title: Choice overload
grade: C
sources:
  - ref: "Iyengar & Lepper (2000), 'When Choice is Demotivating: Can One Desire Too Much of a Good Thing?', Journal of Personality and Social Psychology"
    year: 2000
  - ref: "Scheibehenne, Greifeneder & Todd (2010), 'Can There Ever Be Too Many Options? A Meta-Analytic Review of Choice Overload', Journal of Consumer Research"
    year: 2010
status: active
---

## Claim
More options can reduce satisfaction and conversion — the famous jam
study found six flavors outsold twenty-four. But the 2010 meta-analysis
across the accumulated literature found the average effect across
studies is approximately zero: sometimes more choice helps, sometimes it
hurts, and the sign depends entirely on moderators (assortment
complexity, time pressure, prior preference strength, expertise). Graded
C: not because the underlying studies are weak individually, but because
"fewer options convert better" is not a reliable average-case claim —
it's a claim that's only true under specific, identifiable conditions.

## Applicability — works when
- Users are unfamiliar with the category and have no strong prior
  preference (novices are the group most reliably burdened by choice)
- Options are hard to compare (differ on many dimensions at once) rather
  than cleanly differentiated
- The decision is made under time pressure or low motivation

## Backfires when
- Users have strong, differentiated preferences or real feature needs —
  cutting options here removes the option they actually wanted, not
  cognitive load
- The reduced set is three near-identical plans with cosmetic naming
  differences — that isn't simplified choice, it's choice with the
  information removed, and it frustrates rather than helps
- Expert or repeat users, who benefit from more comparison surface, get
  a worse experience than novices would in the same reduced set

## Growth applications
- Reduce plan count for first-time visitors on the pricing page while
  keeping a "compare all plans" path for return visitors (signup_rate)
- Simplify the first-run feature set shown during onboarding to the
  3–4 that map to the user's stated goal (activation_rate, time_to_activation)
- Segment: fewer options for self-serve trial signups, full catalog for
  sales-assisted / expansion conversations (trial_to_paid, expansion_signups)

## Practice stance
We don't apply "reduce options" as a default — the meta-analytic null
average means we treat it as a hypothesis to test per segment, not a
house rule. We look specifically at whether our users are novices facing
a genuinely hard-to-compare set before touching option count, and we
refuse to relabel three similar plans as "simplified" when what actually
changed is that information was hidden.
