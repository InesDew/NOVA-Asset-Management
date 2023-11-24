# Nova School of Business and Economics

## Asset Management Group Assignment 2022/2023 - T4

1. For this exercise use the file ”Tickers”, which specifies the tickers of the 50 stocks you should use
    given your group number. Retrieve monthly Book-to-Market data and monthly prices for your
    stocks from 1980. Present annualized performance statistics (average return, volatility, Sharpe
    ratio, skewness, kurtosis and max drawdown) for your stocks.
    
2. For each stock and each date, build a Momentum indicator which is defined as the cumulated
    return over the past six months (note that, by construction, during the first six months of
    the sample it will not be possible to build such momentum indicator). Use the characteristics
    Book-to-Market and Momentum to build tercile portfolios, called:V aluehigh,V aluemedand
    V aluelowfor Value (book-to-market); andMoM high,MoM medandMoM lowfor Momen-
    tum. To construct the six portfolios, at each date and for each one of the two characteristic, split
    your 50 stocks in three equally weighted groups of similar sizes (example: for momentum in Jan
    2000 you may have 16 stocks in the low Momentum group, 15 in the Middle group, 15 in the
    high Momentum group and 4 stocks with missing observations at this date). Present annualized
    performance statistics for the 6 portfolios.
    
3. Build two long-short portfolios for Value and Momentum using the tercile portfolios. Backtest
    the portfolio and an equal weighed portfolio investing in the 50 stocks. Plot cumulated returns
    and present annualized performance statistics.
    
4. Naturally, neither Value nor Momentum is the perfect predictor of returns. To combine the
    information that each characteristic contains, construct a composite characteristics. To this end,
    standardize in each month each characteristic to have a cross-sectional mean (standard deviation)
    of zero (one) and combine them into a single characteristicSitdefined as:

    <img width="300" alt="Screenshot 2023-04-29 at 18 01 17" src="https://user-images.githubusercontent.com/123978459/235314713-352e065e-d9b8-459b-b3c8-d27180ca3a94.png">

    where the Mean and Standard deviation are taken over all stocks in the cross-section of month
    t. Now, sort the stocks on the composite characteristic and construct the long-short portfolio
    using tercile portfolios on this charateristics .Backtest this long-short portfolio. Plot cumulated
    returns and present annualized performance statistics for this long-short portfolio.

5. Discuss how the performance of the strategy at the previous point compares to a mixed strategy
    that simply invests 50% in the the value long-short portfolio and %50 in the momentum long-
    short portfolio.
    
6. Consider the long-short portfolios on Value, Momentum, the mixed charateristicSans the equally
    weighted portfolio. Run performance analysis of this strategies against FF5M model. Comment
    on the alphas, the factor exposures and theR^2 of the factor regressions.
    
7. Is the performance analysis (α) driven mostly by one of the two legs (long ot short)? Discuss
    the implications for trading on long-only versus long-short tercile portfolios.
    
8. Discuss theoretically how to modify the construction of the long-short Value portfolio in order
    to make it market neutral (i.e. uncorrelated with returns on the market portfolio) over a rolling
    widow of 3 years.
