---
id: acq-framework-channel-model-fit
stage: acquisition
sub_stage: channel-strategy
business_model: plg-saas
tactic_family: channel-strategy
unit_type: framework
metric: [new_signups, unique_visitors]
provenance: public
sources:
  - "Brian Balfour (Reforge), 'Channel Model Fit for User Acquisition' — one of the Four Fits essays (brianbalfour.com/essays/channel-model-fit-for-user-acquisition, 2017)."
---
**Framework — your business model decides which channels can work: match the channel's cost to your ARPU.**

Channels are determined by the model, and the model by the channels — they are not chosen
independently. Plot a product on an **ARPU ↔ CAC spectrum** (Balfour uses *annual* revenue per user,
because a startup usually needs payback under a year): higher ARPU can fund higher-cost channels,
lower ARPU restricts you to cheap, low-friction ones. The rough tiers Balfour maps:

- **Low ARPU, ads-supported** (Facebook, WhatsApp, Yelp) → virality, user-generated-content SEO.
- **Low-to-mid, transactional / self-serve subscription** (Dollar Shave Club, Slack, SurveyMonkey) →
  paid marketing, viral.
- **Mid, B2B** (HubSpot, Zendesk) → content marketing, inbound / inside sales, partnerships.
- **High, six-to-seven-figure deals** (Palantir, Veeva) → enterprise / outbound sales.

**How to apply.** Before testing channels, locate the product on the spectrum. A channel only fits if
your ARPU can cover its floor cost-per-acquisition. The trap is the **danger zone** in the middle:
ARPU too high for cheap channels (price adds friction that kills virality and content) yet too low to
fund high-CAC sales. Products survive there, but usually on a patchwork of channels and slower growth —
and survivorship bias hides how many don't. If you land in the danger zone, the fix is usually to
change the *model* (raise ARPU, cut friction), not to try harder on a channel that can't pay back.

**When it applies.** Any channel-strategy decision, early channel selection, or a "why isn't this
channel working" diagnosis — check model fit before blaming execution.

**Caution (honesty).** CAC and payback have **no canonical spec id** in `spec/metric-spec.yaml` — flag
the client's own definition rather than inventing one. The tier→channel map is a prior, not a law;
real products straddle tiers. Pairs with [[acq-framework-bullseye-channel-concentration]] (which of
the fitting channels to concentrate on) and [[acq-principle-channel-saturation]] (a fitting channel
still decays).
