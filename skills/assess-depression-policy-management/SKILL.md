---
name: assess-depression-policy-management
description: Assess whether policymakers are managing a debt-cycle bubble, top, depression, or beautiful deleveraging well or poorly. Use when asked to judge government or central bank crisis management, depression management, deleveraging policy quality, policy mistakes, fiscal/monetary response, macroprudential response, bank protection, monetization, austerity, or whether policy is moving toward a beautiful or ugly deleveraging.
---

# Assess Depression Policy Management

## Overview

Use this skill to judge whether policymakers are handling a debt-cycle downturn well or poorly. The assessment should cover the phase-specific policy choices before the bust, at the top, during the depression, and during the reflationary or beautiful-deleveraging phase.

## Workflow

1. Load `references/policy-management-rubric.md`.
2. Identify the country, policy window, debt-cycle phase, and whether the user is asking about government, central bank, regulators, or the combined policy mix.
3. Gather evidence on:
   - Monetary policy, short rates, liquidity provision, asset purchases, monetization, and currency policy.
   - Fiscal policy, austerity, stimulus, transfers, guarantees, and fiscal sustainability.
   - Macroprudential policy, credit restraints, lending standards, capital requirements, and targeted easing/tightening.
   - Treatment of systemically important institutions, banks, shadow banks, depositors, and non-systemic failures.
   - Asset markets, credit growth, debt burdens, nominal growth, inflation, unemployment, and financial stress.
4. Score each relevant phase as `well managed`, `mixed`, `poorly managed`, or `unknown`.
5. Decide whether the overall policy mix is moving toward a beautiful deleveraging, an ugly deflationary depression, or an ugly inflationary depression.
6. State the policy mistakes, best policy moves, missing data, and what would improve or worsen the score.

## Output Template

```text
Policy management: Well managed | Mixed | Poorly managed | Insufficient data
Country/period: <country, dates>
Cycle phase assessed: Bubble | Top | Depression | Beautiful deleveraging | Multi-phase

Bubble management: <score, if applicable> - <evidence>
Top management: <score, if applicable> - <evidence>
Depression management: <score, if applicable> - <evidence>
Beautiful-deleveraging management: <score, if applicable> - <evidence>

Policy mix read-through: <plain-language synthesis>
Main policy mistake or strength: <evidence>
Risk path: Beautiful deleveraging | Ugly deflationary depression | Ugly inflationary depression | Unclear
What would improve the score: <policy/data>
What would worsen the score: <policy/data>
Data caveats: <missing/stale/non-comparable series>
```

## Guardrails

- Do not judge policy only by outcomes. Separate decisions that were knowable at the time from later data.
- Do not treat austerity, monetization, bank protection, or currency depreciation as automatically good or bad. Judge balance, timing, scale, and targeting.
- For current analysis, verify policy actions and macro data because rates, balance sheets, fiscal packages, and bank interventions change quickly.
- Distinguish systemically important institutions from non-systemic entities; good management often protects the former while allowing orderly failure of the latter.
- Do not present the policy assessment as financial advice.
