# VaRMonteCarlo
This is a very quick experiment to demonstrate hot to compute the VaR of a portfolio using a Monte Carlo simulation.
MC is a very elegant way to approximate a probability distribution with a random sampling technique. Basically it simulates thousands of times the occurrence of an event under a random setting and store the results such that, in the long term, the empirical samples obtained will tend to reflect the real probability distribution of the event.
So in this experiment:
1. we will simplify things by estimating the Expected Returns and risks of the portfolio using the historical data we have about the stocks' returns.
2. we will use MC sampling to add a random process, like a Wiener Term, to include volatility in the risk associated to the stocks's future returns, hence to add randomness in the computations of Losses and Gains.
3. Once we have all the expected losses and gains we can use a defined confidence interval to compute the quantiles of the gains distribution and to determine the VaR for this portfolio
