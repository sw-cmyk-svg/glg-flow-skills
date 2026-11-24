# Retention corpus — index

**Version:** 0.0.5 (waves 1–6 — 2026-11-18) · business_model: `plg-saas`
**Status:** drafting (I draft, founder vets). **19 units — all six families ≥3 (robust bar met).**
Target proof size ~20–40 units, **all six tactic families at ≥3** (the robust bar from the Activation
corpus). Same curation rules: authored distilled note + citation, I-draft-you-vet,
verification-as-drafting, persuasion-ethics principle.

**Curation principle — persuasion & ethics (inherited).** Persuasion / behavioral tactics are
allowed, but every persuasion-adjacent unit MUST carry an explicit `Caution (ethics):` line.
Retention is the stage where compulsion lives (variable-reward loops, streak pressure, manipulative
notifications), so this is load-bearing here. Regulated archetypes (bank/wallet, betting) get a
compliance caution, not a ban; outright dark patterns are documented only as anti-patterns.

| id | unit_type | tactic_family | sub_stage | verified |
|---|---|---|---|---|
| [ret-benchmark-retention-curve-pendo](units/ret-benchmark-retention-curve-pendo.md) | benchmark | engagement-depth | retention-curve | ✅ Pendo first-party (6,800+ apps) |
| [ret-benchmark-stickiness-pendo](units/ret-benchmark-stickiness-pendo.md) | benchmark | habit-formation | habit | ✅ Pendo first-party (6,800+ apps) |
| [ret-framework-hook-model](units/ret-framework-hook-model.md) | framework | habit-formation | habit | ⚠ ethics; ✅ Eyal (Hooked) |
| [ret-principle-fogg-behavior-model](units/ret-principle-fogg-behavior-model.md) | principle | habit-formation | habit | ⚠ ethics (prompts); ✅ Fogg (B=MAP) |
| [ret-tactic-variable-rewards-habit](units/ret-tactic-variable-rewards-habit.md) | tactic | habit-formation | habit | ⚠⚠ strongest ethics; ✅ book (Zeiler/Mazar) |
| [ret-principle-sunk-cost](units/ret-principle-sunk-cost.md) | principle | value-reinforcement | habit | ⚠ ethics; ✅ book (Arkes&Blumer/Kantar) |
| [ret-principle-stored-value-switching-costs](units/ret-principle-stored-value-switching-costs.md) | principle | value-reinforcement | habit | ⚠ ethics (lock-in); ✅ Hook + endowment |
| [ret-principle-feature-adoption-breadth](units/ret-principle-feature-adoption-breadth.md) | principle | engagement-depth | engagement | ⚠ correlational; ✅ Pendo |
| [ret-tactic-guide-to-value-continuously](units/ret-tactic-guide-to-value-continuously.md) | tactic | engagement-depth | engagement | ✅ Pendo (vendor-bias flagged) |
| [ret-principle-loss-aversion-winback](units/ret-principle-loss-aversion-winback.md) | principle | re-engagement | resurrection | ⚠ ethics; ✅ book (T&K/Gonzales) |
| [ret-tactic-reengagement-lifecycle](units/ret-tactic-reengagement-lifecycle.md) | tactic | re-engagement | resurrection | ⚠ ethics (spam); ✅ Fogg + practice |
| [ret-tactic-detect-churn-signals-early](units/ret-tactic-detect-churn-signals-early.md) | tactic | re-engagement | resurrection | ⚠ correlational; ✅ Pendo + practice |
| [ret-principle-illusion-of-effort](units/ret-principle-illusion-of-effort.md) | principle | value-reinforcement | engagement | ⚠ honesty; ✅ book (Kruger 2004 / Barnes 2015) |
| [ret-principle-relevance-decay](units/ret-principle-relevance-decay.md) | principle | personalization-relevance | engagement | ⚠ ethics/privacy; ✅ PLG practice |
| [ret-tactic-behavioral-segmentation](units/ret-tactic-behavioral-segmentation.md) | tactic | personalization-relevance | engagement | ⚠ correlational + data boundary; ✅ PLG practice |
| [ret-tactic-next-best-action](units/ret-tactic-next-best-action.md) | tactic | personalization-relevance | engagement | ⚠ ethics (attention); ✅ PLG practice |
| [ret-principle-network-effects-retention](units/ret-principle-network-effects-retention.md) | principle | social-network | habit | ⚠ ethics (coerced invites); ✅ Balfour/Metcalfe |
| [ret-tactic-collaboration-invites](units/ret-tactic-collaboration-invites.md) | tactic | social-network | habit | ⚠ ethics (consent/spam); ✅ Hook + practice |
| [ret-tactic-community-social-accountability](units/ret-tactic-community-social-accountability.md) | tactic | social-network | habit | ⚠⚠ ethics (shaming/pressure); ✅ book ch.6 + practice |

**Tactic-family coverage (robust — all ≥3):** habit-formation ✓✓✓✓, engagement-depth ✓✓✓,
value-reinforcement ✓✓✓, re-engagement ✓✓✓, personalization-relevance ✓✓✓, social-network ✓✓✓.
**Benchmark priors anchored:** retention curve (1-mo avg 38.8%, 3-mo 30.1%, flattening = PMF);
stickiness (WAU/MAU 53% avg / 77% best-in-class). Both Pendo first-party, definition-vs-spec caveat noted.
**Persuasion-adjacent (mandatory `Caution (ethics):`):** hook-model, fogg (prompts), variable-rewards
(strongest), lifecycle (spam), loss-aversion, community-social-accountability (shaming/pressure).
Retention is the compulsion-prone stage, so these carry the heaviest cautions.
**Corpus status:** robust bar met (all six families ≥3, 19 units). Founder vet pending on the
ethics-sensitive units (habit-formation + re-engagement + social-accountability) before the
Retention specialist is authored. Optional future depth (flagged in SOURCES.md): Hooked / Tiny Habits
books for Eyal's Manipulation Matrix; more first-party retention benchmarks.

**First-wave plan (drafting order):**
1. **Benchmarks (anchor first):** 1-month retention ~46.9% (Userpilot); Pendo retention + stickiness;
   Amplitude retention + the activation→retention link (reuse). → gives the Analyze/benchmark priors.
2. **Habit-formation (behavioral core):** the Hook model (Eyal) + Fogg B=MAP + the book's uncertain
   rewards (ch.12) — each with the ethics caution. → the heaviest-ethics family.
3. **Value-reinforcement:** sunk cost (book ch.5), accumulated/earned value, saved state / switching
   costs.
4. Then **engagement-depth**, **re-engagement** (lifecycle), **personalization-relevance**,
   **social-network** to ≥3 each.

**Reuses:** the Activation corpus's PDFs (Userpilot/Pendo/Amplitude) and the book epub are in hand;
Balfour "retention is the engine" is the strategy spine.
