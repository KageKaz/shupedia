---
aliases:
  - significance tests
date: 2024-04-06
---
# Conditions

^a9a273

* random
	* necessary to give an unbiased representation of the [[population]].
* [[normal distribution|normal]] (for [[z-test|t-tests]] and [[z-test|z-tests]])
	* we can assume approximate normality for proportions if the expected number of success and failures are both at least 10 (it isn't skewed too far to 0 or 1)
	* for [[mean|means]], if $n\geq 30$, or there are no [[outlier|outliers]] or strong skew, we can assume normality.
* [[independent]]
	* In order to calculate [[standard deviation]], we need [[independent]] samples. This is because the formula for [[standard deviation]] is based off of assuming we are dealing with [[binomial variable|binomial variables]], which are [[independent|independently]] sampled.
		* see [[sampling distribution#^468e52]]
# Types
* [[z-test|z-tests]] 
* [[t-test|t-tests]]
* [[chi-squared goodness of fit test]]
# Errors
When performing a [[significance test]], we can either make a [[type 1 error]] or [[type 2 error]]
# Power
power is the [[probability]] of rejecting the [[null hypothesis]] when it is false. In other words, the [[probability]] of not making a [[type 2 error]]. 

To increase power, we can increase our [[significance level]]. This makes it easier to reject the [[null hypothesis]], meaning it is harder to make a [[type 2 error]] and easier to make a [[type 1 error]].  

We can also increase sample size, which will make our sample closer to the true [[parameter]], decreasing the chance we get some [[outlier]] that makes it seems as though the [[null hypothesis]] is true.