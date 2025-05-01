# Optimizing a Cryptocurrency Portfolio Using Markowitz Theory

This project applies **Modern Portfolio Theory (MPT)**, developed by Harry Markowitz, to construct and optimize a cryptocurrency portfolio. The goal is to identify the optimal asset allocation that maximizes expected return for a given level of risk, or equivalently, minimizes risk for a target return, within the highly volatile context of digital assets.

## Objectives

- Apply Markowitz’s mean-variance optimization framework to cryptocurrencies
- Analyze the risk-return trade-off in crypto portfolios
- Compare efficient frontiers under different constraints (with or without a risk-free asset)
- Provide practical insights for crypto investors seeking diversification

## Dataset

- **Assets considered:** Bitcoin (BTC), Ethereum (ETH), Solana (SOL), Cardano (ADA), Polkadot (DOT), and others
- **Frequency:** Daily or monthly returns depending on availability
- **Data sources:** Yahoo Finance API, CoinGecko or other public crypto price APIs

## Methodology

1. **Data Collection and Preprocessing**
   - Historical prices are cleaned and aligned
   - Log-returns are computed to ensure stationarity
   - Missing data is handled through forward filling or exclusion

2. **Statistical Analysis**
   - Calculation of expected returns, standard deviations, and covariance matrix
   - Visualization of return distributions and correlation heatmaps

3. **Portfolio Optimization**
   - Construction of the **efficient frontier** using quadratic programming
   - Determination of the **minimum variance portfolio** and the **tangency portfolio**
   - Simulation of 10,000+ random portfolios to visualize the risk/return space
   - Optional: inclusion of a **risk-free asset** (e.g., US T-Bill proxy)

4. **Performance Metrics**
   - Sharpe Ratio
   - Volatility
   - Return
   - Diversification effects

## Tools & Libraries

- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy)
- `cvxopt` or `scipy.optimize` for constrained optimization
- Jupyter Notebook

## Key Insights

- Cryptocurrencies exhibit high volatility but offer diversification opportunities
- The optimal portfolio composition changes significantly depending on whether short selling or a risk-free asset is allowed
- Markowitz optimization, while useful, must be adapted to account for the extreme behavior of crypto assets

## Author

**Abdoulaye Gaye**  
Université Paris Dauphine  
Specialization: Quantitative Finance & Portfolio Optimization
