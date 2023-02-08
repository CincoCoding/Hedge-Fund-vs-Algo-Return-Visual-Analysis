# Hedge Fund vs Algo Return Analysis
## Description
The code evaluates the performance of algorithmic, hedge, and mutual fund portfolios and compares them against the S&P 500 Index.

## Libraries Used
pandas
numpy
datetime
pathlib
seaborn

## File Input
The code uses three csv files as input:
whale_returns.csv
algo_returns.csv
sp500_history.csv

## Data Preparation
Reads the csv files using pandas and sets the date as index.
Drops the NaN values.
Cleans the "Close" column of spy_data file.
Calculates daily returns for the spy_data.
Joins the data of all three portfolios (whale_returns, algo_returns, spy_data) into a single DataFrame.

## Data Visualization
Plots the daily returns of all portfolios.
Plots the cumulative returns of all portfolios.
Plots the riskiness of the Whale and Algo portfolios.
Plots the 21-day rolling standard deviation of all portfolios.
## Risk Assessment
Calculates standard deviation of daily returns for all portfolios.
Finds portfolios that have a higher standard deviation than the S&P 500.
Calculates annualized standard deviation of daily returns for all portfolios.
Calculates the 21-day rolling standard deviation of daily returns for all portfolios.
## Correlation
Prints the correlation matrix of all portfolios.
