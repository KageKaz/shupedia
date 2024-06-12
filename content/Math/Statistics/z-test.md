---
aliases:
  - z-tests
date: 2024-04-06
---
A z-score is![[z-score#^36a915]]
Thus, for a [[z-test]], we look at how many [[standard deviation|standard deviations]] our sample is from our [[mean]], and calculate the [[probability]] of that happening assuming our [[null hypothesis]] is true to find our [[p-value]]. 
For proportions: 
$$
z=\frac{\hat{p}-\mu}{\sqrt{\frac{p(1-p)}{n}  }}
$$
For difference in proportions:
$$
z=\frac{\hat{p}_{1}-\hat{p}_{2}}{\sqrt{\frac{ p_{1}(1-p_{1})}{n_{1}}+\frac{ p_{2}(1-p_{2})}{n_{2}} }}
$$
from here, we can use a z-table or a calculator to find our [[p-value]].