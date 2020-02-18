# Factor investigation, share issaunce (Pontiff 2007)
Run a factor_analysis using prices and shares issuance of international equities

Share issuance effect had shown a strong and significant effect on future stock returns, theories support manager's intent to profit from overpriced situation by issuing shares to the market and from underpriced situations by buying back shares. (Pontiff 2007)

We run a quantopian backtest in order to explore exposition of share issaunce factor to common risk factor such as, volatility, size, investment policy, etc.

The results above are promising for different holding periods that can lead to use share issuance effect in a trading strategy. In order to go further into this hypothesis we back test the share issuance effect through an algorithmic backtester, to determine whether this anomaly can be exploited in a trading strategy.  We use the annual share issuance to simulate our long/short strategy using a backtest algorithm on period 2010-2018 to avoid the financial crisis.  

Furthermore, we use a market friction cost of 0.5% taken for each transaction and a capital base of 10M for a maximum position size of 0.25%. Moreover, we used a backtestesting long/short strategy in order to simulate the trading strategy, sectors neutral, market neutral and covered from five risk factor, momentum, size, book-value, short-term reversal and volatility. We found out that this strategy that aims to maximize the alpha using an optimization package (Pyfolio) failed to obtain strong results that corroborate the share issuance effect once taking into account the market friction costs of 0.05% (On the following graph we see that almost the full backtest period is in a drawdown period resulting in very low confidence using this factor in a trading strategy). 
 
The result of this strategy show a very low alpha factor of 0.02 for a beta of -0.09. We can interpret these results as a demonstration of a market efficiency that erase the returns of this strategy when we take into account market friction costs. We can conclude the algorithmic backtest section with the assumption that the share issuance effect is rather too small or already incorporated into the market as a proof of market efficiency when we use the market friction cost.



https://github.com/Lucas-BLP/test_alphalens/blob/master/Alphalens_results_notebook.ipynb
