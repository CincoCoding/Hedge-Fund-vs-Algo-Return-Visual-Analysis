# Hedge Fund vs Algo Return Analysis

![Portfolio Analysis](Resources/Images/portfolio-analysis.png)

## Description
The code evaluates the performance of algorithmic, hedge, and mutual fund portfolios and compares them against the S&P 500 Index.

## Libraries Used
* pandas
* numpy
* datetime
* pathlib
* seaborn

## File Input
The code uses three csv files as input:
* whale_returns.csv
* algo_returns.csv
* sp500_history.csv

## Data Preparation
1. Reads the csv files using pandas and sets the date as index.
2. Drops the NaN values.
3. Cleans the "Close" column of spy_data file.
4. Calculates daily returns for the spy_data.
5. Joins the data of all three portfolios (whale_returns, algo_returns, spy_data) into a single DataFrame.
![dataframe](Resources/Images/returns-dataframe.png)


## Data Visualization
1. Plots the daily returns of all portfolios.
2. Plots the cumulative returns of all portfolios.
3. Plots the riskiness of the Whale and Algo portfolios.
4. Plots the 21-day rolling standard deviation of all portfolios.
## Risk Assessment
1. Calculates standard deviation of daily returns for all portfolios.
2. Finds portfolios that have a higher standard deviation than the S&P 500.
3. Calculates annualized standard deviation of daily returns for all portfolios.
4. Calculates the 21-day rolling standard deviation of daily returns for all portfolios.

## Correlation
Prints the correlation matrix of all portfolios.
