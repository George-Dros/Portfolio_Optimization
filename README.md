# Portfolio Optimization and Efficient Frontier Analysis

This project explores portfolio optimization techniques to find the best risk-return trade-offs for a set of financial assets. Using Python, we calculate and visualize the efficient frontier, Max Sharpe Ratio (MSR) portfolio, Global Minimum Variance (GMV) portfolio, and the Capital Market Line (CML). This analysis is an essential component of modern portfolio theory and is widely used in financial analysis and investment management.

## Project Overview

In this project, we:
1. Gathered and cleaned stock data.
2. Calculated annualized expected returns and the covariance matrix of returns.
3. Constructed and visualized the efficient frontier.
4. Identified and plotted the Max Sharpe Ratio (MSR) and Global Minimum Variance (GMV) portfolios.
5. Plotted the Capital Market Line (CML) to show the optimal risk-return profile for a given risk-free rate.

This project provides a foundational look into portfolio optimization techniques, commonly used in quantitative finance.

## Table of Contents

- [Installation](#installation)
- [Data Collection](#data-collection)
- [Analysis Steps](#analysis-steps)
- [Results](#results)
- [Future Enhancements](#future-enhancements)
- [Acknowledgments](#acknowledgments)

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/George-Dros/portfolio-optimization.git
   cd portfolio-optimization

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt

3. Data Collection

   The project uses stock price data to calculate historical returns and risks. The data can be sourced from APIs like Yahoo Finance or downloaded directly as CSV       files for the assets included in the analysis. The data should cover daily price information to allow accurate calculation of daily returns, which are then          annualized.

   Ensure that you have a dataset containing daily prices of multiple stocks over a sufficient period (at least a year) for meaningful analysis. Clean any missing       values and format the data to have datetime indices and stock tickers as column headers.

4. Analysis Steps
i. Data Preparation

    Cleaning and Structuring Data: We clean the data to remove missing values and format it for analysis.
    Annualization: Daily returns and risks are converted to annual figures for accurate portfolio comparisons.

ii. Calculating Risk and Return

   Expected Returns: Calculated as the annualized mean of historical returns for each asset.
   Covariance Matrix: Calculated to understand the co-movement between assets, which is essential for portfolio risk estimation.

ii. Efficient Frontier and Portfolio Optimization

   Efficient Frontier: Using portfolio theory, we construct a set of optimal portfolios that offer the best possible returns for a given level of risk.
   Max Sharpe Ratio (MSR) Portfolio: Identified as the portfolio that maximizes the Sharpe ratio, providing the best risk-adjusted return.
   Global Minimum Variance (GMV) Portfolio: The portfolio with the least volatility among all possible portfolios.

iv. Visualization

   Efficient Frontier Plot: Shows the range of optimal portfolios, allowing a visual comparison of return versus risk.
   MSR and GMV Portfolio Markers: Highlighted on the efficient frontier plot for reference.
   Capital Market Line (CML): Plotted from the risk-free rate to the MSR portfolio, illustrating the optimal risk-return trade-off.

5. Results

The following key results are presented in this project:

  i.   Efficient Frontier: A visualization of portfolios with the best risk-return combinations.
  ii.  Max Sharpe Ratio (MSR) Portfolio: Offers the highest return per unit of risk, marked on the plot as a red star.
  iii. Global Minimum Variance (GMV) Portfolio: The portfolio with the lowest possible volatility, marked on the plot as an orange circle.
   iv. Capital Market Line (CML): Shows the best possible risk-return profile by combining the risk-free asset with the MSR portfolio.

Each of these elements provides insights into optimal portfolio construction and helps identify the best portfolios for different levels of risk tolerance.   

6. Future Enhancements

Possible future additions to this project include:

   Backtesting the Portfolios: Simulate the performance of the MSR and GMV portfolios over time to assess their historical effectiveness.
   Alternative Risk Measures: Incorporate Value at Risk (VaR), Conditional Value at Risk (CVaR), and drawdowns to better understand downside risk.
   Additional Constraints: Implement sector constraints, weight limits, or leverage the Black-Litterman model for enhanced portfolio construction.
   Interactive Visualizations: Create interactive plots using Plotly or Streamlit for a more engaging demonstration of portfolio performance.


7. Acknowledgments

This project is inspired by modern portfolio theory and is built on the foundational ideas proposed by Harry Markowitz. Special thanks to the Coursera course material from the EDHEC Risk Institute for guidance on implementing portfolio optimization methods.   
