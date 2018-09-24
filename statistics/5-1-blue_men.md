[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

```
import scipy.stats
mu = 178
sigma = 7.7
distribution = scipy.stats.norm(loc=mu, scale=sigma)
lowBound = distribution.cdf(177.8)
upperbound = distribution.cdf(185.4)
```

In a normal distribution, the "high" value listed in the code above says the total % of men that fall below the height 6 1 while the "low" value listed in the code says the % of men below the height 5 10. To find the height between the two, simply subtract the probability cdf values of each of the variables. The result is 34% of men fall between the bounds. 



