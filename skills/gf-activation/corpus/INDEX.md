# Activation corpus — index

**Version:** 0.0.8 (waves 1–9 — 2026-11-17) · business_model: `plg-saas`
**Status:** drafting (I draft, founder vets). Target proof size ~20–40 units. **29 units — all six families at ≥3.**
See `SOURCES.md` for sourcing + verification status. Units distil + cite; never reproduce.

**Curation principle — persuasion & ethics (founder decision 2026-11-17).** Persuasion / behavioral
tactics are **allowed** in the corpus, but every persuasion-adjacent unit MUST carry an explicit
`Caution (ethics):` line drawing the line between a legitimate nudge and a dark pattern, plus, for
sensitive archetypes (e.g. bank/wallet), a heightened caution advising regulatory / compliance
review rather than a blanket ban. Outright dark
patterns (false scarcity, forced continuity, manufactured regret/FOMO) are documented **only as
anti-patterns to avoid**, never prescribed. This mirrors `copilot/GUARDRAILS.md`.

| id | unit_type | tactic_family | sub_stage | verified |
|---|---|---|---|---|
| [act-principle-time-to-value](units/act-principle-time-to-value.md) | principle | motivation | aha | concept (no stat) |
| [act-principle-goal-dilution](units/act-principle-goal-dilution.md) | principle | guidance | onboarding | ✅ book (Shotton/Flicker) |
| [act-principle-make-it-easy-friction](units/act-principle-make-it-easy-friction.md) | principle | friction-reduction | onboarding | ✅ book (Shotton/Flicker) |
| [act-framework-locate-the-problem](units/act-framework-locate-the-problem.md) | framework | guidance | onboarding | ✅ Amplitude (illustrative) |
| [act-tactic-value-before-signup](units/act-tactic-value-before-signup.md) | tactic | friction-reduction | signup | ✅ UserGuiding |
| [act-benchmark-tour-completion-by-steps](units/act-benchmark-tour-completion-by-steps.md) | benchmark | friction-reduction | onboarding | ✅ Produktly |
| [act-benchmark-activation-predicts-retention](units/act-benchmark-activation-predicts-retention.md) | benchmark | motivation | aha | ✅ Amplitude |
| [act-benchmark-activation-rates-by-percentile](units/act-benchmark-activation-rates-by-percentile.md) | benchmark | friction-reduction | onboarding | ✅ Amplitude |
| [act-design-embedded-cues-over-tours](units/act-design-embedded-cues-over-tours.md) | case-study | guidance | onboarding | ✅ UserGuiding |
| [act-tactic-segment-at-signup](units/act-tactic-segment-at-signup.md) | tactic | personalization | signup | ✅ UserGuiding (collection only) |
| [act-principle-social-proof](units/act-principle-social-proof.md) | principle | social-proof | signup | ⚠ ethics-caution; 2ndary stats flagged |
| [act-tactic-endowed-progress](units/act-tactic-endowed-progress.md) | tactic | incentive | onboarding | ⚠ ethics-caution; ✅ Nunes&Drèze (2ndary) |
| [act-design-embedded-prompt-starters](units/act-design-embedded-prompt-starters.md) | case-study | guidance | onboarding | ✅ AI UX Playground (pattern, no metrics) |
| [act-framework-onboarding-shape](units/act-framework-onboarding-shape.md) | framework | guidance | signup | ✅ AI UX Playground (step counts only) |
| [act-principle-implied-social-proof](units/act-principle-implied-social-proof.md) | principle | social-proof | signup | ⚠ ethics-caution; ✅ book (HMRC/Keizer/Peterson) |
| [act-tactic-uncertain-rewards](units/act-tactic-uncertain-rewards.md) | tactic | incentive | onboarding | ⚠ ethics-caution (gambling); ✅ book (Zeiler/Mazar) |
| [act-design-role-cards-outcome-framed](units/act-design-role-cards-outcome-framed.md) | case-study | personalization | signup | ✅ AI UX Playground (pattern, no metrics) |
| [act-design-branch-checklist-by-experience](units/act-design-branch-checklist-by-experience.md) | case-study | personalization | onboarding | ✅ Appcues/Hotjar (+26% install, rel.) |
| [act-design-daisy-chained-checklists](units/act-design-daisy-chained-checklists.md) | case-study | incentive | onboarding | ✅ Appcues (2%→25% completion) |
| [act-benchmark-product-tour-engagement](units/act-benchmark-product-tour-engagement.md) | benchmark | guidance | onboarding | ✅ Chameleon (platform data, 550M) |
| [act-benchmark-presignup-demo-and-touchpoints](units/act-benchmark-presignup-demo-and-touchpoints.md) | benchmark | friction-reduction | signup | ⚠ 2ndary (Navattic/Arcade/PLA via Chameleon) |
| [act-benchmark-activation-rate-saas-2025](units/act-benchmark-activation-rate-saas-2025.md) | benchmark | motivation | aha | ✅ Userpilot first-party (547 cos; activation 62) |
| [act-benchmark-checklist-completion-saas](units/act-benchmark-checklist-completion-saas.md) | benchmark | incentive | onboarding | ✅ Userpilot first-party (188 cos, ~19%) |
| [act-tactic-video-in-onboarding](units/act-tactic-video-in-onboarding.md) | tactic | guidance | onboarding | ⚠ correlational (Userpilot top activators) |
| [act-principle-activation-first](units/act-principle-activation-first.md) | principle | motivation | aha | ✅ Poyar (preview) + Verna (2ndary, flagged) |
| [act-framework-four-fits-context](units/act-framework-four-fits-context.md) | framework | guidance | onboarding | ✅ Balfour (Four Fits; diagnostic) |
| [act-design-social-proof-beyond-paywall](units/act-design-social-proof-beyond-paywall.md) | case-study | social-proof | signup | ⚠ ethics; metrics = whole redesign (ASL Bloom) |
| [act-design-welcome-survey-tailors-flow](units/act-design-welcome-survey-tailors-flow.md) | case-study | personalization | onboarding | ⚠ bundled (Kontentino +~10% activation) |
| [act-benchmark-time-to-value-saas](units/act-benchmark-time-to-value-saas.md) | benchmark | friction-reduction | aha | ✅ Pendo×MTP first-party (6,800+ apps) |

**Tactic-family coverage:** friction-reduction ✓✓✓✓✓✓, motivation ✓✓✓✓, guidance ✓✓✓✓✓✓✓✓, personalization ✓✓✓✓, social-proof ✓✓✓, incentive ✓✓✓✓ · **fully robust: all six families at ≥3.**
**Unit-type coverage:** principle ✓✓✓✓✓✓, tactic ✓✓✓✓✓, benchmark ✓✓✓✓✓✓✓✓, case-study ✓✓✓✓✓✓✓, framework ✓✓✓ · good spread.
**Persuasion-adjacent units** (carry mandatory `Caution (ethics):`): social-proof ×3, endowed-progress, uncertain-rewards.
**Flagship benchmarks:** two independent first-party datasets now agree on TTV — Userpilot (547 cos, ~1d12h) + Pendo×MTP (6,800+ apps, avg 1.5 days); activation_rate ~37.5%, checklist completion ~19%; by-industry spread incl. FinTech 5% (bank/wallet prior for P7).
**Causal-honesty discipline is visible** across the corpus: correlational (video), bundled-redesign (ASL Bloom, Kontentino), and second-hand (Chameleon-cited, Verna) findings are all explicitly flagged, never presented as proven causation.
**Still available (in hand, not drafted):** more Userpilot cases (Sked 3× checklist; Platformly >40%); deeper MTP + Userpilot segments (retention/NPS/feature-adoption by industry+size).
