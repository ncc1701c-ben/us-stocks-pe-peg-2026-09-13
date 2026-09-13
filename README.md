# US listed common stocks — P/E and PEG comparison

**Latest snapshot:** 13 September 2026

Every primary common stock in the TradingView America scanner (NYSE / NASDAQ / AMEX), joined to Polygon.io trailing ratios. Finviz valuation was not reachable this run (Cloudflare / Elite export), so classic PEG_5Y_expected is blank.

## Google Sheet (weekly)

https://docs.google.com/spreadsheets/d/1lzwiJZV6_LjbjsQhwKIY2DjmRxrSSRkgC1AtPAHjuEo/edit

Live-link a tab with:

```
=IMPORTDATA("https://raw.githubusercontent.com/ncc1701c-ben/us-stocks-pe-peg-2026-09-13/main/US_major_listed_PE_PEG_weekly.csv")
```

## Coverage (13 Sep 2026)

- NYSE + NASDAQ + AMEX primary common: **4,948** tickers
- Trailing P/E > 0: **2,550** (median **21.27**)
- PEG_TTM_growth (TradingView trailing growth): computed where PE and YoY EPS growth are usable
- PEG_5Y_expected (Finviz classic PEG): **0** this week (Finviz blocked)
- S&P 500 matched: **497**
- OTC common supplemental: **5,781**

Blank P/E = unprofitable or no TTM EPS. Blank classic PEG = Finviz unavailable.

## Two PEGs — do not mix them

- `PEG_TTM_growth` = P/E ÷ **trailing** EPS growth (TradingView). **Not** Peter Lynch PEG. Near-zero values are usually a growth-base artifact, not a bargain.
- `PEG_5Y_expected` = classic PEG ≈ Forward P/E ÷ **next-5-year expected** EPS growth (Finviz). Blank this week.

Sources: TradingView America scanner, Polygon.io ratios (as-of cluster 11 Sep 2026).
Not investment advice.
