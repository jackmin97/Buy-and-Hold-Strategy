# Buy-and-Hold-Strategy
The buy and hold is an investment strategy in which the investor buys the assets and hold them for the long term. The holding period can vary from months to years or even decades. In this buy and hold strategy, a portfolio of eight US stocks is created and rebalanced every month.

### 1. Read daily stocks data
The closing prices of the stocks are stored in the csv file. read_csv method of pandas can be used the read csv files.

### 2. Convert daily to monthly data
DataFrame.asfreq() function is used to convert timeseries to specified frequency.
The missing values in the data are dropped using the dropna function.

### 3. Calculate monthly returns
DataFrame.pct_change() is used to calculate the percentage return of the prices.
The missing values in the data are dropped using the dropna function.

### 4. Calculate portfolio returns
We allocate capital to each stock equally. Therefore, we take the mean of monthly returns to calculate the portfolio returns.

Note: If you want to assign specific weights to individual stocks, then you need to multiply the allocation with each stock return and sum the product for all stocks to get total portfolio returns.

### 5. Plot cumulative portfolio returns
Matplotlib is used to plot the cumulative portfolio returns. Then, titles and labels are setted for the plot.
