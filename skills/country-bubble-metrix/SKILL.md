---
name: country-bubble-metrix
description: Build a country-year bubble matrix using the seven-question bubble framework. Use when asked to judge whether a specific country, market, or period is in an asset/debt bubble; to score historical bubbles; to update a bubble dashboard with official data; or to map valuation, leverage, forward demand, new-participant, sentiment, and tightening-risk indicators to official sources.
---

# Country Bubble Metrix

## Overview

Use this skill to judge whether a country in a given year is in a bubble by producing a seven-row evidence matrix backed by official or official-sector data. The framework is designed for country-level asset bubbles, especially equity, housing, credit, and broad debt-cycle bubbles.

## Workflow

1. Identify the country, year or date range, target market, and whether the user wants a historical or current assessment.
2. Load `references/bubble-indicator-catalog.md` for the seven checks, proxy indicators, scoring rules, and reporting template.
3. Load `references/official-data-sources.md` to select official data sources and API entry points.
4. Gather the most recent available data for current assessments; for historical assessments, use vintages when available and clearly label ex-post data.
5. Score each row as `yes`, `mixed`, `no`, or `unknown`. Use `unknown` instead of filling gaps with assumptions.
6. Return the matrix first, then the synthesis, source notes, and caveats.

## Evidence Standard

Prefer sources in this order:

1. National official sources: central bank, statistical office, finance ministry, securities regulator, land registry, exchange, or supervisory agency.
2. Official international datasets: BIS, IMF, OECD, World Bank, Eurostat, ECB, Federal Reserve, and comparable official-sector sources.
3. Official regulatory or self-regulatory market data where relevant, such as FINRA margin statistics, SEC EDGAR, or CFTC Commitments of Traders.
4. Non-official sources only when no official source exists; label them as supplementary and do not let them dominate the score.

Use multiple indicators per row when possible. A single stretched valuation ratio is not enough to call a bubble unless leverage, participation, sentiment, and tightening vulnerability also support the diagnosis.

## Output Shape

Start with this matrix:

```text
Country/market/year: <country, market, year>
Verdict: Strong bubble | Probable bubble | Watchlist | Weak bubble evidence | Insufficient data
Confidence: High | Medium | Low

| # | Bubble check | Score | Official indicators used | Evidence summary | Data/source caveats |
|---|---|---|---|---|---|
| 1 | Prices high relative to traditional measures | yes/mixed/no/unknown | ... | ... | ... |
| 2 | Prices discount future rapid appreciation | yes/mixed/no/unknown | ... | ... | ... |
| 3 | Purchases financed by high leverage | yes/mixed/no/unknown | ... | ... | ... |
| 4 | Buyers/companies making forward purchases | yes/mixed/no/unknown | ... | ... | ... |
| 5 | New participants entered the market | yes/mixed/no/unknown | ... | ... | ... |
| 6 | Broad bullish sentiment | yes/mixed/no/unknown | ... | ... | ... |
| 7 | Tightening risks popping the bubble | yes/mixed/no/unknown | ... | ... | ... |
```

Then add:

- `Score summary`: count yes, mixed, no, unknown.
- `Bubble call`: explain why the pattern does or does not meet the threshold.
- `Most important evidence`: list the 3-5 indicators carrying the conclusion.
- `Missing data`: name the absent official series that would improve confidence.
- `Source notes`: cite data providers, series names/codes, release dates, and retrieval dates.

## Guardrails

- Do not present the result as investment advice.
- Do not treat high prices alone as a bubble; require evidence across the full matrix.
- Do not treat missing data as a `no`.
- Separate broad country bubbles from asset-specific bubbles such as housing-only or equity-only bubbles.
- For current assessments, browse or otherwise verify live official data before answering.
- Use country context: capital controls, pegged currencies, state-directed credit, shadow banking, and data quality can change the interpretation.
