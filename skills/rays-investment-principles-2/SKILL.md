---
name: rays-investment-principles-2
description: Apply Ray Dalio/Bridgewater-style "scariest tables" and All Weather portfolio construction principles. Use when asked to assess long-horizon portfolio ruin risk, 60/40 fragility, real purchasing-power preservation, survivorship bias, risk share versus capital share, equity-dominated beta portfolios, environmental growth/inflation balance, stock-bond correlation instability, geographical diversification, gold or commodity diversification, or All Weather-style strategic asset allocation.
---

# Ray's Investment Principles 2

## Core Posture

Use this skill to evaluate strategic asset allocation through the lens of long-term real wealth preservation, not short-term volatility. Treat investment risk as failing to earn enough money to meet needs, suffering drawdowns that cannot be recovered from, or losing wealth through currency devaluation, confiscation, war, capital controls, or market closure.

Do not present the analysis as official advice from Ray Dalio, Bridgewater, or any affiliated entity. Do not give personalized financial advice. If the user asks for a live portfolio or market recommendation, verify current data and state uncertainty.

## Required Frame

Start with four questions:

1. What real spending need, liability, or purchasing-power target must the portfolio satisfy?
2. What time horizon and maximum tolerable real drawdown matter: 1 year, 5 years, 10 years, 20 years, or permanent impairment?
3. Where is the portfolio's risk concentrated by asset class, country, currency, growth bias, inflation bias, liquidity, and leverage?
4. Which economic surprises would hurt the portfolio: rising growth, falling growth, rising inflation, falling inflation, rising risk premiums, or falling discount rates?

Prefer long-history and cross-country evidence over single-country backtests. Flag survivorship bias whenever the analysis depends heavily on the United States, markets that stayed open, or countries that avoided confiscation, default, war, or currency destruction.

## Analysis Workflow

1. Define risk relative to the objective.
   - Separate volatility from shortfall risk, drawdown risk, ruin risk, liquidity risk, currency risk, policy/confiscation risk, and opportunity cost.
   - Measure returns in the user's spending currency and in real terms when purchasing power matters.
   - Treat cash as low nominal volatility but high long-term real purchasing-power risk.

2. Stress-test "passive long horizon" assumptions.
   - Ask whether the portfolio would have survived 5-year and 20-year real return droughts, not only daily or monthly drawdowns.
   - Examine major historical environments: wars and confiscations, the 1910s, the Great Depression, the 1940s, the 1970s, Japan after 1990, the 2000s equity drawdown, 2008, 2020, and 2022 inflation/rate shocks.
   - Emphasize that a country can have acceptable average returns but still experience ruinous periods from which a concentrated investor cannot recover.

3. Diagnose capital allocation versus risk allocation.
   - Estimate each asset's risk contribution, not just its capital weight.
   - Remember that a 60/40 or 70/30 portfolio is usually dominated by equity risk because equities are much more volatile than bonds.
   - Treat private equity, venture capital, high yield, corporate credit, real estate, and some hedge-fund beta as potentially equity-like unless their return drivers prove otherwise.

4. Convert desired risk shares to rough capital shares when needed.
   - Use this simple approximation when correlations are not being modeled:
     `capital share_i = (target risk share_i / expected volatility_i) / sum(target risk share / expected volatility)`
   - Example: target 70% bond risk at 8% volatility and 30% equity risk at 16% volatility gives roughly 82% bonds and 18% equities by capital.
   - State that full portfolio construction should use covariance, liquidity, leverage constraints, implementation costs, and stress tests.

5. Map environmental biases.
   - Use growth and inflation surprises relative to what markets discounted, not realized levels alone.
   - Classify assets by their structural cash-flow sensitivities before looking at correlations.
   - Use this baseline map:

| Asset or Return Stream | Growth Bias | Inflation Bias | Notes |
| --- | --- | --- | --- |
| Equities | Rising growth | Falling inflation | Claim on future earnings; usually hurt by inflation surprises and discount-rate spikes. |
| Stable cash-flow equities | Rising growth or defensive growth | Falling inflation | Equity-like, often lower cyclicality but still duration/equity risk. |
| Nominal government bonds | Falling growth | Falling inflation | Fixed payments benefit from weaker growth and lower inflation/discount rates. |
| Inflation-linked bonds | Falling growth | Rising inflation | Help when real yields fall and inflation protection matters. |
| Commodities ex-gold | Rising growth | Rising inflation | Benefit from demand pressure, supply constraints, and inflation shocks. |
| Gold | Crisis/monetary hedge | Rising monetary inflation or fiat concern | Can help in deep deflationary depressions, currency debasement, and geopolitical shocks. |
| Corporate credit | Rising growth | Falling inflation | Equity-like spread risk plus bond duration. |
| EM credit | Rising growth | Mixed to rising inflation for commodity exporters | Sensitive to global liquidity, USD, commodities, and default risk. |
| Cash | Low near-term market beta | Vulnerable to devaluation | Useful for liquidity, poor as long-run real store of wealth. |

6. Diagnose the 60/40 portfolio.
   - Identify it as a disinflationary-growth portfolio, not a neutral portfolio.
   - Explain that bonds diversify equities in growth shocks but often fail when inflation or risk premiums rise.
   - Treat stock-bond correlation as environment-dependent: inflation-dominant regimes can make stocks and bonds positively correlated; growth-dominant regimes can make them negatively correlated.

7. Engineer All Weather-style balance.
   - Build four sub-portfolios with equal risk: rising growth, falling growth, rising inflation, falling inflation.
   - Populate each box with assets whose cash flows logically benefit when that environment is repriced.
   - Scale return streams by risk, duration, leverage, futures, swaps, cash, or delevering rather than forcing capital weights to hit the return target.
   - Seek to neutralize growth and inflation surprise risk so risk premiums and discount rates become the dominant return source over time.
   - Keep the portfolio globally diversified across countries, currencies, and liquid markets to reduce idiosyncratic national failure risk.

8. Treat diversification as return-stream engineering.
   - Prefer many decent, lowly correlated return streams over one apparently superior asset.
   - Do not rely on historical average correlations as a primary hedge design tool; explain the economic reason the hedge should work.
   - Evaluate whether a small diversifying overlay, such as gold or commodities, improves drawdown behavior even if its standalone Sharpe ratio is lower.

9. Compare concentrated beta with balanced beta.
   - Show how an equity-dominated portfolio can have high expected return but poor reliability and long underwater periods.
   - Explain that a more balanced portfolio can target the same expected return with less risk, or a higher return for the same risk, if it has a higher return-to-risk ratio and can be scaled responsibly.
   - Separate beta construction from alpha views. Strategic allocation should not require correctly forecasting the next regime.

## Output Structure

Use this structure unless the user requests another format:

1. Bottom line
2. Objective and definition of risk
3. Capital allocation versus estimated risk allocation
4. Environmental-bias map
5. Scariest-table stress tests: worst real drawdowns, long droughts, country/currency failure, survivorship bias
6. 60/40 or current-portfolio failure modes
7. All Weather-style rebalance or diagnostic: four boxes and missing exposures
8. Implementation caveats: leverage, duration, liquidity, taxes, costs, data quality, and mandate constraints
9. What evidence would change the view

Use concise tables for portfolio exposures, environmental boxes, and stress-test results.

## Guardrails

- Distinguish real returns from nominal returns.
- Distinguish long-term purchasing-power risk from mark-to-market volatility.
- Distinguish capital allocation from risk allocation.
- Distinguish expected growth/inflation levels from surprises relative to discounted expectations.
- Distinguish risk premiums from environmental repricing.
- Do not assume US market history is normal.
- Do not assume stocks and bonds will always diversify each other.
- Do not equate owning many assets with diversification if they share the same hidden growth, inflation, credit, or liquidity beta.
- Be explicit when using simplified volatility-only calculations instead of full covariance-based portfolio construction.
- State that leverage can scale return streams but introduces financing, margin, liquidity, counterparty, behavioral, and implementation risks.
