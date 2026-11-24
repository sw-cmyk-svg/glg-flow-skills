---
id: act-benchmark-activation-rate-saas-2025
stage: activation
sub_stage: aha
business_model: plg-saas
tactic_family: motivation
unit_type: benchmark
metric: [activation_rate, time_to_activation]
provenance: public
sources:
  - "Userpilot — SaaS Product Metrics Benchmark Report 2025 (first-party, 547 SaaS companies; activation from 62). Cross-ref: Lenny Rachitsky (~36% avg)."
---
**Benchmark — SaaS user activation rate & time-to-value (first-party, 2025).**

Userpilot's first-party data (547 companies; activation metrics from 62 B2B companies):
- **Activation rate: avg 37.5%, median 37%** — closely matching Lenny Rachitsky's reported
  **~36%**, so ~37% is a reasonable PLG-SaaS prior.
- **Time to value (activation): avg ≈ 1 day 12 hours.**
- **By industry (avg activation):** AI&ML **54.8%** (highest), CRM&Sales 42.6%, MarTech 24%,
  Healthcare 23.8%, HR 8.3%, **FinTech & Insurance 5%** (lowest).

**How to apply (Analyze/Benchmark).** Use ~37% as a starting reference for PLG-SaaS activation,
then adjust hard by vertical — a fintech product at 15% is *above* its peers, while a CRM at
30% is below. Always anchor to the client's own definition and funnel.

**When it applies.** Setting expectations and reading a client's activation number against peers.

**Caution.** **Definitions differ:** Userpilot "activation rate" = % of new users completing a
value-demonstrating action (no fixed window stated), vs the spec's `activation_rate` (event
*within 7 days* of signup); its TTV is an **average**, the spec's `time_to_activation` a
**median** — don't compare naively. Per-industry n is small (e.g. 58 AI&ML) and means/medians
diverge sharply (MarTech mean 24% vs median 7.9%), so treat vertical figures as directional. The
**FinTech 5%** figure is the relevant prior for the future bank/wallet archetype (P7). Pairs
with [[act-benchmark-activation-rates-by-percentile]] and [[act-framework-locate-the-problem]].
