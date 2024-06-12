---
aliases:
  - confidence intervals
date: 2024-02-02
---
 > [!definition] The confidence interval is the range of values which we are a certain [[confidence level]] certain that a [[statistic]] is within. This is equal to the [[statistic]] plus or minus the [[critical value]] times the [[standard deviation]] or [[standard error]].

> [!example] 
> A 95% confidence interval from x to y means that we are 95% sure the interval captures the mean

> [!example] 
> To find the confidence interval that the [[statistic]] is within 95% of the time, we can find the [[standard error]] by taking a sample and use that to find a range that is 2 [[standard deviation|standard deviations]] from the sample proportion. This is because our sample proportion is going to be within two [[standard deviation|standard deviations]] of the true proportion 95% of the time (assuming the [[sampling distribution]] is normal) because of the [[empirical rule]]. If the selected sample proportion was randomly further from the truth than it should have been, the [[margin of error]] will be greater.

> [!warning] 
> The confidence interval refers to the long term success rate of the [[parameter]]. The confidence interval changes, but the parameter does not. Confidence intervals don't give us evidence that a parameter equals a specific value; they give us a range of plausible values it could equal. We shouldn't say the true [[parameter]] is 95% likely to be within the interval, we should say the interval is 95% likely to capture the true [[parameter]].

## Necessary Conditions
similar to the conditions for [[significance test#^a9a273|significance tests]]
1. Random sampling (eliminate bias)
2. Normal 
	1. needs to be normal because the [[critical value]] measures the number of [[standard deviation|standard deviations]] from the sample, so the [[distribution]] needs to be standardized (eg. follows [[empirical rule]]).
	2. for proportions, [[large counts condition]]/at least 10 successes + failures in your sample
	3. for [[mean|means]], $n\geq 30$ to satisfy the [[central limit theorem]], or there are no [[outlier|outliers]] or strong skew
4. Independence - [[10% rule|ten percent rule]] 
# Proportions
$$
\hat{p}\pm z^\star \sqrt{ \frac{\hat{p}(1-\hat{p})}{n} }
$$
### Difference in Proportions
The confidence interval for a difference in proportions is equal to the difference of the sample proportions $\pm$ the [[critical value]] times the standard deviation of the [[standard error]] of the [[sampling distribution]] of the difference of proportions.
![[sampling distribution#^6da569]]

# Means
The [[standard deviation]] of the [[sampling distribution]] for a mean is 
![[sampling distribution#^278894]]
Thus to calculate our [[standard error]], we need to know what $\sigma$ is, the [[standard deviation]] of the [[population]].  Unfortunately, we usually don't know what $\sigma$ is. We can try to substitute $S_{x}$, or the [[standard deviation]] of the sample in, but this approximation tends to underestimate the true [[margin of error]].  Thus, instead of using $z^*$, we use $t^*$ for our [[critical value]].   

# Slope ([[regression line]])

^cfc264
The [[regression line#^bccf14|conditions]] are a little different 

We don't know what $\sigma_{b}$ the [[standard deviation]] of the [[sampling distribution]] of the slope of the [[regression line]] is, so we use [[standard error]] of $b$ to approximate. Thus, we use $t^*$.


