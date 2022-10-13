
## Portfolio modeling

### Background

In this problem, we will construct three different portfolios of exchange-traded funds, or ETFs, and use bootstrap resampling to analyze the short-term tail risk of our portfolios.  If you're unfamiliar with exchange-traded funds, you can read a bit about them [here](http://www.investopedia.com/terms/e/etf.asp).


### The goal  

Suppose we have $100,000 in capital.  The task is to:  
- Construct two different possibilities for an ETF-based portfolio, each involving an allocation of your $100,000 in capital to somewhere between 3 and 10 different ETFs.  ETD's are taken from this database (https://etfdb.com/etfdb-categories/)  
- We downloaded the last five years of daily data on our chosen ETFs, using the functions in the `quantmod` package.   
- We used bootstrap resampling to estimate the 4-week (20 trading day) value at risk of each of your three portfolios at the 5% level.  
- Summarized our portfolios and our VaR findings.  

It is assumed that portfolios are rebalanced each day at zero transaction cost.  For example, if we're allocating our wealth evenly among 5 ETFs, we always redistribute our wealth at the end of each day so that the equal five-way split is retained, regardless of that day's appreciation/depreciation.  
 
Notes:
- If you're unfamiliar with value at risk (VaR), you can refer to any basic explanation of the idea, e.g. [here](https://en.wikipedia.org/wiki/Value_at_risk), [here](http://www.investopedia.com/articles/04/092904.asp), or [here](http://people.stern.nyu.edu/adamodar/pdfiles/papers/VAR.pdf). 
