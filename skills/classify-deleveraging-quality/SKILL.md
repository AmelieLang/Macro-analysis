---
name: classify-deleveraging-quality
description: "Classify whether an economy is experiencing a beautiful deleveraging or ugly deleveraging. Use when asked to monitor, compare, score, dashboard, or explain deleveraging quality using five indicators: nominal growth versus long rates, inflation, unemployment rate, real growth, and government balance."
---

# Classify Deleveraging Quality

## Overview

Use this skill to judge the quality of a deleveraging after deleveraging pressure has been identified. The central question is whether debt burdens are being reduced with acceptable growth and inflation dynamics, or through a disorderly contraction and worsening fiscal stress.

## Workflow

1. Load `references/five-indicator-rubric.md`.
2. Identify the economy, time window, data frequency, and whether the user wants a current reading, historical comparison, or dashboard logic.
3. Gather the five required panels:
   - Nominal growth versus long-term interest rate.
   - Inflation.
   - Unemployment rate.
   - Real growth.
   - Government balance.
4. Normalize each series to the same window and label release dates when using live data.
5. Score every indicator as `beautiful`, `mixed`, `ugly`, or `unknown`.
6. Combine the scores into a regime call and explain the weakest pillar.

## Classification

Classify as:

- `Beautiful deleveraging`: debt burdens can fall because nominal growth is above or near long rates, inflation is positive but controlled, unemployment is stable or falling, real growth is positive or recovering, and the government balance is stabilizing after support.
- `Ugly deleveraging`: nominal growth is below long rates, inflation is too low/deflationary or disorderly high, unemployment rises or stays high, real growth contracts or whipsaws, and the government balance deteriorates without stabilization.
- `Mixed or transition`: the five indicators do not agree, or the regime is moving from ugly toward beautiful or vice versa.
- `Insufficient data`: fewer than three indicators can be scored.

Use the five-indicator pattern, not one standout chart. A beautiful deleveraging is a balance: enough money and income growth to reduce debt burdens, without runaway inflation or persistent depression.

## Reporting Template

```text
Regime: Beautiful deleveraging | Ugly deleveraging | Mixed/transition | Insufficient data
Window assessed: <dates/frequency>

Nominal growth vs long rate: <beautiful/mixed/ugly/unknown> - <evidence>
Inflation: <beautiful/mixed/ugly/unknown> - <evidence>
Unemployment: <beautiful/mixed/ugly/unknown> - <evidence>
Real growth: <beautiful/mixed/ugly/unknown> - <evidence>
Government balance: <beautiful/mixed/ugly/unknown> - <evidence>

Read-through: <plain-language interpretation>
Main risk: <indicator most likely to turn the regime ugly>
What would improve the call: <data/events>
What would worsen the call: <data/events>
Data caveats: <missing/stale/non-comparable series>
```

## Guardrails

- Do not confuse this skill with detecting whether deleveraging exists. Use it to classify the quality of a deleveraging once debt stress or deleveraging pressure is already in scope.
- For current economic analysis, verify live data because rates, inflation, labor markets, growth, and fiscal balances change over time.
- Treat thresholds as heuristics and compare against the economy's own history.
- Distinguish nominal reflation from real recovery. Nominal growth can look good while real growth and unemployment remain ugly.
- Do not present the classification as financial advice.
