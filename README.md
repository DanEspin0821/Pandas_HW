## Portfolio Analysis

Background
Harold's ask:
Determine which portfolio is performing the best across many areas: 
* volatility
* returns
* risk
* Sharpe ratios

Harld needs to analyze and visualize the major metrics of the portfolios across all of these areas, and determine which portfolio outperformed the others. 
Harld's provided input files inlcude:
Historical daily returns of several portfolios: 
* Firm's algorithmic portfolios
* Portfolios of famous "whale" investors like Warren Buffett
* Hedge/Mutual funds
* Custom portfolio of stocks
* S&P 500


Requirements:
Read in and Wrangle Returns Data
Determine Success of Each Portfolio
Choose and Evaluate a Custom Portfolio

## Prepare the Data

Read / clean several CSV files for analysis. The CSV files include whale portfolio returns, algorithmic trading portfolio returns, and S&P 500 historical prices.

Read in each of the CSV files as a DataFrame. Convert the dates to a DateTimeIndex.

Detect and remove null values.

Remove dollar signs from the numeric values and convert the data types as needed.

The whale portfolios and algorithmic portfolio CSV files contain daily returns, but the S&P 500 CSV file contains closing prices. Convert the S&P 500 closing prices to daily returns.

Join Whale Returns, Algorithmic Returns, and the S&P 500 Returns into a single DataFrame with columns for each portfolio's returns.

## Conduct Quantitative Analysis
Analyze the data to see if any of the portfolios outperform the stock market (i.e., the S&P 500).

Calculate and plot cumulative returns.

Create a box plot for each of the returns.

Calculate the standard deviation for each portfolio.

Plot the rolling standard deviation of the firm's portfolios along with the rolling standard deviation of the S&P 500.

Construct a correlation table for the algorithmic, whale, and S&P 500 returns.

Choose one portfolio and plot a rolling beta between that portfolio's returns and S&P 500 returns.

Plot Sharpe Ratios

Using the daily returns, calculate and visualize the Sharpe ratios using a bar plot.

Determine whether the algorithmic strategies outperform both the market (S&P 500) and the whales portfolios.

Choose your own portfolio that performs just as well as the algorithmic portfolios. Investigate by:

Choosing 3-5 stocks for your own portfolio.

Download the data as CSV files and calculate the portfolio returns.
Clean the data

Add your portfolio returns to the DataFrame with the other portfolios and rerun the analysis.

## Resources
[Pandas API Docs](https://pandas.pydata.org/pandas-docs/stable/reference/index.html)

[Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.ewm.html)
