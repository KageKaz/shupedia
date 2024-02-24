---
aliases:
  - sampling distributions
---
Suppose we have a [[population]] that we want to find a [[parameter]] of.  We can take a random sample of the [[parameter]]  and get a [[statistic]] from that and use that to figure out what the [[parameter]] is. But the [[statistic]] doesn't necessarily always equal the [[parameter]]. 

The [[sampling distribution]] is the distribution of all possible values of that [[statistic]].

# Sample [[mean]]
To find if the [[sampling distribution]] of the sample [[mean]] is [[normal distribution|normal]], you can use the [[central limit theorem]]. Because [[mean]] is unbiased, the [[mean]] of the [[sampling distribution]] is equal to the [[mean]] of the population.
The greater your sample size, the smaller the [[Math/Statistics/variance]] of the [[sampling distribution]].  Thus, $\sigma_{\bar{x}}^2=\frac{\sigma^2}{n}$
Solving for [[standard deviation]]: $$\sigma_{\bar{x}}=\frac{\sigma}{\sqrt{ n }}$$
## Difference of Sample Means
The [[mean]] of the difference of two [[sampling distribution|sampling distributions]] is the [[mean]] of those [[sampling distribution|sampling distributions]] subtracted from each other. 

The equation for the [[standard deviation]] of the difference can be derived:
* We cannot subtract [[standard deviation|standard deviations]] because there is a square root. We can add the [[Math/Statistics/variance|variances]] though. The reason why we add and do not subtract is because [[Math/Statistics/variance]] is a measure of spread, and so when combining [[sampling distribution|sampling distributions]] it always increases. 
*  When we use the formula for [[standard deviation]] above, we get (assuming independence):
$$
\sigma_{\bar{x_{1}}}-\sigma_{\bar{x_{2}}}=\frac{\sigma_{1}}{\sqrt{ n_{1} }}+\frac{\sigma_2}{\sqrt{ n_{2} }}
$$

# Sample Proportion
The [[sampling distribution]] of the sample proportion is [[normal distribution|normal]] when it passes the [[large counts condition]]. 

The [[mean]] of this [[sampling distribution]] is equal to the proportion of the population. The [[standard deviation]] of this [[sampling distribution]] is equal to the [[standard deviation]] of the desired part of the population divided by the sample size, because the proportion is equal to the desired part of the population divided by sample size. This simplifies to $$
\sigma_{\hat{p}}=\sqrt{\frac{p(1-p)}{n} }
$$
## Difference of Sample Proportions
The [[mean]] of the difference of two [[sampling distribution|sampling distributions]] is the [[mean]] of the proportion of those [[sampling distribution|sampling distributions]] subtracted from each other. 
The shape of the distribution remains [[normal distribution|normal]] if both [[sampling distribution|sampling distributions]] are [[normal distribution|normal]].
The equation for the [[standard deviation]] of the difference can be derived:
* We cannot subtract [[standard deviation|standard deviations]] because there is a square root. We can add the [[variance|variances]]  though. The reason why we add and do not subtract is because [[variance]] is a measure of spread, and so when combining [[sampling distribution|sampling distributions]] it always increases. 
* When we use the formula for [[standard deviation]] above, we get (assuming independence):
$$
\sigma_{\hat{p_{1}}}-\sigma_{\hat{p_{2}}}=\sqrt{ \frac{p_{1}(1-p_{2})}{n}+\frac{p_{2}(1-p_{2})}{n} }
$$
