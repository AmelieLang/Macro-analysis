# Five-Indicator Deleveraging Quality Rubric

## Core Premise

Classify deleveragings by the balance of five indicators:

1. Nominal growth versus long-term interest rate.
2. Inflation.
3. Unemployment rate.
4. Real growth.
5. Government balance.

A beautiful deleveraging reduces debt burdens without intolerable economic pain. An ugly deleveraging reduces debt through contraction, defaults, deflation, unemployment, fiscal deterioration, or unstable inflation.

## Indicator 1: Nominal Growth Versus Long Rate

Preferred measure:
- Nominal GDP growth or nominal income growth.
- Long-term government bond yield, usually 10-year yield.
- Spread: nominal growth minus long rate.

Beautiful:
- Nominal growth is above the long rate, or close enough that debt ratios can stabilize.
- The spread is improving after stress.
- Long rates are contained while nominal income recovers.

Mixed:
- Nominal growth and long rates are close.
- Spread improves but remains volatile.
- Long rates rise for healthier reasons, such as better growth expectations, not funding stress.

Ugly:
- Nominal growth is persistently below the long rate.
- Long rates rise while nominal growth is weak.
- Debt-service pressure intensifies.

Why it matters:
- Deleveraging is easier when income growth exceeds borrowing costs. It is ugly when debt compounds faster than nominal incomes.

## Indicator 2: Inflation

Preferred measure:
- CPI, PCE, GDP deflator, or comparable broad inflation gauge.

Beautiful:
- Inflation is positive and moderate.
- Deflation risk fades without runaway inflation.
- Inflation helps lift nominal incomes and reduce real debt burdens.

Mixed:
- Inflation is low but rising from deflationary conditions.
- Inflation is above target but decelerating in an orderly way.
- Relative-price shocks distort the headline reading.

Ugly:
- Deflation or near-zero inflation persists during debt stress.
- Inflation accelerates disorderly and undermines real incomes or long-rate stability.
- Inflation volatility damages confidence and policy credibility.

Why it matters:
- Some reflation is useful in deleveraging. Too little inflation keeps real debt burdens high; too much creates instability.

## Indicator 3: Unemployment Rate

Preferred measure:
- Headline unemployment rate, supplemented by underemployment, participation, or employment-to-population when relevant.

Beautiful:
- Unemployment is falling or stable at tolerable levels.
- Labor-market recovery broadens after the initial shock.
- Wage income supports household deleveraging.

Mixed:
- Unemployment is high but clearly falling.
- Employment improves while participation remains weak.
- Labor data lag the growth recovery.

Ugly:
- Unemployment rises sharply or stays elevated.
- Labor-force exits mask weakness.
- Income losses force defaults, austerity, or political stress.

Why it matters:
- A deleveraging cannot be called beautiful if household incomes and employment keep deteriorating.

## Indicator 4: Real Growth

Preferred measure:
- Real GDP growth, industrial production, real final sales, or a comparable activity measure.

Beautiful:
- Real growth is positive or recovering after a short contraction.
- Growth is less volatile and less dependent on emergency support.
- Private demand improves as balance sheets repair.

Mixed:
- Growth is weak but no longer contracting.
- Recovery is uneven across sectors.
- Headline real growth is distorted by inventories, trade, or base effects.

Ugly:
- Real growth is negative, unstable, or repeatedly relapsing.
- Deleveraging happens through forced spending cuts and defaults.
- Activity remains dependent on emergency policy support.

Why it matters:
- Nominal reflation is not enough. Beautiful deleveraging needs a real activity floor.

## Indicator 5: Government Balance

Preferred measure:
- Fiscal balance as a percent of GDP. Use general government where available.

Beautiful:
- The deficit widens during support, then narrows as growth recovers.
- Fiscal policy supports incomes without creating an uncontrolled funding problem.
- Debt dynamics improve because nominal growth and revenues recover.

Mixed:
- Deficit remains large but is improving.
- One-off support obscures the underlying balance.
- Fiscal consolidation begins while growth remains fragile.

Ugly:
- Fiscal balance deteriorates persistently.
- Austerity deepens contraction, or deficits rise without restoring growth.
- Funding stress pushes long rates up or forces disorderly monetization.

Why it matters:
- Fiscal support can make deleveraging beautiful, but uncontrolled deficits with weak growth can make it ugly.

## Scoring

Assign each indicator:

```text
beautiful = 2
mixed = 1
ugly = 0
unknown = null
```

Interpretation:
- 8-10 points with no more than one mixed and no ugly indicators: beautiful deleveraging.
- 6-7 points: mostly beautiful but monitor weak pillars.
- 4-5 points: mixed or transition.
- 0-3 points, or two or more ugly indicators: ugly deleveraging.
- Any unknown indicators: reduce confidence and list the data needed.

Override rules:
- If nominal growth is far below the long rate and unemployment is rising, do not classify as beautiful even if inflation is positive.
- If inflation is disorderly high and long rates are surging, do not classify as beautiful solely because nominal growth is high.
- If government balance is ugly but the other four indicators are beautiful, classify as mostly beautiful with fiscal risk rather than ugly.

## Pattern Recognition

Beautiful deleveraging often shows:
- Nominal growth recovering above long rates.
- Inflation positive but not spiraling.
- Unemployment rolling over and trending down.
- Real growth recovering from contraction.
- Government deficit narrowing after crisis support.

Ugly deleveraging often shows:
- Nominal growth below long rates.
- Deflation or unstable inflation.
- Unemployment rising or stuck high.
- Real growth contracting or repeatedly relapsing.
- Government balance worsening or failing to recover.

## Common False Reads

- Mistaking high inflation for beauty when real growth and unemployment are ugly.
- Mistaking a shrinking deficit for beauty when it comes from austerity that worsens growth.
- Mistaking low long rates for beauty when nominal growth is even lower.
- Mistaking one quarter of rebound growth for a durable beautiful deleveraging.
- Ignoring base effects after crisis collapses.

## Data Notes

Use official or reputable sources:
- National statistics agencies for real GDP, nominal GDP, inflation, and unemployment.
- Central banks or finance data vendors for long-term government yields.
- Treasury, finance ministry, IMF, OECD, or national budget offices for government balance.

For live analysis, verify source dates and revisions. Fiscal balance and GDP data are often revised and released with lags, while yields and market-implied rates move daily.

## Suggested Output Language

Use concise, conditional language:
- "This is a beautiful deleveraging reading: nominal growth is above long rates, inflation is moderate, unemployment is falling, real growth is positive, and the deficit is narrowing."
- "This is an ugly deleveraging reading: debt-service math is unfavorable, unemployment and real growth are weak, and fiscal balance is deteriorating."
- "This is mixed: nominal reflation is helping, but real growth and unemployment have not yet confirmed a beautiful deleveraging."
