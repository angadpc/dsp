[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```
randomNumList = np.random.random(1000)
pmf = thinkstats2.Pmf(randomNumList)
thinkplot.Pmf(pmf, linewidth=0.1)
thinkplot.Config(xlabel='', ylabel='PMF')
cdf = thinkstats2.Cdf(t)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='Random variate', ylabel='CDF')
```

The random numbers generated here are a continuous distribution instead of discrete distributions that we have been looking at this far so the PMF chart does not help very much in terms of displaying the distribution. But the close linearity with the slope of close to 1 of the CDF function indicates that the numbers are distributed uniformly  
