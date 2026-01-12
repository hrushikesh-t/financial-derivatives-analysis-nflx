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
## Methodology

### Equity Return Analysis
- Downloaded daily historical price data for NFLX
- Computed daily log returns using adjusted close prices
- Visualized return series to examine volatility behavior
- Calculated skewness and kurtosis to assess distributional properties
- Compared adjusted and unadjusted statistical measures

---

### Options & Volatility Analysis
- Retrieved call and put option chains for multiple expiration dates
- Computed option mid-prices as the average of bid and ask prices
- Implemented Black–Scholes pricing formulas for calls and puts
- Estimated implied volatility using a numerical root-finding (bisection) method
- Handled edge cases where implied volatility could not be computed
- Visualized put option volatility smiles across selected expiration dates

## Results & Insights

### Equity Return Behavior
- Daily log returns exhibited noticeable volatility and non-normal behavior
- Negative skewness indicated a higher probability of extreme negative returns
- High kurtosis reflected fat tails, suggesting the presence of extreme market movements
- Differences between adjusted and unadjusted statistics highlighted the importance of bias correction in financial return analysis

**Insight:**  
Return distributions deviate significantly from normality, reinforcing the need for risk-aware modeling rather than relying solely on mean–variance assumptions.

---

### Options & Implied Volatility
- Implied volatility varied across strike prices and expiration dates
- Numerical root-finding successfully estimated implied volatility for liquid options
- Volatility smiles were observed for put options, particularly around at-the-money strikes

**Insight:**  
The presence of volatility smiles indicates that market participants price tail risk asymmetrically, reflecting higher perceived downside risk and uncertainty.
## Tech Stack
- R
- Financial Data Analysis
- Time Series & Return Analysis
- Options Pricing
- Black–Scholes Model
- Numerical Methods (Bisection)
- Data Visualization
## How to Run
1. Clone the repository
2. Open the R Markdown file in RStudio
3. Install required R packages (quantmod, zoo, TTR, etc.)
4. Knit the `.Rmd` file to reproduce the analysis and results
5. ## Code & Report
- `FE515_FinalProject.Rmd` — Full analysis and implementation
- `FE515_FinalProject.pdf` — Rendered report with results and visualizations

