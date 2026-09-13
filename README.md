# US listed common stocks — P/E and PEG comparison

**Latest snapshot:** 13 September 2026

Every common stock in the TradingView America scanner, joined to Polygon.io trailing ratios and Finviz valuation.

## Google Sheet (weekly)

Google Drive is connected, but this account cannot *create* a native Sheet from here. Fastest path:

1. In Google Sheets: **File → Import** the Excel workbook from Grok, or
2. Live-link a tab with:

```
=IMPORTDATA("https://raw.githubusercontent.com/ncc1701c-ben/us-stocks-pe-peg-2026-09-13/main/US_major_listed_PE_PEG_weekly.csv")
```

A Sunday 6:00pm America/Chicago Grok automation rebuilds the file each week.

## Coverage (13 Sep 2026)

- NYSE + NASDAQ + AMEX common: **5,188** tickers
- Trailing P/E: **2,687** (median **21.3**)
- PEG_TTM_growth (TradingView, trailing growth): **2,120** (median **0.24**)
- PEG_5Y_expected (Finviz classic PEG): **1,577** (median **1.11**)
- S&P 500 classic PEG median: **1.51**

Blank P/E = unprofitable or no TTM EPS. Blank PEG = no usable growth estimate.

## Two PEGs — do not mix them

- `PEG_TTM_growth` = P/E ÷ **trailing** EPS growth (TradingView). **Not** Peter Lynch PEG.
- `PEG_5Y_expected` = classic PEG ≈ Forward P/E ÷ **next-5-year expected** EPS growth (Finviz).

Correlation on the S&P 500 is about 0.05.

Sources: TradingView, Polygon.io (11 Sep 2026), Finviz (13 Sep 2026).
Not investment advice.
