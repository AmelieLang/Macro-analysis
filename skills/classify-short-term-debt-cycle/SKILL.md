---
name: classify-short-term-debt-cycle
description: "Classify a country or period into the archetypical short-term debt cycle phases. Use when asked to assess early recovery, mid-cycle, late cycle, late boom/early recession, early recession, or late recession using growth versus potential, GDP gap, inflation, unemployment, short rates, yield curve, private debt/GDP, housing, durables consumption, capacity utilization, real equities, commodities, bonds, and policy stance."
---

# Classify Short-Term Debt Cycle

## Overview

Use this skill to classify where a country-period sits in the archetypical short-term debt cycle. The cycle is driven by central bank easing and tightening, credit growth, slack, inflation pressure, debt service, and the response of asset classes.

## Workflow

1. Load `references/short-term-cycle-rubric.md`.
2. Identify the country, exact period, frequency, and whether the user wants a current snapshot, historical diagnosis, or monitoring dashboard.
3. Gather the core indicators:
   - Real growth versus potential growth and GDP gap.
   - Inflation.
   - Unemployment.
   - Short-term policy rate and yield curve.
   - Private debt/GDP and credit growth.
   - Housing and durables consumption.
   - Capacity utilization.
   - Real equity prices or total returns.
   - Bonds, commodities, and inflation-hedge assets where available.
4. Score the evidence against each phase signature.
5. Assign a primary phase, confidence, and adjacent phase risk.
6. Explain the policy stance and the expected asset-class pattern.
7. List what would confirm a move to the next phase or invalidate the call.

## Phase Labels

Use these labels:

- `Early recovery`: economy emerges from recession; slack is high; inflation is low or falling; rates are low/easing; credit, housing, durables, retail sales, and equities begin to recover.
- `Mid-cycle`: growth is steady and near expectations; slack remains; inflation is low/stable; rates are not tightening materially; equity gains moderate.
- `Late cycle`: above-potential growth consumes slack; inflation, wages, capacity utilization, investment, profits, commodities, and inflation hedges rise; rates and bond yields rise.
- `Late boom/early recession`: central bank tightens aggressively; short rates rise relative to long rates; curve flattens/inverts; liquidity falls; equities and long-duration assets sell off.
- `Early recession`: central bank stays tight while activity deteriorates; spending, credit, investment, equities, commodities, and employment fall; inflation has not yet fully cooled.
- `Late recession`: inflation finally subsides; central bank cuts aggressively; equities bottom before the economy; housing/durables and borrowing begin to stabilize.
- `Mixed/transition`: evidence spans adjacent phases.
- `Insufficient data`: core growth, inflation, labor, rates, curve, and market data are missing.

## Output Template

```text
Short-term debt cycle phase: <phase>
Confidence: High | Medium | Low
Country/period: <country, dates>

Growth vs potential/GDP gap: <evidence>
Inflation/slack/labor: <evidence>
Policy rates/yield curve: <evidence>
Credit/private debt/housing/durables: <evidence>
Capacity/investment/activity: <evidence>
Markets: <equities/bonds/commodities/inflation hedges evidence>

Why this phase: <plain-language synthesis>
Adjacent phase risk: <prior/next phase evidence>
What would confirm next phase: <data/events>
What would invalidate: <data/events>
Data caveats: <missing/stale/non-comparable series>
```

## Guardrails

- Do not classify from one chart. Use the full pattern across growth, slack, inflation, rates, credit, and assets.
- Distinguish short-term debt cycles from long-term debt cycles. Use `stage-debt-cycle` for long-term debt-cycle staging.
- For current analysis, verify live data because rates, labor, inflation, markets, and policy expectations change quickly.
- Compare indicators to the country's own history and institutional structure.
- Do not present the phase call as financial advice.
