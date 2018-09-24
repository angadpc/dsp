[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

Solution: Cohen's Effect essentially finds the difference between the MEAN quantities of two variables. So in the case of Total Weight in pounds for first born babies & the rest, it takes the MEAN weight of all first born babies & the MEAN weight of all the others & finds the mean difference which has to be divided by the combined standard deviations of the two groups. Pooled standard deviation is the average of the standard deviations of the individual groups.

```meanTotalWeightFirstBabies = firsts.totalwgt_lb.mean()
meanTotalWeightOthersBabies = others.totalwgt_lb.mean()
print(meanTotalWeightFirstBabies)
print(meanTotalWeightOthersBabies)
print("Cohen effect on total weight between first & others: " + str(abs(CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)))
```

In the above code, I first recorded mean total weights for first born babies and for other babies to see on average who is heavier. The mean weight of others was 7.32 lbs and mean weight of first born babies was 7.20 lbs indicating that on average, babies in the "others" category weighed more than first born babies. 

The Cohen's D for total weight between the two groups above was 0.08 standard deviations while the Cohen's D for preg length between the above two groups was 0.02 standard deviations. The difference in mean for the two groups was higher for the total weight compared to the difference in mean for pregnancy length. 
