﻿# FinTech-MonteCarlo-project
A Python-based portfolio optimization project that analyzes S&P 500 sectors using Modern Portfolio Theory to find optimal asset allocations.
Features

Fetches real-time S&P 500 sector data
Calculates sector-wise average prices and returns
Performs Monte Carlo simulation for portfolio optimization
Identifies portfolios with maximum Sharpe ratio and minimum volatility
Generates visualization of efficient frontier

Dependencies
Copypandas
yfinance
numpy
matplotlib
scipy
scikit-learn
Data Sources

S&P 500 companies data from Wikipedia
Historical price data via Yahoo Finance API

Key Components

Data Collection

Fetches S&P 500 company list
Downloads historical price data
Calculates sector-wise averages


Portfolio Analysis

Calculates log returns
Performs Monte Carlo simulation with 20,000 iterations
Computes portfolio metrics (returns, volatility, Sharpe ratio)


Optimization Results

Maximum Sharpe Ratio Portfolio
Minimum Volatility Portfolio
Portfolio weight distributions across sectors



Usage

Install required dependencies:

bashCopypip install pandas yfinance numpy matplotlib scipy scikit-learn

Run the notebook:

Each cell is sequential and builds upon previous calculations
Data is automatically fetched and processed
Results are displayed with portfolio metrics and weights



Output Files

sp500_sectors_avg_prices.xlsx: Sector-wise average prices
log_return.xlsx: Calculated log returns for all sectors

Portfolio Metrics
The analysis provides two optimized portfolios:

Maximum Sharpe Ratio Portfolio

Optimizes risk-adjusted returns
Uses risk-free rate of 1%
Considers transaction costs and rebalancing


Minimum Volatility Portfolio

Focuses on risk minimization
Provides most stable returns
Optimal for risk-averse investors



Notes

Data is fetched for the last 90 days
Analysis assumes daily rebalancing
Log returns are filtered for positive values only
Monte Carlo simulation uses 20,000 random portfolio weights
