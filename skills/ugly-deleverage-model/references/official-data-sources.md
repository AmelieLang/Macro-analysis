# Official Data Sources

Use official or official-sector data first. For current assessments, verify the latest releases and cite retrieval dates.

## Japan Primary Sources

### Cabinet Office / ESRI

Use for:

- Real GDP and nominal GDP.
- Potential growth and output gap estimates where available.
- National Accounts and macro releases.

Entry points:

- Cabinet Office Economic and Social Research Institute: https://www.esri.cao.go.jp/en/
- National Accounts: https://www.esri.cao.go.jp/en/sna/menu.html
- Monthly Economic Report and output-gap/potential-growth materials from Cabinet Office: https://www5.cao.go.jp/keizai3/getsurei-e/index-e.html

### Bank of Japan

Use for:

- Call rates, basic discount/basic loan rates, money-market rates.
- Long rates and financial markets.
- Effective exchange rates.
- Flow of Funds: debt, credit, sector balance sheets.
- Monetary base, central bank balance sheet, deposits and loans.

Entry points:

- BOJ Statistics: https://www.boj.or.jp/en/statistics/index.htm
- BOJ Time-Series Data Search: https://www.stat-search.boj.or.jp/index_en.html
- Flow of Funds: https://www.boj.or.jp/en/statistics/sj/index.htm
- Effective Exchange Rate: https://www.boj.or.jp/en/statistics/market/forex/jikko/index.htm
- Foreign Exchange Rates: https://www.boj.or.jp/en/statistics/market/forex/fxdaily/index.htm

### Statistics Bureau of Japan

Use for:

- Unemployment rate and Labour Force Survey.
- Consumer Price Index.
- Population and household statistics.

Entry points:

- Statistics Bureau: https://www.stat.go.jp/english/
- Labour Force Survey: https://www.stat.go.jp/english/data/roudou/index.html
- Labour Force Survey monthly results: https://www.stat.go.jp/english/data/roudou/results/month/index.html
- Consumer Price Index: https://www.stat.go.jp/english/data/cpi/index.html

### METI

Use for:

- Indices of Industrial Production.
- Production, shipments, inventories, production capacity, and operating ratio.

Entry points:

- Indices of Industrial Production: https://www.meti.go.jp/english/statistics/tyo/iip/index.html
- Historical IIP data: https://www.meti.go.jp/english/statistics/tyo/iip/b2020_result-2.html

### Ministry of Finance Japan

Use for:

- Fiscal statistics, budget, debt, JGBs, balance of payments, reserves, and intervention.
- Long JGB interest-rate historical data when needed.

Entry points:

- MOF Statistics: https://www.mof.go.jp/english/statistics/index.html
- JGB interest rates: https://www.mof.go.jp/english/policy/jgbs/reference/interest_rate/index.htm
- Central government debt and JGB data: use the JGBs section of MOF Statistics.
- Balance of Payments, international reserves, and intervention: use the International Policy section of MOF Statistics.

### Japan Exchange Group

Use for:

- TOPIX, equity market data, trading volume, margin and short-selling related market statistics where available.
- Historical index values and market statistics.

Entry points:

- JPX Data and Statistics: https://www.jpx.co.jp/english/markets/
- TOPIX: https://www.jpx.co.jp/english/markets/indices/topix/

## Cross-Country Official Sources

Use these to compare Japan with other country cases or when national data are hard to access.

### BIS

Use for credit, debt service, credit gaps, residential property prices, and real/nominal effective exchange rates.

- BIS Data Portal: https://data.bis.org/
- BIS API documentation: https://stats.bis.org/api-doc/v2/
- Residential property prices: https://data.bis.org/topics/RPP
- Credit to the non-financial sector: https://www.bis.org/statistics/totcredit.htm
- Debt service ratios: https://data.bis.org/topics/DSR
- Credit-to-GDP gaps: https://data.bis.org/topics/CREDIT_GAPS

### IMF

Use for WEO macro series, IFS interest rates/exchange rates, government finance, balance of payments, reserves, and cross-country current account data.

- IMF Data: https://www.imf.org/en/data
- IMF Data Portal: https://data.imf.org/
- IMF API: https://data.imf.org/en/Resource-Pages/IMF-API

### OECD

Use for GDP, unemployment, inflation, output gaps, confidence indicators, house prices, and long-rate comparisons.

- OECD Data Explorer: https://data-explorer.oecd.org/
- OECD API guidance: https://www.oecd.org/en/data/insights/data-explainers/2024/09/api.html
- Housing prices: https://www.oecd.org/en/data/indicators/housing-prices.html

### World Bank

Use for annual macro and financial-market indicators, especially market capitalization to GDP and official exchange rate.

- Indicators API: https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-about-the-indicators-api-documentation
- Indicators browser: https://data.worldbank.org/indicator
- Official exchange rate: `PA.NUS.FCRF`
- Market capitalization, percent of GDP: `CM.MKT.LCAP.GD.ZS`
- Stocks traded turnover ratio: `CM.MKT.TRNR`

### FRED As Official-Sector Aggregator

Use FRED for convenient retrieval only when the underlying source is official, and cite the original provider shown on the FRED series page.

- FRED API: https://fred.stlouisfed.org/docs/api/fred/
- Example: Japan general government gross debt series cites IMF WEO as the underlying source.

## Data Construction Notes

- Real growth versus potential growth: use real GDP growth minus potential growth, or compare actual real GDP level with potential GDP/output gap.
- Real rates: nominal policy or money-market rate minus current/expected inflation.
- Yield curve: long government yield minus short rate.
- Net domestic debt: use BOJ Flow of Funds or BIS credit/debt measures; be explicit about sector coverage.
- Asset prices: use TOPIX/Nikkei/JPX for equities; use BIS/OECD/national land/property indexes for real estate.
- P/E ratio: prefer exchange or official market-statistics sources. If official P/E is unavailable, label commercial estimates as supplementary.
- Reserve flow: use changes in reserves or official balance-of-payments reserve assets scaled by GDP.
- Fiscal balance: use general government balance when cross-country comparable; use national fiscal data for timelier local analysis.
