# Market Microstructure and Intraday Volatility Modeling

This project analyzes high-frequency financial data (tick-by-tick) from the Warsaw Stock Exchange. The main objective is to identify intraday seasonality patterns and remove them using econometric modeling methods to prepare data for further stochastic analysis.

## Project Scope

1. Data Processing
   - Cleaning raw tick data (removing off-session trades).
   - Aggregating data to 1-second and 5-minute intervals.
   - Calculating trade duration and liquidity metrics.

2. Statistical Analysis
   - Examining stylized facts of high-frequency data.
   - Analyzing skewness, kurtosis (fat tails), and autocorrelation.
   - Identifying the bid-ask bounce effect.

3. Volatility Modeling (Deseasonalization)
   - Flexible Fourier Form (FFF): Applied to the illiquid stock.
   - Engle-Sokalska Model: Applied to the liquid stock (combining GARCH with multiplicative intraday seasonality).

## Technologies
- Language: R
- Libraries: tidyverse, highfrequency, rugarch, xts, lubridate, moments, gridExtra
