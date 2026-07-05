---
name: rays-investment-principles
description: Apply a Ray Dalio/Bridgewater-style investment lens that is fundamental, systematic, and diversified. Use when the user asks for "Ray's angle", "Ray's investment principles", transaction-based pricing, money-and-credit analysis, debt-cycle or liquidity framing, All Weather-style asset-class sensitivities, market pricing versus future expectations, bubbles, macro-to-market transmission, or structured analysis of stocks, bonds, credit, commodities, gold, currencies, inflation, growth, central-bank policy, QE, leverage, or portfolio diversification.
---

# Ray's Investment Principles

## Core Posture

Use this skill to analyze markets through a fundamental, systematic, and diversified lens. Treat markets and economies as the sum of transactions, with prices shaped by total money and credit spent relative to quantity sold.

Do not present the analysis as official advice from Ray Dalio, Bridgewater, or any affiliated entity. Do not give personalized financial advice. If the user asks for a live market view, verify current data before forming conclusions.

## Required Frame

Start from the transaction identity:

`Price = total money and credit spent / total quantity sold`

Translate the user's question into:

1. What market or asset is being priced?
2. Who are the important buyers and sellers?
3. How much money and credit are they likely to spend?
4. How much quantity is being sold or issued?
5. What future growth, inflation, risk premium, and discount-rate assumptions are embedded in price?
6. Where might those assumptions be wrong?

For deeper reference on the framework, read [references/ray-framework.md](references/ray-framework.md).

## Analysis Workflow

1. Define the market machine.
   - Specify the asset, time horizon, currency, and pricing unit.
   - Identify the main buyer and seller cohorts.
   - Separate cash buyers, leveraged buyers, forced sellers, price-insensitive actors, and policy-sensitive actors.

2. Attribute price pressure to dollars and quantity.
   - Break demand into money and credit.
   - Identify leverage, collateral values, lending standards, margin, refinancing needs, and liquidity conditions.
   - Break supply into issuance, production, inventories, buybacks, retirements, and idiosyncratic disruptions or gluts.
   - Emphasize that total spending normally swings faster than physical or financial quantity.

3. Compare market-implied expectations with your view.
   - Infer what price says about future growth, inflation, risk premiums, and discount rates.
   - State whether the market is discounting a plausible, optimistic, pessimistic, or unstable future.
   - Name the specific disagreement that could create opportunity.

4. Map the asset's environmental bias.
   - Equities usually benefit from stronger-than-expected growth and often from lower-than-expected inflation.
   - Nominal bonds usually benefit from weaker-than-expected growth and lower-than-expected inflation.
   - Inflation-linked bonds usually benefit most from falling real yields and can benefit from realized inflation protection.
   - Commodities usually benefit from stronger-than-expected growth and higher-than-expected inflation.
   - Gold usually behaves more like anti-fiat monetary insurance than a normal growth asset.
   - Corporate credit usually benefits from stronger growth, but spreads can widen sharply when default risk rises.
   - EM hard-currency debt spreads often benefit from stronger global growth and, for exporters, higher commodity-linked inflation.

5. Connect policy and liquidity.
   - Examine central-bank reaction function, short rates, long rates, QE/QT, money creation, credit creation, fiscal deficits, currency pressure, and debt-service burdens.
   - Distinguish money printing that offsets credit contraction from money printing that adds to already-expanding credit.

6. Test for bubble or deleveraging dynamics.
   - Look for extrapolated expectations, leveraged buying, broad buyer entry, new issuance, worsening quality, policy accommodation, and vulnerability to tightening.
   - Look for falling collateral values, forced selling, credit contraction, rising defaults, and policy attempts to replace lost private credit with public money.

7. Convert the view into a diversified portfolio implication.
   - Do not make the answer depend on a single macro forecast.
   - Identify what wins and loses if growth rises/falls and inflation rises/falls.
   - Suggest hedges or balanced exposures when uncertainty is high.

## Output Structure

Prefer this structure unless the user requests a different format:

1. Bottom line
2. Transaction map: buyers, sellers, money, credit, quantity
3. What price is discounting
4. Growth/inflation/risk-premium/discount-rate drivers
5. Policy and liquidity transmission
6. Upside case, downside case, and what would change the view
7. Portfolio or risk-management implication

Use concise tables when comparing assets, regimes, or buyer/seller cohorts.

## Guardrails

- Distinguish realized data from expectations.
- Distinguish nominal growth from real growth and inflation.
- Distinguish real yields, break-even inflation, nominal yields, and credit spreads.
- Treat credit as spending power, not as a footnote.
- Prefer causal transaction attribution over vague statements like "the market was risk-on."
- State uncertainty and the indicators that would falsify the view.
