---
id: mon-principle-value-metric
stage: monetization
sub_stage: pricing-model
business_model: plg-saas
tactic_family: pricing-model
unit_type: principle
metric: [paying_conversion, arpu, weekly_revenue]
provenance: public
sources:
  - "Kyle Poyar (OpenView), summarized by Reforge (2019), from OpenView's SaaS pricing assessment of 1,800 companies."
---
**Principle — charge on the value metric: the unit that scales with the value the customer gets.**

The most important pricing decision is *what* you charge for, not how much. The **value metric** is the
unit a customer is billed on — it should rise as the customer gets more value (e.g. API calls for
Twilio, videos for Wistia, contacts for an email tool), so the bill grows with success rather than
feeling like a tax. Evidence distilled from Poyar's OpenView work (1,800-company assessment): only
**4%** of companies scored "excellent" at pricing and **44%** failed, and choosing the wrong value
metric is a leading cause; companies whose metric tracks value are far more likely to say their pricing
aligns with value.

**How to apply.** Find the one unit that best tracks the value this product delivers, and align the
price to it. Test it against three questions: does it grow as the customer gets more value, is it easy
for the customer to understand and predict, and does it let a small customer start cheap. Fix the value
metric before arguing about the price points.

**When it applies.** Any pricing design or re-pricing; especially PLG where the buyer self-serves and
the metric must be legible.

**Caution (honesty).** A value metric the customer can't predict or control (a bill that spikes
unexpectedly) breaks trust even when it "scales" — pair it with visibility and caps. Don't pick a
metric just because it maximises extraction; it has to track value the customer agrees they got. Pairs
with [[mon-principle-usage-vs-seat]] and [[mon-tactic-model-choice]].
