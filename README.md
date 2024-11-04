# Portfolio Optimization and Efficient Frontier Analysis

This project demonstrates portfolio optimization techniques to identify optimal risk-return trade-offs for a diversified set of financial assets. Using Python, we calculate and visualize the **Efficient Frontier**, **Max Sharpe Ratio (MSR) Portfolio**, **Global Minimum Variance (GMV) Portfolio**, and the **Capital Market Line (CML)**. Additionally, we incorporate **benchmark comparisons** and perform **backtesting with rolling metrics** to validate portfolio performance. This analysis is central to modern portfolio theory, commonly applied in financial analysis and investment management.

## Project Overview

In this project, we:
1. Gathered and cleaned historical stock data.
2. Calculated annualized returns and the covariance matrix for portfolio optimization.
3. Constructed and visualized the efficient frontier.
4. Identified and plotted the Max Sharpe Ratio (MSR) and Global Minimum Variance (GMV) portfolios.
5. Included the Capital Market Line (CML) to illustrate the optimal risk-return trade-off with a risk-free rate.
6. Performed backtesting to evaluate historical performance, including benchmark comparisons.
7. Conducted rolling Sharpe Ratio and volatility analysis for dynamic insights.
8. Analyzed drawdowns to assess downside risk and portfolio resilience.

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

The project utilizes stock price data to calculate historical returns and risks. Data can be sourced from Yahoo Finance or directly imported as CSV files. Ensure the data includes daily prices over a sufficient time frame (preferably 5+ years) for meaningful analysis. After importing, clean missing values and format the data with datetime indices and ticker symbols as column headers.

4. Analysis Steps
   
   i. Data Preparation

    Cleaning and Structuring Data: We clean the data to remove missing values and format it for analysis.
    Annualization: Daily returns and risks are converted to annual figures for accurate portfolio comparisons.

   ii. Calculating Risk and Return

   Expected Returns: nnualized average returns for each asset.
   Covariance Matrix: Evaluates the co-movement between assets, essential for estimating portfolio risk.

   iii. Efficient Frontier and Portfolio Optimization

   Efficient Frontier: Constructed using modern portfolio theory to illustrate optimal risk-return portfolios.
   Max Sharpe Ratio (MSR) Portfolio: Identified as the portfolio that maximizes the Sharpe ratio, providing the best risk-adjusted return.
   Global Minimum Variance (GMV) Portfolio: Portfolio that maximizes risk-adjusted return (Sharpe Ratio).

iv. Benchmark Selection: A global benchmark (MSCI World Index) was included for comparative analysis.
   Rolling Sharpe Ratios: Calculated rolling Sharpe Ratios over a 1-year window for MSR, GMV, and benchmark portfolios.
   Rolling Volatility: Examined volatility trends to understand risk exposure dynamics over time.

v. Visualization

   Efficient Frontier Plot: Displays the range of optimal portfolios with risk-return profiles.
   Portfolio Markers: Highlights MSR and GMV portfolios on the efficient frontier.
   Capital Market Line (CML): Plotted from the risk-free rate to the MSR portfolio, showing the best possible risk-return trade-off.
   Cumulative Returns: Shows backtested performance of MSR, GMV, and benchmark portfolios over time.
   Rolling Metrics: Visualizes rolling Sharpe Ratios and volatilities for dynamic analysis.
   Drawdown Analysis: Assesses portfolio resilience during market downturns by comparing drawdowns.

5. Results

The project’s main results include:

   Efficient Frontier: A visual display of the optimal portfolios across different risk levels.
   Max Sharpe Ratio (MSR) Portfolio: Portfolio offering the best risk-adjusted return, marked on the efficient            frontier.
   Global Minimum Variance (GMV) Portfolio: The portfolio with the lowest possible volatility, also marked.
   Capital Market Line (CML): Illustrates the optimal risk-return trade-off.
   Benchmark Comparison: Provides context to the portfolio performance relative to a global market index.
   Rolling Metrics: Show trends in risk-adjusted returns and volatility, allowing for dynamic performance insights.
   Drawdown Analysis: Highlights downside risk and the resilience of each portfolio compared to the benchmark.

   Each element provides valuable insights into the risk-return characteristics of optimized portfolios, aiding in       the selection of portfolios suited for different risk tolerances.
   
6. Future Enhancements

Possible future additions to the project include:

Extended Backtesting: Perform deeper backtesting of MSR and GMV portfolios across different economic cycles.
Alternative Risk Metrics: Incorporate metrics like Conditional Value at Risk (CVaR) and Sortino Ratio for more nuanced risk assessment.
Interactive Visualizations: Implement tools like Plotly or Streamlit for interactive analysis.
Machine Learning for Optimization: Explore ML models to improve portfolio weighting strategies based on market trends.


7. Acknowledgments

This project is inspired by modern portfolio theory and is built on the foundational ideas proposed by Harry Markowitz. Special thanks to the Coursera course material from the EDHEC Risk Institute for guidance on implementing portfolio optimization methods.   
