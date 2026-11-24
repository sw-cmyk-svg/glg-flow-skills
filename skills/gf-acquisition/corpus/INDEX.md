# Acquisition corpus — index

**Version:** 0.3.0 (waves 1–3 — 2026-11-19) · business_model: `plg-saas`
**Status:** drafting (I draft, founder vets). **18 units — all six families ≥3 (robust bar met).**
Same curation rules: authored distilled note + citation, I-draft-you-vet, verification-as-drafting,
persuasion-ethics principle.

**Curation principle — persuasion & ethics (inherited).** Persuasion tactics are allowed, but every
persuasion-adjacent unit MUST carry an explicit `Caution (ethics):` line. Acquisition's ethics edge is
**truthful marketing**: deceptive ads, fake scarcity / urgency, bait-and-switch value props,
undisclosed paid promotion, spam, and knowingly buying junk traffic are dark patterns — documented as
anti-patterns, never prescribed — and several breach advertising / consumer-protection law. Regulated
archetypes (bank/wallet, betting) get an advertising / financial-promotion / responsible-use
compliance caution, not a ban.

## Six tactic families (target ≥3 each)

1. **channel-strategy** — channel portfolio, channel-market / channel-model fit, concentration (find
   the one or two channels that work — Bullseye), growth loops vs funnels.
2. **targeting-positioning** — ICP / audience, message-market fit, positioning as the acquisition
   input (you can't out-spend weak positioning).
3. **acquisition-conversion** — landing pages, ad→page message match, value prop, the visitor→signup
   flow (owns `signup_rate`).
4. **paid-acquisition** — paid-channel economics: CAC, bids / budget / creative, and the LTV:CAC /
   payback discipline that says whether paid is sustainable.
5. **organic-content** — SEO, content marketing, owned / earned channels, compounding (loop) vs rented
   (paid) distinction.
6. **attribution-efficiency** — measuring acquisition honestly: attribution's limits, CAC / payback /
   LTV:CAC, cohort quality (qualified signups that activate, not vanity volume).

## Planned sourcing waves

- **Wave 1 — strategy spine (channel-strategy, targeting-positioning):** Four Fits / channel-model fit
  (Balfour), Bullseye / channel concentration (Traction), law of shitty clickthroughs / channel
  saturation (Andrew Chen), positioning as acquisition input (Dunford).
- **Wave 2 — surface + paid (acquisition-conversion, paid-acquisition):** message match / landing-page
  conversion + its benchmark (Unbounce/WordStream), visitor→signup friction, CAC / payback discipline,
  LTV:CAC rule-of-thumb benchmark (OpenView/Bessemer).
- **Wave 3 — organic + measurement (organic-content, attribution-efficiency):** content/SEO as a
  compounding loop, owned-vs-rented, attribution limits, cohort-quality (vanity volume vs qualified
  signups), k-factor as a measured channel (with the Referral seam).

| id | unit_type | tactic_family | sub_stage | verified |
|---|---|---|---|---|
| [acq-framework-channel-model-fit](units/acq-framework-channel-model-fit.md) | framework | channel-strategy | channel-strategy | ✅ Balfour, Channel Model Fit (primary essay) |
| [acq-framework-bullseye-channel-concentration](units/acq-framework-bullseye-channel-concentration.md) | framework | channel-strategy | channel-strategy | ✅ Traction (Weinberg & Mares) via Balfour's Bullseye essay; Thiel |
| [acq-principle-channel-saturation](units/acq-principle-channel-saturation.md) | principle | channel-strategy | channel-strategy | ✅ Andrew Chen, Law of Shitty Clickthroughs (primary; 78% HotWired 1994) |
| [acq-framework-positioning-dunford](units/acq-framework-positioning-dunford.md) | framework | targeting-positioning | targeting-positioning | ✅ Dunford, Obviously Awesome 2019 (5 components) |
| [acq-framework-beachhead-narrow-icp](units/acq-framework-beachhead-narrow-icp.md) | framework | targeting-positioning | targeting-positioning | ✅ Moore, Crossing the Chasm 1991 (beachhead/bowling-pin) |
| [acq-principle-message-market-fit](units/acq-principle-message-market-fit.md) | principle | targeting-positioning | targeting-positioning | ⚠ ethics; ✅ Schwartz 1966 (concept, not verbatim) + Dunford |
| [acq-tactic-message-match](units/acq-tactic-message-match.md) | tactic | acquisition-conversion | acquisition-conversion | ⚠ ethics (no bait-and-switch); ✅ CRO practice |
| [acq-benchmark-landing-page-conversion](units/acq-benchmark-landing-page-conversion.md) | benchmark | acquisition-conversion | acquisition-conversion | ✅✅ Unbounce 2024 — all 9 per-industry medians + SaaS channels VERIFIED at primary public pages (SaaS 3.8%, ecom 4.2%, entertainment 12.3%); NOT gated |
| [acq-tactic-reduce-signup-friction](units/acq-tactic-reduce-signup-friction.md) | tactic | acquisition-conversion | acquisition-conversion | ⚠ Activation seam + dark-pattern line; ✅ CRO practice |
| [acq-benchmark-cac-payback](units/acq-benchmark-cac-payback.md) | benchmark | paid-acquisition | paid-acquisition | ✅✅ CORRECTED — High Alpha 2024 p38 (payback by stage ~2/8/14/14/20mo) VERIFIED at primary; Benchmarkit = CAC *Ratio* $2.00, not payback-months |
| [acq-principle-ltv-cac-heuristic](units/acq-principle-ltv-cac-heuristic.md) | principle | paid-acquisition | paid-acquisition | ✅✅ Skok origin + High Alpha 2024 p33 (high-NRR grows 2.5x) VERIFIED at primary; payback+NRR > LTV:CAC |
| [acq-principle-paid-creative-and-scale-limits](units/acq-principle-paid-creative-and-scale-limits.md) | principle | paid-acquisition | paid-acquisition | ⚠ concept only (vendor CPA/ROAS figures NOT cited); ✅ 2024–25 practitioner consensus |
| [acq-principle-owned-vs-rented-channels](units/acq-principle-owned-vs-rented-channels.md) | principle | organic-content | organic-content | ✅ Balfour growth-loops + practice (concept) |
| [acq-principle-content-compounds](units/acq-principle-content-compounds.md) | principle | organic-content | organic-content | ⚠ HubSpot's own ~2016 study (10%→38%), concept only, not replicated |
| [acq-tactic-seo-search-intent](units/acq-tactic-seo-search-intent.md) | tactic | organic-content | organic-content | ⚠ black-hat anti-pattern line; ✅ established SEO practice |
| [acq-principle-attribution-limits](units/acq-principle-attribution-limits.md) | principle | attribution-efficiency | attribution-efficiency | ✅ measurement practice + privacy context (ATT/cookies); incrementality > models |
| [acq-benchmark-channel-conversion-varies](units/acq-benchmark-channel-conversion-varies.md) | benchmark | attribution-efficiency | attribution-efficiency | ✅✅ Unbounce 2024 SaaS channels VERIFIED at primary (email 16.9% → display 0.3%) |
| [acq-principle-cohort-quality-vs-vanity-volume](units/acq-principle-cohort-quality-vs-vanity-volume.md) | principle | attribution-efficiency | attribution-efficiency | ✅ PLG practice + Activation seam (quality > volume) |

**Tactic-family coverage (robust — all ≥3):** channel-strategy ✓✓✓, targeting-positioning ✓✓✓,
acquisition-conversion ✓✓✓, paid-acquisition ✓✓✓, organic-content ✓✓✓, attribution-efficiency ✓✓✓.

**Wave-2 verification notes (per founder's standing ask — recent data only for figures).** Benchmarks
refreshed to current sources; **old rules of thumb were corrected, not carried over**: landing-page
conversion anchored to **Unbounce's 2024 Conversion Benchmark Report** (overall median **6.6%**, SaaS
lowest at **~3.8%**, e-comm ~4.2%, finance ~8.3%, entertainment ~12.3%; data mid-2023→mid-2024) — this
replaced the planning-doc's vague "~2–6%". CAC payback anchored to **Benchmarkit's 2025 report** —
**2024 median ~18 months** (up from ~14 in 2023), ~16 in 2025, ~11mo sub-$5K to ~22mo $50K–$100K ACV;
the old "<12 months median" prior was **wrong** (<12mo is "good", not typical). LTV:CAC 3:1 is kept
only as a **concept/first-screen** (Skok's origin, from *mature public* companies) with the modern
correction that **CAC payback + NRR predict profitable growth better** (Poyar). The paid-creative /
marginal-CAC unit is **concept-level only** — the circulating "$30→$40 CPA" / "2× spend → 20–30% ROAS
drop" figures are vendor-anecdotal and were **deliberately not cited**. Benchmark figures reached via
secondary summaries of the primary reports (primary PDFs not opened) — flagged in-unit to verify before
quoting to a client. Nothing fabricated.

**Primary verification pass (2026-11-19, founder supplied the reports + Unbounce via browser).** The
secondary figures were checked against the primaries, and two were CORRECTED:
- **CAC payback** — the widely-cited "~18-month median (Benchmarkit)" is **wrong as attributed**.
  Benchmarkit's 2025 deck reports a **New Customer CAC *Ratio*** (median **$2.00** of S&M per $1 new
  ARR, CY-24; blended $1.40) — a ratio, **not** payback-in-months. The real payback-in-months
  benchmark is **High Alpha 2024, p.38**: median is **stage-dependent** — ~**2mo** (<$1M, flagged as
  understated), **8mo** ($1–5M), **14mo** ($5–50M), **20mo** (>$50M). Unit rewritten to the primary;
  the "<12mo = healthy" rule reframed as early/mid-stage only. (High Alpha also: "CAC Payback Increases
  as Companies Mature… as Sales Channels Become Saturated" — corroborates channel-saturation.)
- **Landing-page conversion** — fully VERIFIED at primary; the per-industry detail turned out **not to
  be gated** (correcting an earlier assumption). All nine industry medians read from Unbounce's public
  per-industry pages: SaaS **3.8%** (lowest), ecommerce 4.2%, travel 4.8%, professional services 6.1%,
  legal 6.3%, healthcare 8.2%, finance 8.3%, education 8.4%, entertainment **12.3%** (highest), all-ind
  **6.6%**. SaaS channel splits also public (email 16.9% ≫ display 0.3%) — captured for wave-3
  attribution-efficiency. No email form was filled.
- **LTV:CAC** — the NRR-beats-LTV:CAC point is now primary-backed: **High Alpha 2024 p.33**, high-NRR
  (>106%) companies grow **~2.5× faster** than low-NRR (<98%); the unverified "~4x median" was removed.
- **Benchmarkit "Big Book of AI Metrics"** (July 2026, Rike & Buchanan) — an AI-metrics guide, not a
  source for these figures; not cited.
- NRR note for later: High Alpha / Benchmarkit put **median NRR ~100–105% (101%)**, slightly below the
  **~110%** the Monetization corpus cites from Poyar/Growth Unhinged 2024 — different datasets; worth a
  reconcile when Monetization is next touched.

**Wave-1 verification notes (per founder's standing ask):** Balfour's Channel-Model-Fit full essay,
his Bullseye essay, and Andrew Chen's Law of Shitty Clickthroughs were read at **primary source**
(brianbalfour.com / andrewchen.com) — the first-banner-ad CTR is **78% (HotWired 1994)** per Chen's
own post; a secondary site's **44%** figure conflicts with the primary and was **not** used.
*Traction* (19 channels + Bullseye) is grounded in the book via Balfour's primary summary. Dunford's
five components and Moore's beachhead are consistent across multiple summaries and attributed to the
books (2019 / 1991). Schwartz's "channel existing desire" is used as a **concept** (the exact wording
varies across secondary sites and the 1966 book was not read verbatim — no verbatim quote claimed).
Nothing fabricated to fill a gap.

**Wave-3 verification notes.** organic-content is deliberately **concept-grounded** (no shaky live
figures per the recency rule): owned-vs-rented leans on Balfour's growth-loops framing; content-compounds
uses HubSpot's own ~2016 "compounding posts" study (**10% of posts → 38% of traffic**) as a *concept*
only — HubSpot's data, not independently replicated, flagged in-unit; seo-search-intent is established
SEO practice with a black-hat anti-pattern line. attribution-efficiency: attribution-limits is standard
measurement practice plus the recent privacy context (Apple ATT 2021, cookie deprecation) with
incrementality as the stronger test; **channel-conversion-varies is primary-verified** — SaaS channel
medians read directly from Unbounce's public SaaS page (email **16.9%** → display **0.3%**);
cohort-quality-vs-vanity-volume is PLG practice on the Activation seam. **Corpus now robust (18 units,
all six families ≥3) — ready for the specialist anatomy (playbook + I/O contracts + assurance) and the
D-03 proof.**
