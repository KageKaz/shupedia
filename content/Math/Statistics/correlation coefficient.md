---
aliases:
  - r
---
> [!info] $r=\frac{1}{n-1}\sum\left( \frac{x_{i}-\bar{x}}{s_{x}} \right)\left( \frac{y_{i-\bar{y}}}{s^y} \right)$

essentially what we are doing is taking the product of the [[z-score|z-scores]] of each point and [[mean|averaging]] them.

$-1\leq r\leq 1$
$r$ tells us how well a line can describe the data
if r is 1, then a straight line with a positive slope can perfectly describe the data.
if r is -1, then a straight line with negative slope can perfectly describe the data.

intuition: when the [[z-score|z-scores]] have the same sign (both are below or above their respective means), the product is positive, making the average higher, leading to higher correlation. When they don't have the same sign, it contributes to a lower correlation coefficient. 

### $r^2$
> [!info] $r^2$ measures how much error is eliminated when we use a [[regression line|least-squares regression line]].

$r^2$ is also called the coefficient of determination

### Influential points
 [[outlier|outliers]], or points that don't fit the line very well influence it a lot.
 * [[outlier|outliers]] close to the mean impact the correlation coefficient the most.
 * [[outlier|outliers]] far from the mean are highly influential
   
 