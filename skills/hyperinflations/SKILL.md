---
name: hyperinflations
description: Assess whether an inflationary depression or inflationary deleveraging is spiraling into hyperinflation. Use when asked about hyperinflation risk, extreme currency collapse, money printing, wage-price spirals, loss of money's store-of-value or medium-of-exchange role, Weimar-style or Venezuela-style crises, or whether policymakers can still stop printing and stabilize the currency.
---

# Hyperinflations

## Overview

Use this skill to judge whether an inflationary deleveraging has moved from a severe currency crisis into hyperinflation risk or actual hyperinflation. Hyperinflation here means extreme inflation, roughly goods and services prices more than doubling every year or worse, combined with severe wealth destruction and economic hardship.

## Workflow

1. Identify the country, period, currency regime, debt structure, and whether the user asks about current risk, historical staging, policy failure, or investment/asset behavior.
2. Load `references/hyperinflation-spiral-rubric.md` for the trigger conditions, stages, scoring, and output template.
3. Load `references/official-data-sources.md` to gather official or official-sector data.
4. Determine whether the country is already in an inflationary deleveraging. If not, classify the preconditions before judging hyperinflation.
5. Score the hyperinflation escalation matrix:
   - External imbalance not closing.
   - External spending/debt service funded by repeated money printing.
   - Currency depreciation and capital flight reinforcing each other.
   - Inflation psychology and wage/price indexation spreading.
   - Money printing losing growth impact as funds move to real/foreign assets.
   - Maturities shortening and the banking system becoming illiquid.
   - Money losing store-of-value, unit-of-account, or medium-of-exchange functions.
6. Classify the country as `no hyperinflation risk`, `watchlist`, `high risk`, `spiraling`, or `hyperinflation`.
7. Explain the causal chain, policy choices, and what would stop or worsen the spiral.

## Output Shape

```text
Country/period: <country, dates>
Classification: No hyperinflation risk | Watchlist | High risk | Spiraling | Hyperinflation | Insufficient data
Confidence: High | Medium | Low

Trigger matrix:
External imbalance not closing: <yes/mixed/no/unknown> - <evidence>
Money printing funds external spending/debt service: <yes/mixed/no/unknown> - <evidence>
Depreciation-capital-flight spiral: <yes/mixed/no/unknown> - <evidence>
Inflation psychology/wage-price spiral: <yes/mixed/no/unknown> - <evidence>
Printed money fleeing to real/foreign assets: <yes/mixed/no/unknown> - <evidence>
Maturities shorten and liquidity breaks: <yes/mixed/no/unknown> - <evidence>
Money functions breaking down: <yes/mixed/no/unknown> - <evidence>

Spiral stage: Currency crisis | Inflationary depression | Hyperinflation risk | Hyperinflation | Currency replacement/repair
Policy read-through: <why printing is continuing or stopping>
Asset behavior: <currency, bonds, equities, gold/commodities, foreign assets>
What would stop the spiral: <hard backing/new currency/fiscal-external adjustment/default/restructuring>
What would worsen it: <continued monetization, capital flight, indexation, disorderly defaults>
Official data used: <sources, series, dates>
Data caveats: <missing/stale/non-comparable data>
```

## Guardrails

- Do not call ordinary high inflation hyperinflation unless inflation, currency, money, and behavioral evidence support the call.
- Do not infer hyperinflation from money growth alone. The key is the interaction of external imbalance, monetization, currency collapse, inflation psychology, and money-function breakdown.
- For current assessments, verify live official data because inflation, exchange rates, reserves, and policy actions can change quickly.
- Distinguish local-currency asset gains from real or hard-currency wealth preservation.
- Do not present investment observations as personalized financial advice.
