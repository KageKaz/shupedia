---
aliases:
  - confidence intervals
---
> [!info] The confidence interval is the range of values which we are a certain [[confidence level]] certain that a [[statistic]] is within. This is equal to the [[statistic]] plus or minus the [[critical value]] times the [[standard error]].

> [!example] A 95% confidence interval from x to y means that we are 95% sure the interval captures the mean

> [!example] To find the confidence interval that the [[statistic]] is within 95% of the time, we can find the [[standard error]] by taking a sample and use that to find a range that is 2 [[standard deviation|standard deviations]] from the sample proportion. This is because our sample proportion is going to be within two [[standard deviation|standard deviations]] of the true proportion 95% of the time (assuming the [[sampling distribution]] is normal) because of the [[empirical rule]]. If the selected sample proportion was randomly further from the truth than it should have been, the [[margin of error]] will be greater.

> [!warning] The confidence interval refers to the long term success rate of the [[parameter]]. The confidence interval changes, but the parameter does not. Confidence intervals don't give us evidence that a parameter equals a specific value; they give us a range of plausible values it could equal. We shouldn't say the true [[parameter]] is 95% likely to be within the interval, we should say the interval is 95% likely to capture the true [[parameter]].

# Proportions
## Necessary Conditions
1. Random sampling
2. Normal - [[large counts condition]]/at least 10 successes + failures in your sample
3. Independence - [[10% rule|ten percent rule]] 
### Difference in Proportions
The confidence interval for a difference in proportions is equal to the difference of the sample proportions $\pm$ the [[critical value]] times the standard deviation of the [[standard error]] of the [[sampling distribution]] of the difference of proportions.
$$
\sigma_{\hat{p}_{1}-\hat{p}_{2}}=\sqrt{ \frac{\hat{p}_{1}(1-\hat{p}_{1})}{n_{1}}+\frac{\hat{p}_{2}(1-\hat{p}_{2})}{n_{2}} }
$$
