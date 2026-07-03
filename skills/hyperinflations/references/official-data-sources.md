# Official Data Sources

Use official or official-sector data first. Cite source, series, date, frequency, and retrieval date.

## Core Official Sources

### IMF

Use for CPI, exchange rates, money, reserves, balance of payments, fiscal balance, debt, and program documents.

- IMF Data Portal: https://data.imf.org/
- IMF API: https://data.imf.org/en/Resource-Pages/IMF-API
- World Economic Outlook: https://data.imf.org/en/datasets/IMF.RES%3AWEO
- International Financial Statistics: search IMF Data Portal topics for prices, money, exchange rates, interest rates, and reserves.
- Balance of Payments and International Investment Position: current account, financial account, reserves, and external position.
- Government Finance Statistics and Fiscal Monitor: fiscal balance, debt, revenue, spending, and financing.
- IMF country reports/program documents: conditionality, financing gaps, money targets, exchange-rate regime, arrears, and debt restructuring.

### World Bank

Use for annual cross-country indicators and external debt.

- Indicators browser: https://data.worldbank.org/indicator
- Indicators API documentation: https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-about-the-indicators-api-documentation
- International Debt Statistics: https://datacatalog.worldbank.org/search/dataset/0038015/international-debt-statistics

Useful indicator families:

- Inflation, consumer prices: `FP.CPI.TOTL.ZG`
- CPI index: `FP.CPI.TOTL`
- Official exchange rate: `PA.NUS.FCRF`
- Broad money growth: `FM.LBL.BMNY.ZG`
- Broad money percent of GDP: `FM.LBL.BMNY.GD.ZS`
- Total reserves: `FI.RES.TOTL.CD`
- Current account balance: `BN.CAB.XOKA.CD`, `BN.CAB.XOKA.GD.ZS`
- Imports and exports of goods/services: WDI trade indicators.
- External debt stocks and debt service: use IDS indicators by country.

### BIS

Use for effective exchange rates, foreign-currency credit, debt service, credit gaps, and banking exposure.

- BIS Data Portal: https://data.bis.org/
- BIS API documentation: https://stats.bis.org/api-doc/v2/
- Effective exchange rates: https://www.bis.org/statistics/eer.htm
- Global liquidity indicators: use for foreign-currency credit where available.
- International banking statistics: use when cross-border bank funding matters.

### National Official Sources

Use country central banks, statistical offices, finance ministries, debt offices, and securities exchanges for timely or high-frequency data:

- CPI and wage indexes.
- Daily or monthly exchange rates.
- Monetary base, broad money, central-bank credit to government, central-bank balance sheet.
- FX reserves, intervention, import cover, external debt service.
- Fiscal deficit, arrears, debt issuance, central bank financing.
- Bank deposits by maturity and currency, deposit withdrawals, credit growth.
- Wage indexation, price controls, capital controls, currency redenomination, and new currency announcements.

## Data Construction Notes

- Annual inflation: use year-over-year CPI when monthly data exist; use annual average only when high-frequency data are unavailable.
- Price doubling threshold: annual inflation above 100 percent means prices more than double yearly.
- Monthly hyperinflation marker: monthly CPI inflation above 50 percent is a severe classic threshold.
- Real interest rate: policy or money-market rate minus current or expected inflation.
- Currency depreciation: use local currency per USD or trade-weighted exchange rate; make direction clear.
- Money acceleration: compare monetary base and broad money growth to inflation, exchange-rate depreciation, and nominal GDP.
- External financing gap: current account deficit plus external debt service/maturities minus stable inflows and official financing.
- Money-function breakdown: official data may be scarce; use central-bank/finance-ministry documents, IMF reports, legal tender changes, redenomination notices, and official controls.
