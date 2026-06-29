---
name: monitor-deleveraging
description: Monitor and assess macro deleveraging monetization signals. Use when asked to detect, monitor, build dashboards for, write checks for, or analyze whether a deleveraging is underway using the combined pattern of large fiscal deficits, short-term interest rates pinned near zero or falling into a hard-landing regime, and monetary base/M0 expansion relative to nominal GDP.
---

# Monitor Deleveraging

## Overview

Use this skill to evaluate whether a macro environment is entering or in a deleveraging monetization regime. Treat the signal as a conjunction: do not call a deleveraging unless fiscal deficits, short-term rates, and money creation all confirm together.

## Workflow

1. Load the detailed signal definitions in `references/signal-framework.md`.
2. Identify the country, currency area, dates, and data frequency before scoring.
3. Gather or request the minimum data series:
   - Fiscal balance or deficit as a percent of nominal GDP.
   - Short-term policy rate or comparable short-term money-market rate.
   - M0, monetary base, reserve money, or closest high-powered-money proxy.
   - Nominal GDP for scaling money changes.
4. Normalize each series to the same reporting window. Use year-over-year changes for M0/monetary base scaled by nominal GDP unless the user specifies another convention.
5. Score each pillar independently, then combine them with the three-signal rule.
6. Report the current state, evidence, missing data, and invalidation conditions. Avoid making trade recommendations unless the user asks for a strategy.

## Decision Rule

Classify the regime as:

- `Confirmed deleveraging monetization`: all three core signals are active or two are active and the third is clearly moving into confirmation with no contradictory evidence.
- `Watch`: one or two signals are active, but the full conjunction is absent.
- `Not confirmed`: fewer than two signals are active, or one pillar directly contradicts the thesis.
- `Insufficient data`: the available data cannot fairly score at least two pillars.

Do not overfit to one chart or one crisis. The distinctive pattern is the simultaneous presence of deficit pressure, exhausted rate cuts, and money creation.

## Reporting Template

Use a concise structure:

```text
Regime: Confirmed deleveraging monetization | Watch | Not confirmed | Insufficient data
Window assessed: <dates/frequency>

Fiscal deficit: <active/watch/inactive> - <evidence>
Short-term rates: <active/watch/inactive> - <evidence>
M0/base money monetization: <active/watch/inactive> - <evidence>

Read-through: <plain-language interpretation>
What would confirm next: <data/events>
What would invalidate: <data/events>
Data caveats: <missing/stale/non-comparable series>
```

## Guardrails

- Separate deleveraging monetization from ordinary recessions, normal rate-cutting cycles, and routine deficit spending.
- Be explicit about data source timing and revisions when using live data.
- For current-market analysis, browse or use reliable data tools because macro data, rates, and policy actions change over time.
- Treat thresholds as heuristic, not mechanical. Explain judgment calls.
- Do not present this framework as financial advice.
