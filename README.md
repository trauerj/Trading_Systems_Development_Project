# Trading systems development Project Overview
* The first trading system based on the Exponential Moving Average (EMA) and Moving average convergence/divergence (MACD) indicator.
* The second algorithm based on a combination of MACD and RSI indicators.
* The third one based on a combination of  RSI indicator and an other "indicator". The basis of this "indicator" is the Gaussian like distribution of the close price changes.

 - The final equities are 257398.2, 455316.85 and 645539.03 for first, second and third strategy.
 - Use the whole budget at every trade.

## Code
* Python 3 (ipykernel)
* Packages: pandas, numpy, matplotlib, talib, pandas_ta, yfinance, datetime

## Different Strategies

I tried three different strategy:
* Only the MACD indicator.
* Combination of RSI and MACD indicators.
* Combination of RSI indicator and an "own" "indicator".

* The first algorithm buy ETFs if the Signal line cross the MACD line from below and the Signal line value on the day before is less than -1.5. If the Signal line cross the MACD line from above and the Signal line value on the day before is greater than 1.5 then sell the ETFs.
* For the second system, I added an other condition to buy or sell ETFs. If the current RSI value is higher than 75 then buy ETFs. If the RSI value lower than 25 then sell ETFs.
* The third algorithm used the RSI indicator on the same way as the second did, but I wrote an additional condition to buy or sell ETFs. If the Close price changes are higher than the standard deviation of price changes on the last two days then buy ETFs. If the Close price changes are lower than the standard deviation of price changes on the last three days then sell ETFs.

![Performance](https://github.com/trauerj/Trading_Systems_Development_Project/blob/main/dist_plot.png)

### Meaning of the "own indicator"
The thought behind the 

## Strategy Performance


![Performance](https://github.com/trauerj/Trading_Systems_Development_Project/blob/main/Equity_Curves.png)
_**This figure shows us the Equity curves of the different algorithms.**_

## Conclusion

