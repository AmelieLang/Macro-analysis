# Official Data Sources

Use this reference to choose data feeds for the bubble matrix. Prefer direct official APIs or downloadable official files. Always cite provider, dataset, series name/code, frequency, latest observation used, and retrieval date.

## Global Official Sources

### Bank for International Settlements

Use BIS first for cross-country credit, property prices, and leverage stress.

- Data portal: https://data.bis.org/
- API documentation: https://stats.bis.org/api-doc/v2/
- Help page: https://data.bis.org/help/tools
- Residential property prices: https://data.bis.org/topics/RPP
- Credit to the non-financial sector: https://www.bis.org/statistics/totcredit.htm
- Debt service ratios: https://data.bis.org/topics/DSR
- Credit-to-GDP gaps: https://data.bis.org/topics/CREDIT_GAPS
- Effective exchange rates and global liquidity: use BIS topics when currency/external funding matters.

Typical rows supported: 1, 3, 7; sometimes 2 through real property price trends.

### OECD

Use OECD for house price valuation ratios, confidence indicators, lending, and macro data for OECD and selected partner economies.

- Data Explorer: https://data-explorer.oecd.org/
- API guidance: https://www.oecd.org/en/data/insights/data-explainers/2024/09/api.html
- Analytical house price indicators: search Data Explorer for `DSD_AN_HOUSE_PRICES` / `DF_HOUSE_PRICES`.
- Housing prices indicator page: https://www.oecd.org/en/data/indicators/housing-prices.html

Useful house-price measures include real house prices, price-to-income ratio, and price-to-rent ratio.

Typical rows supported: 1, 2, 6, 7.

### IMF

Use IMF for macro context, interest rates, external balances, government finance, inflation, unemployment, and financial statistics.

- IMF Data Portal: https://data.imf.org/
- IMF data overview: https://www.imf.org/en/data
- IMF API page: https://data.imf.org/en/Resource-Pages/IMF-API
- WEO: GDP, inflation, unemployment, fiscal balance, current account.
- IFS and related IMF portal datasets: interest rates, exchange rates, money, credit, balance of payments, and reserves.

Typical rows supported: 2, 3, 7; macro controls for all rows.

### World Bank

Use World Bank APIs for country macro series and financial-market indicators, especially when annual country coverage matters.

- Indicators API documentation: https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-about-the-indicators-api-documentation
- Indicators browser: https://data.worldbank.org/indicator
- Market capitalization of listed domestic companies, % of GDP: `CM.MKT.LCAP.GD.ZS`
- Market capitalization, current US$: `CM.MKT.LCAP.CD`
- Listed domestic companies, total: `CM.MKT.LDOM.NO`
- Stocks traded, total value, % of GDP: `CM.MKT.TRAD.GD.ZS`
- Stocks traded, turnover ratio of domestic shares: `CM.MKT.TRNR`
- GDP, inflation, real interest rate, lending rate, unemployment, current account, reserves, exchange rate, and other WDI macro controls.
- Global Financial Development Database indicators include stock market capitalization to GDP (`GFDD.DM.01`) and turnover (`GFDD.EM.01`) where available.

Typical rows supported: 1, 2, 5, 6, 7.

### Eurostat And ECB

Use Eurostat and ECB for European country detail when OECD/BIS/IMF are insufficient.

- Eurostat: https://ec.europa.eu/eurostat
- ECB Data Portal: https://data.ecb.europa.eu/
- Use ECB Statistical Data Warehouse/Data Portal for rates, credit, bank lending, securities issuance, and euro-area financial accounts.
- Use Eurostat for housing, construction, national accounts, labor markets, and confidence where available.

Typical rows supported: 1, 3, 4, 6, 7.

## National Official Sources

Use national sources whenever the bubble question is country-specific and global sources are stale or too aggregated.

### Central Banks And Supervisors

Look for:

- Policy rates, yield curves, real rates, monetary aggregates, bank credit, sectoral credit, debt service, lending standards, non-performing loans, and financial stability reports.
- Household debt, corporate debt, mortgage characteristics, loan-to-value, debt-to-income, floating-rate share, maturity mismatch, and stress-test results.
- Macroprudential measures such as LTV caps, DTI caps, reserve requirements, countercyclical capital buffers, and property taxes.

Typical rows supported: 3, 6, 7, with qualitative support for 2 and 5.

### Statistical Offices, Land Registries, And Housing Agencies

Look for:

- House price indexes, rents, disposable income, construction permits, starts, completions, inventories, vacancies, transaction volumes, buyer categories, and regional price dispersion.
- First-time buyer, investor, foreign buyer, and nonresident purchase shares where available.

Typical rows supported: 1, 2, 4, 5.

### Securities Regulators And Exchanges

Look for:

- Market capitalization, index levels, valuation statistics, turnover, margin financing, short interest, new accounts, IPOs, secondary issuance, fund launches, insider filings, and investor composition.
- Regulator annual reports, exchange fact books, and market-statistics downloads.

Typical rows supported: 1, 3, 5, 6.

## U.S. Official And Regulatory Sources

Use these when the country is the United States or when U.S. market positioning is directly relevant:

- Federal Reserve FRED API documentation: https://fred.stlouisfed.org/docs/api/fred/
- Federal Reserve data and Data Download Program/FRED information: https://www.federalreserve.gov/data/data-download-fred-information.htm
- Federal Reserve Financial Accounts (Z.1): debt, credit, net worth, broker-dealer receivables, and sector balance sheets.
- FINRA margin statistics: https://www.finra.org/rules-guidance/key-topics/margin-accounts/margin-statistics
- SEC EDGAR APIs: https://www.sec.gov/search-filings/edgar-application-programming-interfaces and https://data.sec.gov/
- CFTC Commitments of Traders: https://www.cftc.gov/MarketReports/CommitmentsofTraders/index.htm
- CFTC public reporting/API help: https://publicreporting.cftc.gov/stories/s/User-s-Guide/p2fg-u73y/

## Indicator-To-Source Map

```text
1. Prices high relative to traditional measures
   BIS RPP; OECD house price ratios; World Bank market cap/GDP and turnover;
   national exchanges/regulators; national house price and rent data.

2. Prices discount future rapid appreciation
   BIS/OECD real house price growth; World Bank equity and GDP series;
   IMF macro/rate data; official surveys or financial stability reports.

3. Purchases financed by high leverage
   BIS credit, DSR, credit gaps; IMF credit/rates; central bank financial accounts;
   FINRA/Fed/CFTC/market regulators for securities leverage where relevant.

4. Forward purchases
   National statistical offices, land registries, housing agencies, customs/import data,
   central bank sectoral credit, company/regulator filings, and official inventory data.

5. New participants
   Securities regulators/exchanges, SEC EDGAR or local filing systems,
   land registries/housing agencies, central bank household finance surveys,
   World Bank listed companies and market activity indicators.

6. Broad bullish sentiment
   OECD confidence indicators, national official confidence surveys,
   central bank lending surveys and financial stability reports,
   exchange/regulator issuance and turnover data.

7. Tightening risks popping the bubble
   IMF rates/external data; BIS DSR/credit gaps/effective exchange rates;
   central bank rates, yield curves, debt maturity/floating-rate data,
   reserves, capital flows, macroprudential policy, and stress tests.
```

## Data Caveats

- Official global datasets may lag national releases; state the latest observation.
- Historical bubble analysis may need ex-post revised data; state whether real-time vintages are unavailable.
- Market sentiment and forward purchases rarely have one clean global official series; combine official quantity, survey, and regulatory evidence.
- FRED is an official-sector aggregator. When using FRED, cite the original source shown on the series page when possible.
- If a row depends mainly on qualitative reports, quote sparingly and summarize the official document's evidence.
