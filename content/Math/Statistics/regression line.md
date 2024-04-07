---
aliases:
  - line-of-best-fit
  - best-fit-line
  - least-squares regression line
---
# Linear
> [!info] 
> $\hat{y}=a+bx$
> $m=r\frac{s_{y}}{s_{x}}$
> $(\bar{x},\bar{y})$ is definitely a point

intuition: if r is 1, then your slope is just equal to the ratio of [[standard deviation|standard deviations]], the [[mean|average]] change in y over the [[mean|average]] change in x. if r is zero, your slope is zero. if r is a little less, then your slope is a little less than the exact ratio of [[standard deviation|standard deviations]].

# Inference
### Conditions 
1. Linear relationship between x and y
2. [[independent]] observations ([[10% rule]])
3. normally distributed across the line ![[Pasted image 20240406224342.png]]
4. equal variance, each of those [[distribution|distributions]] has the same spread
5. random sampling
^bccf14


we can represent the regression line of the [[population]] as
$$
\hat{y}=\alpha+\beta x
$$
unfortunately, we can't usually sample the entire [[population]]. Thus, we take a smaller sample and create a sample regression line.
$$
\hat{y}=a_{1}+b_{1}x
$$
we can utilize [[confidence interval#^cfc264|confidence intervals]] and [[significance test|significance tests]] to determine how well this regression line corresponds to the truth. 

