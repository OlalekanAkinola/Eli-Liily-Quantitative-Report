Eli Lilly Python Analysis

Letter E in my A–Z Equity Research Series, comparing Eli Lilly (LLY) with Novo Nordisk (NVO) and the SPDR S&P 500 ETF Trust (SPY).

This project applies Python to market performance, risk measurement, financial statement analysis, technical charts and Monte Carlo simulation. It explores how a company's operating growth can differ from its share-price performance.

Author: Olalekan Emmanuel Akinola


Scope
Component	Measurement period or specification
Historical market performance	January 2020–December 2025
Current-year market performance	2026 YTD through 2 October 2026
Financial statements	FY2020–FY2025 and H1 2026
Primary company	Eli Lilly, LLY
Selected peer	Novo Nordisk, NVO
Broad market proxy	SPY, an ETF tracking the S&P 500
Monte Carlo calibration window	September 2023–2 October 2026
Monte Carlo simulation	10,000 paths over 252 trading days
Simulation starting price	$1,142.84, as used in the report


Historical returns are annualized; YTD returns are cumulative and cover only part of a year. Volatility is annualized, rather than the size of a typical daily price move.

Selected findings

Selected results from the Python analysis are summarized below.

Measure	Eli Lilly	SPY	Novo Nordisk
Historical annualized return	41.97%	16.02%	17.23%
Historical annualized volatility	33.96%	20.78%	34.80%
Historical maximum drawdown	−34.47%	−33.70%	−68.49%
2026 YTD return	6.29%	13.53%	−25.20%
YTD annualized volatility	36.87%	13.15%	47.90%
YTD maximum drawdown	−23.50%	−8.90%	−43.60%
Lilly's historical Sharpe and Sortino ratios were 1.15 and 1.83, compared with 0.06 and 0.11 in the YTD assessment.
FY2025 revenue reached approximately $65.18 billion, up 44.7%; operating and net margins reached 40.4% and 31.7%.
H1 2026 revenue reached approximately $42.77 billion, up 51.2% against H1 2025.
Free cash flow recovered from approximately $0.8 billion in FY2023 to $9.0 billion in FY2025. H1 2026 generated approximately $10.8 billion.
Strong operating growth did not translate into equally strong YTD stock performance in this measurement window.
Free cash flow here means operating cash flow less purchases of property and equipment. It excludes separate acquisition and purchased in-process R&D spending. Operating R&D is already reflected in operating cash flow and should not be deducted a second time. H1 totals should not be compared with full-year totals as equivalent periods.

Analysis covered
- Historical and YTD returns, annualized volatility, beta, CAPM and maximum drawdown.
- Historical and YTD Sharpe-versus-Sortino comparisons across Lilly, Novo Nordisk, SPY and the healthcare proxy, including the distinction between total and downside risk.
- One-day historical VaR and CVaR at 95% confidence using YTD daily returns: reported loss magnitudes of 2.78% and 4.28%, respectively.
- Revenue, revenue growth, profitability margins, operating cash flow, CapEx, R&D and free cash flow.
- Candlestick charts and moving averages.
- Monte Carlo paths and the distribution of terminal prices.

Valuation is reserved for a separate exercise. Portfolio optimization is outside this project's scope.

Monte Carlo exercise
Output	Reported result
Mean terminal price	$1,561.12
Median terminal price	$1,464.49
5th percentile terminal price	$830.21
95th percentile terminal price	$2,602.00
Simulated outcomes above starting price	76.46%
Simulated outcomes below starting price	23.54%


These are outcomes under the model's assumptions, not forecasts or valuation targets. The share finishing above the starting price is a simulation frequency, not a reliable real-world probability of profit.

Python tools
The exercise uses pandas and NumPy for data processing and calculations, yfinance for market data, Matplotlib for charts and mplfinance for candlestick charts.

Data sources
- Yahoo Finance — Eli Lilly
- Yahoo Finance — Novo Nordisk
- Yahoo Finance — SPY
- Lilly FY2025 Annual Report
- Lilly H1 2026 Form 10-Q
- Lilly FY2024 Form 10-K
- Lilly Annual Reports archive
The report uses a 5.28% US 10-year Treasury yield recorded on 2 October 2026 as its stated risk-free reference for CAPM and Sharpe calculations.

Educational purpose
This is a personal Python and financial-data analysis exercise. It does not constitute investment advice, a recommendation or an offer to buy or sell securities. Historical outcomes and simulations do not guarantee future performance.

More of my work
- GitHub
- Lemm Financials
