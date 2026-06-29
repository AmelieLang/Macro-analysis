---
name: stage-debt-cycle
description: Classify a country and time period into long-term debt cycle stages. Use when asked to judge whether a country-period is in the early cycle, debt bubble, top, recession/depression, or reflationary deleveraging using debt burdens, debt service, income growth, asset prices, interest rates, credit conditions, inflation, unemployment, policy response, and the seven-question bubble scoreboard.
---

# Stage Debt Cycle

## Overview

Use this skill to locate a country-period within the long-term debt cycle. The stages are sequential but messy in real time: early cycle, debt bubble, top, recession/depression, and reflationary deleveraging.

## Workflow

1. Load `references/stage-rubric.md`.
2. Identify the country, exact time period, data frequency, and whether the user wants a historical or current assessment.
3. Gather or request the minimum evidence:
   - Total debt to GDP or debt to income.
   - Debt service as a percent of income or GDP.
   - Nominal income/GDP growth and real growth.
   - Credit growth, lending standards, leverage, and debt composition when available.
   - Asset prices, especially equities and real estate.
   - Short and long interest rates.
   - Inflation, unemployment, and external/currency stress.
   - Fiscal and monetary policy response.
4. Compare the country-period to the phase signatures in the rubric. Use changes and direction, not just levels.
5. If the evidence points to a debt bubble, late-cycle boom, or top, apply the seven-question bubble scoreboard in `references/stage-rubric.md`.
6. Assign a primary stage, confidence, and any adjacent-stage risk.
7. State what evidence would move the classification earlier or later in the cycle.

## Classification Labels

Use one of these labels:

- `Early cycle`: borrowing funds productivity-enhancing investment; incomes rise as fast as or faster than debt; debt burdens are stable; inflation and growth are balanced.
- `Debt bubble`: debt growth outstrips income growth; debt burdens and often debt service rise; asset prices and leverage boom; credit standards weaken.
- `Top`: asset bubble is bursting or vulnerable; rising rates, tighter liquidity, or a shock ends the up-wave; asset prices roll over while debt burdens remain high.
- `Depression` or `Recession/depression`: debt deflation becomes self-reinforcing; asset prices and incomes fall; interest-rate cuts are insufficient; defaults, unemployment, liquidity runs, and fiscal stress rise.
- `Reflationary deleveraging`: policy shifts to reflation; income growth returns above debt growth; activity rebounds while debt burdens and/or debt service begin to fall.
- `Mixed/transition`: evidence spans adjacent stages or timing is too narrow for a decisive call.
- `Insufficient data`: core debt, income, asset price, and policy evidence is missing.

## Reporting Template

```text
Stage: Early cycle | Debt bubble | Top | Depression/Recession | Reflationary deleveraging | Mixed/transition | Insufficient data
Confidence: High | Medium | Low
Country/period: <country, dates>

Debt burden/debt service: <evidence>
Income and growth: <evidence>
Asset prices and leverage: <evidence>
Bubble scoreboard: <score, if applicable>
Rates and credit conditions: <evidence>
Labor/inflation/external stress: <evidence>
Policy response: <evidence>

Why this stage: <plain-language synthesis>
Adjacent-stage risk: <previous/next stage evidence>
What would confirm: <data/events>
What would invalidate: <data/events>
Data caveats: <missing/stale/non-comparable series>
```

## Guardrails

- Do not classify from debt-to-GDP level alone. The cycle stage depends on the interaction among debt, income, debt service, asset prices, rates, and policy.
- For current country-periods, verify live data because policy rates, yields, asset prices, and macro releases change quickly.
- Distinguish long-term debt cycle stages from ordinary short-term business cycles.
- Treat the equity-market top as a useful anchor, not an automatic phase label for every country.
- Use local context: reserve-currency economies, emerging markets, pegged currencies, banking systems, and external debt structures can move through the cycle differently.
- Do not present the stage call as financial advice.
