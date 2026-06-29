# Deleveraging Monetization Signal Framework

## Core Premise

A deleveraging monetization regime is identified by three conditions occurring together:

1. Large fiscal deficits or rapidly deteriorating fiscal balances.
2. Short-term interest rates at or near the lower bound, or falling sharply in a hard-landing response.
3. Expansion in M0, monetary base, or reserve money relative to nominal GDP.

The combination matters more than any single input. Each condition can happen outside deleveragings; the conjunction is the distinctive signal.

## Signal 1: Fiscal Deficit Pressure

Preferred measure: government fiscal balance as percent of nominal GDP, with deficits shown as negative values or absolute deficit share.

Active:
- Deficit is deeply negative, typically worse than -5% of GDP for peacetime developed markets, or materially worse than the country's own recent norm.
- Deficit deteriorates quickly during recession, crisis, war, banking stress, or private-sector balance-sheet repair.
- Authorities use fiscal transfers, guarantees, bailouts, or stimulus large enough to change debt dynamics.

Watch:
- Deficit is widening but not yet extreme.
- Political or crisis conditions point toward materially larger issuance.
- Off-balance-sheet guarantees or quasi-fiscal support are large but not fully visible in headline deficit data.

Inactive:
- Fiscal balance is stable, improving, or small relative to GDP.
- Deficit widening is modest and financed without pressure on rates or money creation.

Notes:
- Wartime deficits are a special case; flag them separately because they can dominate the signal.
- Use general government data where available; central government data can understate the impulse.

## Signal 2: Short-Term Rates Pinned or Hard-Landing Cuts

Preferred measure: policy rate, overnight rate, 3-month Treasury bill, SOFR-equivalent, or closest money-market rate.

Active:
- Short-term rates are near zero or the effective lower bound.
- Rates have been cut rapidly toward zero in response to recession, banking stress, or asset deflation.
- The central bank has little conventional easing room left.

Watch:
- Rates are falling quickly but are not yet near the lower bound.
- Forward guidance, market pricing, or central bank communication implies aggressive cuts.
- Real rates are collapsing even if nominal rates remain above zero.

Inactive:
- Short-term rates are high or rising because policy is tightening.
- The central bank has ample conventional room and is not easing into crisis.

Notes:
- Use country-specific lower bounds. Some jurisdictions can operate slightly below zero.
- In high-inflation emerging markets, "near zero" may be less useful; focus on real rates, loss of market access, and central bank financing.

## Signal 3: M0/Base Money Monetization

Preferred measure: year-over-year change in M0, monetary base, or reserve money as a percent of nominal GDP:

```text
monetization_impulse = (M0_t - M0_t_minus_1_year) / nominal_GDP_t
```

Active:
- M0/base money is expanding sharply relative to GDP.
- The change is clearly above the prior-cycle norm, often several percentage points of GDP in developed markets.
- Expansion is linked to asset purchases, reserve creation, lending facilities, yield control, or direct/indirect fiscal financing.

Watch:
- M0/base money has turned up from a long flat period.
- Central bank balance sheet expansion is announced but not yet visible in M0/base money.
- Reserves are rising while broader money or credit remains weak.

Inactive:
- M0/base money is flat or contracting relative to GDP.
- Central bank actions sterilize liquidity or do not create durable base money.

Notes:
- Monetary aggregates differ by country. Prefer the narrowest high-powered-money measure available.
- If M0 is unavailable, use central bank liabilities, reserve money, or balance sheet assets as a proxy and label it clearly.

## Combining The Signals

Use this scoring rubric:

```text
active = 2
watch = 1
inactive = 0
unknown = null
```

Interpretation:
- 6 points with all three pillars active: confirmed.
- 5 points with no inactive pillar: confirmed but note the lagging pillar.
- 3-4 points: watch.
- 0-2 points: not confirmed unless data are missing.
- Any unknown pillar: reduce confidence and list the data needed.

Do not let a single extreme observation override an inactive pillar. The framework is designed to catch the cluster, not isolated stress.

## Common False Positives

- Ordinary recession: deficits widen and rates fall, but M0/base money does not expand materially.
- Routine quantitative easing: base money expands and rates are low, but fiscal deficits are not under stress.
- Fiscal stimulus in an expansion: deficits widen while rates are not pinned and money creation is absent.
- Banking liquidity operations: reserves rise temporarily while fiscal deficits and private deleveraging are not present.
- High-inflation tightening: deficits may be large, but short rates rise and liquidity is restrained.

## Useful Data Sources

Use official or reputable sources where possible:

- Central bank statistical releases for policy rates, M0, monetary base, reserves, and balance sheet data.
- Treasury or finance ministry releases for fiscal balance and issuance.
- National statistics agencies for nominal GDP.
- IMF, World Bank, OECD, FRED, BIS, or CEIC/Haver/Bloomberg when official series are hard to combine.

For live or recent assessments, verify current values and release dates. State the source and date because policy rates and central bank balance sheets can change quickly.

## Output Guidance

Be decisive but conditional. Good outputs say whether the three-part pattern is present, which pillar is weakest, and what data would change the call.

Use language like:
- "The deleveraging monetization pattern is confirmed for this window because all three pillars are active."
- "This is a watch, not a confirmation: deficits and rates line up, but base money has not expanded relative to GDP."
- "This looks like ordinary easing rather than deleveraging monetization because fiscal pressure is absent."
