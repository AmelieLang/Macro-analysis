---
name: assess-macro-conditions
description: "Assess a country's economic and market conditions using a macro dashboard. Use when asked to evaluate country conditions, macro regime, cyclical momentum, overheating, recession risk, external balance, debt pressure, currency conditions, bond returns, equity returns, valuation, or policy stance using indicators such as real growth, potential growth, inflation, industrial production, unemployment, output gap, rates, yield curve, debt, FX, reserves, current account, fiscal balance, currency index, bonds, equities, and P/E."
---

# Assess Macro Conditions

## Overview

Use this skill to assess a country's economic and market conditions from a broad macro dashboard. The goal is to synthesize growth, inflation, labor, policy rates, debt, external balances, fiscal stance, currency behavior, and asset-market pricing into a coherent regime call.

## Workflow

1. Load `references/macro-dashboard-rubric.md`.
2. Identify the country, date range, data frequency, and whether the user wants a current snapshot, historical diagnosis, comparison, or monitoring dashboard.
3. Gather the dashboard indicators where available:
   - Real growth and potential growth.
   - Inflation.
   - Industrial production.
   - Unemployment rate.
   - Output gap.
   - Short rate and long rate.
   - Yield curve.
   - Net domestic debt as percent of GDP, preferably 12-month moving average.
   - Real FX versus trade-weighted index.
   - Reserve flow as percent of GDP.
   - Current account as percent of GDP.
   - Fiscal balance as percent of GDP.
   - Currency index.
   - Bond total returns.
   - Equity total returns.
   - P/E ratio on actual earnings.
4. Score each pillar as `supportive`, `neutral`, `stressed`, or `unknown`.
5. Combine the pillar scores into a macro regime and market-condition assessment.
6. State the main tail risk, strongest support, missing data, and what would change the assessment.

## Regime Labels

Use these labels when useful:

- `Goldilocks expansion`: growth above potential or improving, inflation contained, unemployment falling, output gap not dangerously positive, curves/rates not restrictive, debt/external/fiscal conditions stable, and asset returns supported by fundamentals.
- `Overheating late cycle`: growth and industrial production strong, output gap positive, unemployment low, inflation rising, rates rising, yield curve flattening, debt or asset valuations stretched.
- `Disinflationary slowdown`: growth and industrial production weaken, inflation falls, unemployment rises, output gap opens, curve steepens or policy eases, and risky assets weaken.
- `Debt/financial stress`: debt burdens rise, yield curve inverts or rates are restrictive, FX/reserves/current account weaken, credit-sensitive markets fall, and valuation or leverage risk is high.
- `External pressure`: real FX weakens, reserves flow out, current account deteriorates, currency index falls, and policy faces a growth-versus-currency tradeoff.
- `Reflation/recovery`: growth and industrial production recover, inflation normalizes from low levels, output gap closes, unemployment improves, policy is supportive, reserves/current account stabilize, and asset returns recover.
- `Mixed/transition`: indicators conflict or the country is moving between regimes.
- `Insufficient data`: too many core indicators are missing.

## Output Template

```text
Macro regime: <label>
Country/period: <country, dates>
Confidence: High | Medium | Low

Growth/activity: <supportive/neutral/stressed/unknown> - <evidence>
Inflation/labor/slack: <supportive/neutral/stressed/unknown> - <evidence>
Rates/yield curve: <supportive/neutral/stressed/unknown> - <evidence>
Debt/fiscal: <supportive/neutral/stressed/unknown> - <evidence>
External/FX/reserves: <supportive/neutral/stressed/unknown> - <evidence>
Markets/valuation: <supportive/neutral/stressed/unknown> - <evidence>

Read-through: <plain-language synthesis>
Main risk: <risk>
Strongest support: <support>
What would improve: <data/events>
What would worsen: <data/events>
Data caveats: <missing/stale/non-comparable series>
```

## Guardrails

- Do not classify from one indicator. Use the dashboard pattern and the direction of change.
- Compare each indicator to the country's own history and structure; thresholds differ across developed markets, emerging markets, commodity exporters, and reserve-currency economies.
- For current analysis, verify live or recent data because rates, FX, reserves, markets, and policy can change quickly.
- Distinguish nominal strength from real strength, and asset-price gains from sustainable fundamentals.
- Do not present the assessment as financial advice.
