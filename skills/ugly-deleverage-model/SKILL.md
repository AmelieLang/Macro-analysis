---
name: ugly-deleverage-model
description: Diagnose ugly deleveraging risk and policy mistakes using the Japan 1984-1994 template. Use when asked why a country failed to ease enough after a debt/asset bubble, whether policy is too tight during a deleveraging, how fiscal/monetary/currency policy interact with deflationary forces, whether currency conditions create inflationary-depression risk, whether an inflationary deleveraging is being managed beautifully or poorly, or which economic indicators are leading versus lagging in an ugly deleveraging.
---

# Ugly Deleverage Model

## Overview

Use this skill to assess whether a country is moving from bubble/top into an ugly deleveraging because policy easing is too late, too small, or too narrowly focused to offset debt deflation. The core template is Japan from 1984 to 1994.

## Workflow

1. Identify the country, period, and cycle phase: bubble build-up, top/still-tightening, free fall, or later repair.
2. Load `references/japan-1984-1994-case-study.md` when the user asks for the Japan template or for a comparison to Japan.
3. Load `references/Inflationary deleveraging in non-reserve currency economies.md` when the user asks about Korea, Asian Financial Crisis dynamics, balance-of-payments crises, foreign-currency debt, reserve drains, currency defense, whether the country has bottomed, whether policy is doing well, or inflationary deleveraging in non-reserve-currency economies.
4. Load `references/ugly-deleverage-rubric.md` for the policy-pillar framework, leading/lagging indicators, and output template.
5. Load `references/official-data-sources.md` to gather or verify current/historical data from official sources.
6. Split the assessment into three windows:
   - `Pre-top/bubble`: the boom and tightening phase.
   - `Top/still-tightening`: asset prices and forward indicators break while policy remains tight or eases only modestly.
   - `Free fall with easing`: policy rates fall, but income, asset prices, credit, and confidence keep deteriorating.
7. Assess three policy pillars in each window:
   - Fiscal: stance, automatic stabilizers, stimulus, austerity, bank support, and balance-sheet repair.
   - Monetary: short rates, real rates, yield curve, liquidity, money/base money, credit transmission, and lender support.
   - Currency: exchange-rate pressure, reserve flows, current account, intervention, reserve-currency status, FX reserves, foreign-currency debt, external financing gaps, real rates, inflation credibility, and whether currency strength/weakness helps or hurts reflation.
8. Separate leading indicators from lagging indicators before judging policy mistakes.
9. Return the matrix first, then explain the policy error, lagging-indicator trap, and ugly-deleveraging mechanism.

## Output Shape

Use this structure:

```text
Country/period: <country, years>
Regime: Ugly deleveraging | Ugly-deleveraging risk | Mixed/transition | Not ugly deleveraging | Insufficient data
Core error: <late easing, modest easing, fiscal drag, currency squeeze, bank/credit impairment, or other>
Confidence: High | Medium | Low

Period 1 - Pre-top/bubble:
Fiscal: <stance and evidence>
Monetary: <stance and evidence>
Currency: <stance and evidence>
Economic indicators: <growth, output gap, inflation, industrial production, unemployment, debt, asset prices, P/E, credit>
Read-through: <why the economy looked strong or vulnerable>

Period 2 - Top/still-tightening:
Fiscal: <stance and evidence>
Monetary: <stance and evidence>
Currency: <stance and evidence>
Economic indicators: <what broke first, what still looked okay>
Read-through: <policy mistake and lagging-indicator trap>

Period 3 - Free fall with easing:
Fiscal: <stance and evidence>
Monetary: <stance and evidence>
Currency: <stance and evidence>
Economic indicators: <debt deflation and policy transmission>
Read-through: <why easing did not stop the fall>

Leading warning indicators: <asset prices, valuations, yield curve, credit, debt service, IP, currency/reserves, etc.>
Lagging indicators that fooled policymakers: <unemployment, inflation, output gap, GDP, fiscal balance, etc.>
Currency/inflationary-depression vulnerability: <reserve currency, reserves, FX debt, fiscal/trade deficits, real rates, inflation history>
Ugly-deleveraging mechanism: <plain-language causal chain>
What would have improved the outcome: <policy counterfactual>
Data caveats: <missing/stale/non-comparable series>
```

## Guardrails

- Do not judge policy only with hindsight. State which warning signals were visible at the time.
- Do not rely on unemployment, inflation, or fiscal balance alone; these can lag badly at the top.
- Do not call a deleveraging "beautiful" just because rates are falling. Easing must be large enough to restore nominal income growth, credit transmission, and balance-sheet repair.
- For current country analysis, verify live official data before answering.
- Do not present the analysis as financial advice.
