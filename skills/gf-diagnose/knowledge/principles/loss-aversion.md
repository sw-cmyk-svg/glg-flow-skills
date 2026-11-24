---
id: loss-aversion
collection: principles
title: Loss aversion
grade: B
sources:
  - ref: "Kahneman & Tversky (1979), 'Prospect Theory: An Analysis of Decision under Risk', Econometrica"
    year: 1979
  - ref: "Gal & Rucker (2018), 'The Loss of Loss Aversion: Will It Loom Larger Than Its Gain?', Journal of Consumer Psychology"
    year: 2018
status: active
---

## Claim
Framed as a loss, an outcome motivates more than the same outcome framed
as an equivalent gain. The direction of the effect is well established
since prospect theory, but the 2018 Gal & Rucker review found the
magnitude far less consistent than assumed — several canonical
demonstrations don't replicate at the claimed size, and in some
conditions gains and losses move people about equally. Grade B, not A:
the effect exists, but "losses loom twice as large" is a folk exaggeration
of a real but variable phenomenon.

## Applicability — works when
- The framing describes a genuine, concrete loss (losing access, losing
  progress, losing a discount already implied) rather than an abstract one
- The audience is making a fast, low-deliberation decision
- The loss is truthful — the user really would forfeit something

## Backfires when
- Loss-framed copy in trust-sensitive flows (billing, data deletion,
  account security) reads as manipulative rather than motivating, and
  damages trust more than the frame gains in conversion
- Overused across every CTA, it habituates — users learn to ignore
  urgency language, which also dulls it for the times it's genuinely true
- The claimed loss is exaggerated or false, which is both an ethical
  problem and a durable trust cost once discovered

## Growth applications
- "You'll lose your saved progress" framing on exit-intent for
  incomplete onboarding (activation_rate)
- Expiring-credit framing on trial-to-paid conversion emails, only when
  the credit genuinely expires (trial_to_paid)
- Downgrade-consequence framing ("lose access to X") on cancellation
  flows, stated factually (expansion_signups)

## Practice stance
We use loss framing only where the loss is literal and use gain framing
as the default elsewhere — the evidence doesn't support loss framing as
a universal multiplier, so we don't treat it as one. On billing and
security surfaces specifically, we refuse loss-framed urgency; the trust
cost there is asymmetric and not worth the modest, contested lift.
