# Financial Derivatives and Volatility Analysis of NFLX
This project analyzes Netflix (NFLX) stock returns and options market data to study return behavior, 
distributional characteristics, and implied volatility dynamics. Using R, the analysis combines 
equity return statistics, option pricing techniques, and volatility smile visualization to 
demonstrate practical financial data analysis and risk modeling concepts.
## Project Overview
This project is divided into two main analytical components to examine both equity and derivatives markets
for Netflix (NFLX):

1. **Equity Return Analysis**  
   Daily stock prices are transformed into log returns and analyzed to understand return behavior,
   volatility, and distributional characteristics.

2. **Options & Volatility Analysis**  
   Options market data is used to estimate implied volatility, analyze option pricing behavior,
   and visualize volatility smiles to gain insights into market expectations and risk.

Together, these analyses demonstrate an end-to-end financial data workflow, from raw market data
collection to statistical analysis and visualization.

## Dataset

This project uses publicly available financial market data for Netflix (NFLX) from Yahoo Finance.

### Stock Price Data
- Daily historical prices for :contentReference[oaicite:0]{index=0} (ticker: NFLX)
- Time period: January 2025 onward
- Adjusted close prices used to compute daily log returns

### Options Market Data
- Call and put option chains for NFLX across multiple expiration dates
- Fields include strike price, bid, ask, volume, and open interest
- Option mid-prices calculated as the average of bid and ask prices

