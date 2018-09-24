[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```
resp = nsfg.ReadFemResp()
actual_pmf = thinkstats2.Pmf(resp.numkdhh, label="actual")
biased_pmf = BiasPmf(actual_pmf, label="biased" )
print(actual_pmf)
print(biased_pmf)
thinkplot.PrePlot(2)
thinkplot.Pmfs([actual_pmf, biased_pmf])
thinkplot.Config(xlabel = "Num of Children", ylabel = "PMF")
```

The above code is straightforward. I first calculated the actual PMF using the thinkstats PMF function which used actual data, and then I calculared the biased_pmf using the BiasPmf method provided which calculates the PMF with biased data. 
