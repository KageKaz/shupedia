---
aliases:
  - variances
---
> [!info] variance is the typical squared distance a distribution has from the mean

# Population Variance
$$
\sigma^2=\frac{\sum_{i=1}^N(x_{i}-\mu)^2}{N}
$$
# Sample Variance
### Biased
$$
S_{n}^2=\frac{\sum_{i=1}^n(x_{i}-\mu)^2}{n}
$$
### Non-Biased
$$
S_{n-1}^2=\frac{\sum_{i=1}^n(x_{i}-\mu)^2}{n-1}
$$divided by a smaller number, so slightly larger than $S_{n}^2$
> [!question] Why do we divide by $n-1$? This is because the sample variance utilizes the sample [[mean]], which is likely different than the [[population]] [[mean]]. Dividing by N would yield the least possible variance. If we divide by n-1, its a little bigger, and closer to the true variance. This is confirmed empirically as well.