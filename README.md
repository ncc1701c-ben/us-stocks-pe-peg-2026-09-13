# US listed common stocks — P/E and PEG comparison

**Snapshot date:** 13 September 2026

Every common stock in the TradingView America scanner, joined to Polygon.io trailing ratios and Finviz valuation.

## Coverage

- NYSE + NASDAQ + AMEX common: **5,188** tickers
- Trailing P/E available: **2,687** (median **21.3**)
- PEG_TTM_growth (TradingView, trailing growth): **2,120** (median **0.24**)
- PEG_5Y_expected (Finviz classic PEG): **1,577** (median **1.11**)
- S&P 500 classic PEG median: **1.51**
- Quality screen (cap ≥ $300M, P/E 5–50, classic PEG 0.05–2.5): **922** names, median classic PEG **1.04**
- OTC common: **5,782** additional names

Blank P/E = unprofitable or no TTM EPS. Blank PEG = no usable growth estimate. That is expected.

## Two PEGs — do not mix them

- `PEG_TTM_growth` = P/E ÷ **trailing** EPS growth (TradingView). **Not** Peter Lynch PEG. Correlation vs classic PEG on S&P 500 is ~0.05.
- `PEG_5Y_expected` = classic PEG ≈ Forward P/E ÷ **next-5-year expected** EPS growth (Finviz). This is the PEG investors usually mean.

## Files

- `US_sector_medians_PE_PEG.csv` — sector medians
- `US_mega_caps_PE_PEG.csv` — top 50 by market cap
- `US_quality_classic_PEG.csv` — 922-name quality screen
- `SP500_PE_PEG_Finviz_vs_TradingView.csv` — S&P 500 multi-source comparison
- `US_major_listed_PE_PEG.csv` — full 5,188-row dual-PEG table

Open CSVs in Excel or Google Sheets (File → Import).

Sources: TradingView America scanner, Polygon.io ratios (11 Sep 2026), Finviz valuation screener (13 Sep 2026).
Not investment advice.
